# Schlangen működése 
kettő függvény van alapból, `init()` és `step()`, mindkettőnél kapsz egy [_api_](https://schlangen.bytewerk.org/static/docs/python/classapi_1_1Api.html) változót, ebből adatokat tudsz kérni a játéktól, használatuk lent van mutatva, és a docks entryhez van egy link. 

## init fázis
Ebben a functionben tudjuk lefuttatni azokat a kódokat amiket a spawnolásnál akarunk csinálni ez nagyrészt a szín beállításából áll, lehet beállítani memóriát ami életek között megmarad amit itt lehet célszerű beolvasni. Az utóbbi nem néztem meg hogy működik de ha érdekel a dockson van információ

## step fázis 
a `step()` funkció fog lefutni minden frame-en, és ide kell írni a fő logikáját a kígyódnak. ez a function 3 értéket ad vissza, a az irányváltozásod, azt hogy boostolj-e és hogy megölje-e magát a kígyó. Ezek működése a példa kódban van jól érthetően le van írva a commmentekben

### [food](https://schlangen.bytewerk.org/static/docs/python/classapi_1_1IpcFoodInfo.html)
class ami a látható foodokról ad információt
```python
for food in api.food:
    api.log(food.dist)
```
### [segments](https://schlangen.bytewerk.org/static/docs/python/classapi_1_1IpcSegmentInfo.html)
class ami az információt ad az összes szegmensekről amit látsz.
```python
for seg in api.segments:
    api.log(seg.dist)
```

### [bots](https://schlangen.bytewerk.org/static/docs/python/classapi_1_1IpcBotInfo.html)
class amiből a közeli botok nevét és id-jét lekérheted
```python
for b in api.bots:
    api.log(b.bot_name)
```
### [self_info](https://schlangen.bytewerk.org/static/docs/python/classapi_1_1IpcSelfInfo.html)
class amivel magadról kérhetsz adatokat
```python
api.log(api.self_info.sight_radius)
```