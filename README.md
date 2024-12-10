# show_annotation_for_teeth3ds

This program reads an OBJ file of a 3D model and an annotation JSON file, and displays the model with colors corresponding to the labels assigned to each vertex.

## Usage

```sh
python [show_annoation_for_teeth3ds.py](http://_vscodecontentref_/0) <obj_filepath>
```

### Arguments
- `<obj_filepath>`: Path to the OBJ file. It is assumed that a JSON file with the same name, written in teeth3ds format, exists in the same directory.

## Requirements
Install the required Python packages using the following command:

```sh
pip install -r requirements.txt
```

## File Structure
```
- fdi_number.json
- ODC3F7X8/
  - ODC3F7X8_lower.json
  - ODC3F7X8_lower.obj
- README.md
- requirements.txt
- show_annoation_for_teeth3ds.py
```

- `fdi_number.json`: Contains the color definitions for each label.
- `ODC3F7X8/ODC3F7X8_lower.json`: Annotation JSON file with labels for each vertex.
- `ODC3F7X8/ODC3F7X8_lower.obj`: 3D model file in OBJ format.
- `show_annoation_for_teeth3ds.py`: Main script to read the files and display the 3D model with colored vertices.

## Example
To display the 3D model with annotations, run the following command:

```sh
python show_annoation_for_teeth3ds.py ODC3F7X8/ODC3F7X8_lower.obj
```

This will read the ODC3F7X8_lower.obj file and the corresponding ODC3F7X8_lower.json file, and display the 3D model with vertex colors based on the labels defined in the JSON file.
