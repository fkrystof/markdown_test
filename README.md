# GET_CLIENT_SERVICES
---
## Popis
Vrátí seznam portfolií, ve kterých je daný klient obsluhován.

## Typ
Function

|aa|aaa|aaa|
|---|---|---|
|bb|bb|bb|

## Parametry

|Name|Type|Direction|Mandatory|NULL|Defaul value|Description|
|---|---|---|---|---|---|---|---|
|p_client_id|integer|in|Y|N||Id klienta, pro nějž je načítán seznam portfolií, ve kterých je obsluhován.|
|p_mode|integer|in|Y|N|Typy portfolií, které mají být načteny:<br><br>1 - pouze primární obsluha<br>2 - aktuální obsluha (primární, event. dočasný převod);<br>3 - všechny obsluhy (primární i všechny sekundární).<br><br>Pozn.: ve všech módech bude vracena i obsluha typu LOST (pokud existuje).|
|p_service_code|varchar2|in|N|Y|Typ obsluhy portfolia. Pokud NULL, budou vráceny všechny typy obsluhy.|

---
