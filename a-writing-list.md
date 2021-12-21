# Elasticsearch

 * current experience with statistics
 * arrays of values by default
 * re-use/parameterize large query body

# Etc.

 * i18n Facade
 * caching mechanisms => details to decide upon later, replace with functional interfaces/programming; defer decisions upon details...
 * problem-based learning (?) at work? false sense of mastering?
 * CSV batch / stream / enriching exceptions
 * custom Jackson mapping, mapping raw JSON, etc.
 * Oualline, Program Design, reusability
   * `boolean itemTypeExists(@NotNull String itemTypeId)` <> `boolean itemTypesExist(ConfigContext context)`
 * Tagging experience, findCommonTagLabelsFor(), NavigableMap
 * ```@NotNull
    public <T, C extends Collection<? super T>> C findAllItemTypes(
      @NotNull BiFunction<String, JsonNode, T> itemTypeFactory, @NotNull Supplier<C> collectionFactory) { ... }
   ```
 * Cognitive Complexity / SonarQube; might streams help? -- calculate Cognitive Complexity for the 1st example [here](https://developer.ibm.com/articles/j-java-streams-1-brian-goetz/)
