# form_builder_image_picker
## git@github.com:sramos30/form_builder_image_picker.git
## https://github.com/danvick/form_builder_image_picker
## https://pub.dev/packages/form_builder_image_picker

Field for picking image(s) from Gallery or Camera for flutter_form_builder  package

## Usage
```dart
FormBuilder(
  child: Column(
    mainAxisAlignment: MainAxisAlignment.center,
    children: <Widget>[
      FormBuilderImagePicker(
        name: 'photos',
        decoration: const InputDecoration(labelText: 'Pick Photos'),
        maxImages: 1,
      ),
      const SizedBox(height: 15),
      RaisedButton(onPressed: (){
        if(_formKey.currentState.saveAndValidate()){
          print(_formKey.currentState.value);
        }
      })
    ],
  ),
),
```
