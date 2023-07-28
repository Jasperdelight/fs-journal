# Managing the Fullstack Application

1. Describe the two ways to bind Data in Vue?

  > | v-bind and v-model. v-bind is one way so like binding the picture property from an object when we for loop through an array. the property coming in can change but while the html element itself stays the same, just the data coming in is changing. v-model is what we use for text areas and its 2 way binding because when you interact with the page it changes the data  |

2. The `SPA` acronym stands for what?

  > | Single page application|

3. What are some of the advantages/uses of a `SPA` over a traditional one?

  > | All the code related to that one particular thing is all in one spot. For instance an album card has all the styling on it as well as functionality of card itself. makes debugging much easier, as well as scalability |

4. What does the `onMounted` method in Vue do?

  > | Whenever the page is mounted (fancy words for refresh/ on load i believe) run this code |

5. What is the `v-model` attribute in Vue for, and when might you use it?

  > | 2 way data binding. Use for forms or anytime you want to save data the user reacts with in real time. |

6. What is the package.json file used for?

  > |Its like the 'options' for the node project, allowing you to define scripts and dependencies. |

7. Which Vue attributes(directives) could you use to conditionally render elements on a page?

  > | v-if v-else v-show |

8. What is the purpose of the `key` attribute when using `v-for` on an element?

  > | its the unique identifier so the program knows where it's at when its going through the loop. |

9. What is the `<slot>` element and what is it used for?

  > | Allows you to swap in different content depending on certain conditions, like you could have one modal but slot in different content depending on what button you press. Making you have to write much less code. |
