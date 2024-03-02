# Adventurer 3 Orca Slicer Profile

This is a working Orca Slicer profile for the Flashforge Adventurer 3 Series 3D Printers.

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

Add the relevant print profiles to the ```process_list``` parameter:

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

Add the relevant filaments to the ```filament_list``` parameter:

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

Add Nozzle information to the ```machine_list``` parameter:

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

Reload Orca Slicer once all details have been added

Find the Adventurer 3 and select the relevant nozzle.

Tweak settings as necessary and enjoy.

