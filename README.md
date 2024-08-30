# nx + expo-router + nativewind V4 issue

<!-- https://github.com/nativewind/nativewind/issues/972 -->

<!-- 
https://github.com/nrwl/nx/discussions/21847?sort=old  

i followed these instructions:
https://github.com/nrwl/nx/issues/23101#issuecomment-2147308325  
-->

<a alt="Nx logo" href="https://nx.dev" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/nrwl/nx/master/images/nx-logo.png" width="45"></a>

✨ **This workspace has been generated by [Nx, Smart Monorepos · Fast CI.](https://nx.dev)** ✨


## Pre-requisites

node v20.14.0  
npm v10.7.0  

## Setup

```bash
npm install
```

## Start the app

```bash
npx nx start mobile
```

## The issue

Nativewind V4 is not working with Expo Router.

For example the `Text` component in `apps/mobile/app/(tabs)/index.tsx` is not styled.

```tsx
<Text className="text-red-500 text-2xl">Tab One</Text>
```

Adding `verifyInstallation` to `apps/mobile/app/(tabs)/index.tsx` will print the following error:
```tsx
const isNativeWindVerified = verifyInstallation();
console.log('isNativeWindVerified', isNativeWindVerified);
```

```
ERROR  Error: Nativewind received no data. Please refer to http://nativewind.dev/troubleshooting#no-data
```# nx-expo-nativewind-v4
