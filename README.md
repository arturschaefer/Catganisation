# Catganisation

Cats need your help, and with this app everyone can login and see beautiful cats, because they are so amazing.
You can use your Google Account to login the app.

In the first screen it's possible to see a list of cats and filter by country! Itsn't amazing or what? And there are more!
When you click on a card you'll see all details about that cat like image, name, description, country code, the temperament and a shortcut Wikipedia's link of the particular breed. 

## Video


## Architecture
This app was built using the Clean Architecture + MVVM.
It's also multimodule and the `app` only have the main activity and application's start. 
I choose this approach to start Koin and launch the default activity of this project.

### Libraries
There are three libraries:
- `core`: all network stuff and some extensions
- `navigation`: contains interfaces for features
- `uishared`: common resources like strings, dimens and styles

### Features
There are two main features in this app:
- `login`: first screen to login the app and manage the user
- `breed`: list of breeds and their details

## Libraries
- RxKotlin
- MockK
- Coroutines
- Retrofit
- Glide
- OkHttp
- Lottie
- ViewModel
- Timber
- Koin
- Country
- MaterialRatingBar
- Firebase Auth
- Material

### API

We use the https://docs.thecatapi.com/ to get all the info you need about cats.

## IMPORTANT
- To run this project it's necessary to create your own `CATS_API_KEY_RELEASE` and `CATS_API_KEY_DEV` in your `local.properties`.
- Create a new project in your Firebase account and put the `google-services.json` inside `app's` folder.
