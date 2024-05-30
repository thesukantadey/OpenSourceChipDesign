# OpenSourceChipDesign
# RTL to GDS2 Flow
![image](https://github.com/thesukantadey/OpenSourceChipDesign/assets/3337377/f96b0cc3-1399-43d5-916c-9d040c2790e7)

# Antenna Rules and Violations
![image](https://github.com/thesukantadey/OpenSourceChipDesign/assets/3337377/fdfceab0-594f-456d-bc05-f1c24f99b062)

![image](https://github.com/thesukantadey/OpenSourceChipDesign/assets/3337377/ad0360e4-f3ec-415c-aebc-1824d311b336)

![image](https://github.com/thesukantadey/OpenSourceChipDesign/assets/3337377/be6d580e-e515-4e94-9d72-75dbc353d6ec)


# Running openlane in docker and Synthesis:

```bash
docker
./flow.tcl -interactive
prep -design picorv32a
run_synthesis
```


![image](https://github.com/thesukantadey/OpenSourceChipDesign/assets/3337377/3bb595e9-3644-4735-b951-ad3cc320753f)

![image](https://github.com/thesukantadey/OpenSourceChipDesign/assets/3337377/40e956b8-8988-43c3-b8db-d622dfd85981)


# Flop ratio
![image](https://github.com/thesukantadey/OpenSourceChipDesign/assets/3337377/2ad3466b-ad04-48d7-91ec-56d3ffbfcfaf)

number of D FF (dfxtp_2) = 1613 \
number of cells = 14876 \
Flop ratio = 1613/14876 = 0.1084

# Floorplanning and Viewing layout in Magic

```bash
run_floorplan
```
![image](https://github.com/thesukantadey/OpenSourceChipDesign/assets/3337377/8e3f09c2-87e7-43e4-b9ce-aebfb03a6ab7)

![image](https://github.com/thesukantadey/OpenSourceChipDesign/assets/3337377/7435c1ac-2a74-4a89-990f-1f7a913461b9)


```bash
magic -T /home/vsduser/Desktop/work/tools/openlane_working_dir/pdks/sky130A/libs.tech/magic/sky130A.tech lef read results/floorplan/merged_unpadded.lef def read results/floorplan/picorv32a.floorplan.def
```
![image](https://github.com/thesukantadey/OpenSourceChipDesign/assets/3337377/632f7a99-59ed-486b-a4d7-8877226ea161)
