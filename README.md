Simple camera app using `expo-camera/legacy`
See link [Code with Beto](https://www.youtube.com/watch?v=9EoKurp6V0I&list=LL&index=10)

## Project Creation

Create the project using:
```bash
npx create-expo-app@latest camera-code --template blank
```

## Get started

1. Install dependencies

   ```bash
   npm install
   ```

   Expo package may be installed individually with   
   ```
   npx expo install <package> 
   ``` 

2. Start the app

   ```bash
    npx expo start
   ```

## Troubleshoot

1. Replace `import { Camera, CameraType } from 'expo-camera';` with
```jsx
import { Camera, CameraType } from 'expo-camera/legacy';`
```
2. Replace `const [type, setType] = useState(Camera.Constants.Type.back)` with
```jsx
const [type, setType] = useState(CameraType.back);
```

## TO DO
Fix problem with flash