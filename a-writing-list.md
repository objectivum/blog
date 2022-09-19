# Elasticsearch

 * current experience with statistics
 * arrays of values by default
 * re-use/parameterize large query body

# Etc.

 * i18n Facade
 * caching mechanisms => details to decide upon later, replace with functional interfaces/programming; defer decisions upon details...
 * problem-based learning (?) at work? false sense of mastering?
 * custom Jackson mapping, mapping raw JSON, etc.
 * Oualline, Program Design, reusability
   * `boolean itemTypeExists(@NotNull String itemTypeId)` <> `boolean itemTypesExist(ConfigContext context)`
 * Tagging experience, findCommonTagLabelsFor(), NavigableMap
 * ```@NotNull
    public <T, C extends Collection<? super T>> C findAllItemTypes(
      @NotNull BiFunction<String, JsonNode, T> itemTypeFactory, @NotNull Supplier<C> collectionFactory) { ... }
   ```
 * Cognitive Complexity / SonarQube; might streams help? -- calculate Cognitive Complexity for the 1st example [here](https://developer.ibm.com/articles/j-java-streams-1-brian-goetz/)
 * Error handling strategy in Spring Boot-based applications (not libs!)
   * I usually don't (want to) care about the exception
   * I might want to care sometimes => I use a few well-defined exceptions
   * Do I imply logging as feedback? (because cross-cutting concerns then come together)
   * Consider all ports / inputs and how we report back to either the user or support or...
   * Techniques: log and continue (how?); should we log-and-throw, after all? Throw and catch at ports (since it's usually little else we can do)
   * In a (typical? -- nice adjective to guide the reader :) ) application, we usually log (or at least want to) every or most of the time while we respond only sometimes because... `The Times They Are A-Changin'` (_Bob Dylan_) and a common application does both sync and async processing
   * Batch / stream / enriching exceptions
   * Resources:
     * https://reflectoring.io/spring-boot-exception-handling/
     * https://www.toptal.com/java/spring-boot-rest-api-error-handling
     * https://auth0.com/blog/get-started-with-custom-error-handling-in-spring-boot-java/
     * https://victorrentea.ro/blog/exception-handling-guide-in-java/
     * https://victorrentea.ro/blog/presenting-exceptions-to-users/
     * https://www.youtube.com/watch?v=zko8R_alQgw&ab_channel=Devoxx
     * https://www.youtube.com/watch?v=6va1hAyh-M8&ab_channel=DevTernityConference
 
