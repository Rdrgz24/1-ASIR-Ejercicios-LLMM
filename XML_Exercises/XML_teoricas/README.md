# Ejercicios de XML - Preguntas teóricas
Repositorio donde están las actividades de LLMM del documento de google llamado "XML+XML-DOM+Ajax+Json+RSS_exercises" relacionadas con XML.
## 1. Simple questions:
### a. How should an element with the name test element and the content "This is our first element!" look?
```xml
<test_element>This is our first element!</test_element>
```
### b. Please show (in xml-syntax) the hierarchy of the element book with the subelements chapters and author. author has the further subelements name and address.
```xml
<libro>
  <capitulo></capitulo>
  <autor>
    <nombre></nombre>
    <direccion></direccion>
  </autor>
</libro>
```
### c. How does an element with the name entry which has got 2 attributes: no with the value 24 and date with the value 27.10.2004 look?
```xml
<entry no=24 date=27.10.2004></entry>
```
## 2. XML tree structures (Analyse the XML file below.)
Abrir el archivo [Ex2.xml](/XML_Exercises/XML_teoricas/Ex2.xml) y analizar la estructura de este.
![image](https://github.com/user-attachments/assets/0f09e149-b75f-4da6-a7b9-8c6a74f665e8)
Vemos que indica el XML de una publicación, con sus item de noticias, el recurso que dentro aporta la agencia y el editor y la clase de articulo junto a la cabecera, texto y sumario.
## 3. XML structure (Analyse the following XML file. Correct errors in design.)
Solucionado en el archivo [ex3-err.txt](/XML_Exercises/XML_teoricas/ex3-err.txt), donde se explican los errores del XML y se muestra este corregido.
## 4. Mark up the following email message to identify its information content.
En vez de crear un archivo xml se mostrará la solución aquí.
```xml
<email>
  <from>
    <name>Simon North</name>
    <address>north@synopsys.com</address>
  </from>
  <to>
    <name>Nick</name>
    <address>sintac@xs4all.nl</address>
  </to>
  <subject>Hi</subject>
  <body>
    Hi Nick, this is just a quick message to say I got the material. Thanks.
  </body>
</email>
```
## 5. XML file, CD information.
Solución propuesta para ejercicio Ex5a.xml
```xml
<CDList>
  <CD>
    <recordName>VANITY</recordName>
    <artist>Bryant Barnes</artist>
    <category>Pop</category>
    <year>2024</year>
    <tracks>
      <track>
        <number>1</number>
        <title>Give Me A Sign</title>
        <duration>2:40</duration>
      </track>
      <track>
        <number>2</number>
        <title>Want You All The Time</title>
        <duration>2:22</duration>
      </track>
    </tracks>
  </CD>
</CDList>
```
Solución propuesta para ejercicio Ex5b.xml
```xml
<CDList>
  <CD serial="X34B45" disc-length="18:29">
    <recordName>VANITY</recordName>
    <artist>Bryant Barnes</artist>
    <category>Pop</category>
    <year>2000</year>
    <tracks>
      <track number="1" duration="2:40">Give Me A Sign</track>
      <track number="2" duration="2:22">Want You All The Time</track>
    </tracks>
  </CD>
</CDList>
```

## 6. XML: a letter template.
```xml
<letter>
  <sender>
    <name>Juan Pepito</name>
    <address>Av. Siempre Viva 123, Manzote</address>
  </sender>
  <receiver>
    <name>Manuel Gómez</name>
    <address>Calle Falsa 42, Sevilla</address>
  </receiver>
  <date>2025-05-12</date>
  <body>
    Estimado Manuel:
    Espero que estés bien. Solo quería saludarte y enviarte mis mejores deseos.
  </body>
  <signature>Juan</signature>
</letter>
```
## 7. The XML standard.
### a. What do comments look like in XML?
```xml
<!-- Esto es un comentario -->
```
### b. Can an attribute be repeated in the same element
No. Un atributo no puede repetirse dentro del mismo elemento.
### c. Where is it stated that the element names in opening and closing tags must match?
En la sección 3.1 del estándar XML, se establece que los nombres de las etiquetas de apertura y cierre deben coincidir exactamente (incluyendo mayúsculas y minúsculas).
