# ONNX Runtime and Blazor

## Introduction
This repository is a web application project that uses ONNX Runtime and Blazor to classify images

## Prerequisites
- .NET 6
- Visual Studio Code

## Setup

### Project
The project was created as a Blazor server applicattion with the next template:
```
dotnet new blazorserver -o demo-ortblazor --no-https
```

### Restore packages
The project uses the next packages:
```
dotnet add package Microsoft.ML.OnnxRuntime
dotnet add package SixLabors.ImageSharp
```
It's not necessary to add them again, just restore the packages or build the project

## Run the project
Just run the project in your localhost using the command:
```
dotnet run
```

In the web application open the menu tab "Ort Blazor"
Select the image of a dog located in the same project **demo-ortblazor/SampleImg/dog.jpeg**

if the project runs successfully it should show the next result:
```
Golden Retriever	0.7550826
Kuvasz	0.1418474
Clumber Spaniel	0.02673398
Otterhound	0.011237004
Sussex Spaniel	0.008394765
Pyrenean Mountain Dog	0.007158577
Labrador Retriever	0.004976533
Saluki	0.0046295193
Tibetan Terrier	0.004320859
English Setter	0.003663472
```

## Colaboration
This project was based on the [onnxruntime-csharp-cv-template](https://github.com/microsoft/onnxruntime-csharp-cv-template) and updated for .NET 6
