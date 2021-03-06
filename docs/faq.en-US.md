---
order: 22
title: FAQ
type: Other
---

Before you ask a question, please check the following FAQ.

---

### What is the difference between Ant Design React and Ant Design Pro?

It can be understood that Ant Design React is a set of React component libraries, and Pro is a complete front-end scaffolding using this set of component libraries.

### How to use Ant Design Pro?

Please read the document [Getting Started](/docs/getting-started), and Ant Financial users please read [Getting Started (Ants Financial User)] (/docs/getting-start-inner).

### Can I use Ant Design Pro in a production environment?

Of course you can! Ant Design Pro is based on the latest antd version. There are currently multiple middle and backend projects in use.

### How to update Ant Design Pro?

- Upgrade the `antd` version separately for updating the base components.
- Compare the differences between different Ant Design Pro versions and manually modify the local configuration.
- You can also try merging remote branches: `git pull https://github.com/ant-design/ant-design-pro` (note that you need to resolve conflicts yourself).
- Copy the latest typical template directly on GitHub.

### `npm test` hangs on `MacOS Sierra`?

You need to install [watchman](https://github.com/facebookincubator/create-react-app/blob/master/packages/react-scripts/template/README.md#npm-test-hangs-on-macos-sierra).

### How to modify the default webpack configuration?

See [roadhog configuration](https://github.com/sorrycc/roadhog#configuration) for details.

### How to add babel plugins?

See details [roadhog extraBabelPlugins](https://github.com/sorrycc/roadhog#extrababelplugins).

### How to use static resources such as pictures?

Absolute paths can be used directly (map support is required). If you want to use local files directly, you can import them as follows.

```jsx
<img src={require('../assets/picture.png')} />
```

### How is my `#` number in my url? How to get rid of?

Please refer to the deploy document [Routing and server integration](/docs/deploy#Routing-and-server-integration).

### How to add scss support?

Open the `sass` configuration in `.webpackrc`, see [sass] (https://github.com/sorrycc/roadhog#sass).

### Git commit error?

<img src="https://gw.alipayobjects.com/zos/rmsportal/KkPUhMMpGtEdhSGfxxKz.png" width="600" />

Scaffolding defaults to the [eslint](http://eslint.org/) code style check. Please follow the prompts and resubmit it, or you can manually check `npm run lint`.

### Disable browser opening automatically on `npm start`

Modify `scripts.start` in `package.json` to:

```js
"start": "cross-env BROWSER=none roadhog server",
```

### Does Ant Design Pro support internationalization?

This is one of the features of Ant Design Pro. The first version is currently available in Chinese. Internationalization is in our 2.0 plan and will be released soon.

### English Documentation?

English Documentation will be translated in next couple of monthes, trace [ant-design/ant-design-pro#54](https://github.com/ant-design/ant-design-pro/issues/54#issuecomment-340804479) and [ant-design-pro/issues/120](https://github.com/ant-design/ant-design-pro/issues/120) for more detail.

---

More FAQs can be found in [Trouble Shooting] (https://github.com/facebookincubator/create-react-app/blob/master/packages/react-scripts/template/README.md#troubleshooting) and [roadhog] ( Https://github.com/sorrycc/roadhog). If this does not solve your problem, please [Report to us] (https://github.com/ant-design/ant-design-pro/issues).