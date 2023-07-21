# Single Page Applications with Vue
01. What is the entrypoint of an application?

  > | either the main.js or app.js |

02. What is the difference between a vue `component` and `page`?

  > | At their core, they are both the same thing. both a vue page using a vue template. the difference though is components are brought into pages. You wont bring a page into a component. I.E. Home page has a profile component on it that stores all the html/js/css for the profiles part of the whole home page.|

03. What is ***Component-Based Architecture***?

  > | What we have been doing in Vue, bit different from MVC. It's where we build components out which are parts of our one page, that way you can troubleshoot an individual component as well as reuse it instead of just having your whole backend/front end on one page. |

04. What are the three tags that make up a Vue component?

  > | template, script, and style |

05. What are ***lifecycle hooks***? What are lifecycle hooks used for?

  > | Lifecycle hooks is the lifecycle of the webpage loading process, that allows you to 'hook' into various stages of the components lifecycle. They're used to load things onmount, unmount, created ect. Allows you to run certain code at certain lifecycle of the page/component |

06. Which component in Vue does the vue-router use to mount pages onto?

  > | Router view |

07. What is the difference between the `AppState` and the state object within a component?

  > | Appstate is your global data storage, while state object within a component would be just data stored in that individual component. When we set a state object in a component like for instant 'Account: null' that would be the state object, when we use the computed property we are referencing the Appstate with the new object we just made. I.E. 'Account: computed(()
   =>AppState.Account)' |

08. What is the responsibility of `Services` in our Vue projects?

  > | Same as our previous projects, to handle any changing of data in the Appstate. |

09. What are ***props*** and how are they used? Provide an example

  > | Props is a way for us to pass data from one component to another in a parent/child relationship. (unidirectional flow)|

10. What is the Vue method used to create watchable objects such as `state` or `AppState`?

  > | Computed and Reactive are two Vue methods that are used to create watchable objects, similar to how we used the on and emit method previously.|
