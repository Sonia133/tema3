# Soluție

## 1. Traceroute

Am implementat soluția iar aici este output-ul:
(din cauza conexiunii la internet a masinii virtuale nu trece de IP-ul de RDS)

### Ruta către IP1
```
realestate.com.au : TTL -> 1
172.8.1.1
{'country': 'United States', 'region': 'KS', 'city': 'Topeka'}
TTL -> 2
10.0.2.2
{}
Socket timeout  timed out
```

### Ruta către IP2
```
google.com.au : TTL -> 1
172.8.1.1
{'country': 'United States', 'region': 'KS', 'city': 'Topeka'}
TTL -> 2
10.0.2.2
{}
Socket timeout  timed out
```

### Ruta către IP3
```
shack.co.za : TTL -> 1
172.8.1.1
{'country': 'United States', 'region': 'KS', 'city': 'Topeka'}
TTL -> 2
10.0.2.2
{}
Socket timeout  timed out
```

### Ruta către IP4
```
rsvp.com.au : TTL -> 1
172.8.1.1
{'country': 'United States', 'region': 'KS', 'city': 'Topeka'}
TTL -> 2
10.0.2.2
{}
Socket timeout  timed out
```

## 2. Reliable UDP

### Emițător - mesaje de logging
Rulăm `docker-compose logs emitator` și punem rezultatul aici:
```
....
....
....
....
....
```


### Receptor - mesaje de logging
Rulăm `docker-compose logs receptor` și punem rezultatul aici:
```
....
....
....
....
....
```
