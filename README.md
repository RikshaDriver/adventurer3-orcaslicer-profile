# Adventurer 3 Orca Slicer Profile

<img width="800" alt="image" src="https://github.com/RikshaDriver/adventurer3-orcaslicer-profile/assets/5790757/ad5dcd8a-af04-412f-8314-64267fd806e0">
<br />
<br />
This is a working Orca Slicer profile for the Flashforge Adventurer 3 Series 3D Printers.
<br />
<br />
The installation instructions are as per below.


## 1. Copy Files

Copy the Flashforge folder under the Orca Slicer installation to the relevant profiles location.

On Windows, this folder can be found under: ```C:\Program Files\OrcaSlicer\resources\profiles\Flashforge```

## 2. Edit Flashforge.json

Manually edit Flashforge.json file under resources\profiles directory.

On Windows, this is under: ```C:\Program Files\OrcaSlicer\resources\profiles\Flashforge.json```

> [!IMPORTANT]
> If adding new items to the list, ensure you add a comma separator value ```,``` to the end of the last item before adding new parameters.


### 2.1 Add Machine Model

Add the Adventurer 3 inside the ```machine_model_list``` parameter:

```
{
  "name": "Flashforge Adventurer 3 Series",
  "sub_path": "machine/Flashforge Adventurer 3 Series.json"
}
```

### 2.2 Add Print Profile

Add the relevant print profiles inside the ```process_list``` parameter:

```
{
  "name": "0.20mm Standard @Flashforge AD3 0.4 Nozzle",
  "sub_path": "process/0.20mm Standard @Flashforge AD3 0.4 Nozzle.json"
},
{
  "name": "0.30mm Standard @Flashforge AD3 0.6 Nozzle",
  "sub_path": "process/0.30mm Standard @Flashforge AD3 0.6 Nozzle.json"
}
```

### 2.3 Add Filaments

Add the relevant filaments inside the ```filament_list``` parameter:

```
{
  "name": "Flashforge ABS",
  "sub_path": "filament/Flashforge ABS.json"
},
{
  "name": "Flashforge PETG",
  "sub_path": "filament/Flashforge PETG.json"
},
{
  "name": "Flashforge PLA",
  "sub_path": "filament/Flashforge PLA.json"
}
```

### 2.4 Add Nozzle Information

Add Nozzle information inside the ```machine_list``` parameter:

```
{
  "name": "Flashforge Adventurer 3 Series 0.4 Nozzle",
  "sub_path": "machine/Flashforge Adventurer 3 Series 0.4 nozzle.json"
},
{
  "name": "Flashforge Adventurer 3 Series 0.6 Nozzle",
  "sub_path": "machine/Flashforge Adventurer 3 Series 0.6 nozzle.json"
}
```


## 3. Usage

Reload Orca Slicer once all details have been added.

<br />
<br />
<img width="600" alt="image" src="https://github.com/RikshaDriver/adventurer3-orcaslicer-profile/assets/5790757/e3484c55-9e99-4bc4-b994-539b0e584235">
<br />
<br />

Find the Adventurer 3 and select the relevant nozzle.

Tweak print/profile settings as necessary and enjoy.


### WiFi/Network Printing

Orca Slicer currently does not support direct communication to Flashforge printers. This is likely to change, but on the interim use the following steps to print via Network/WiFi:

1. Slice Model
2. Export G-code file as ```.gcode```
3. Open exported ```.gcode``` file in Flashprint and send to printer
