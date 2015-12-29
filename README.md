# BURP RSA Extension

## Intro

This is a plugin to handle RSA Crypto encryption / decryption in Burp.

It registers two Intruder **payload processors** so you can encrypt/decrypt payloads on the **Intruder Tab**. 

It also registers a **Scanner insertion point provider**. What this does is when you request an active Burp scan, it looks in existing parameters for AES payloads that can be decrypted using the current configuration / keys. If it finds any, it registers scanner insertion points to perform injection inside the AES payloads.

Contact me via twitter at @shengqi158 for suggestions and use cases and I will try to implement them. I welcome ideas or pull requests.

## Compilation

This can be compiled normally using 'javac'. I still haven't built a build.xml or pom.xml file, but there's a jardesc file to compile and package it using Eclipse. There's a precompiled jar at the dist/ folder.

## Usage

Install the burp extension as usual in burp. 

## Screenshots
![Alt text](/../screenshots/screenshots/burpaes_sshot1.PNG?raw=true "Burp AES extention screenshot")
