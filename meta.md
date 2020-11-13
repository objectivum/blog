# blog

## Theme

 * Programming font
   - https://www.recursive.design/ (not only for programming)
   - `JetBrains Mono`, `Fira Code`, `Cascadia`, `Dank Mono`, `IBM Plex Mono`, `Input Mono`, `Inconsolata`, `Victor Mono`, `NotCourier`
   - https://itnext.io/11-best-programming-fonts-724283a9ed57
   - https://github.com/ryanoasis/nerd-fonts
   - https://input.fontbureau.com/
 * General style
   - martinFowler.com (e.g. https://martinfowler.com/articles/replaceThrowWithNotification.html)
   - https://kevinsmith.io/
   - https://diveintopython3.problemsolving.io/
   - https://jrsinclair.com/
   - http://modernperlbooks.com/books/modern_perl_2016/index.html
   - https://fonts.google.com/specimen/Proza+Libre; Muli; Work Sans?
   - https://fonts.google.com/specimen/Karla
   - https://fontpair.co/

## Content (ideas)

 * Section: (code) snippets
   * ifPresent() on Dto, etc.; usefulness: set `boolean` from `Boolean` i.e., primitive from wrapper
     ```java
       public class Converters {

         public static <V> void ifPresent(Supplier<? extends V> supplier, Consumer<? super V> consumer) {
           final V value = supplier.get();
           if (present(value)) {
             consumer.accept(value);
           }
         }

         public static <FROM, TO> void ifPresent(Supplier<? extends FROM> supplier,
                                                 Function<? super FROM, ? extends TO> mapper, Consumer<TO> consumer) {
           final FROM from = supplier.get();
           final TO to = present(from) ? mapper.apply(from) : null;
           if (present(to)) {
             consumer.accept(to);
           }
         }

         private static boolean present(Object o) {
           return (o instanceof Map && !((Map<?, ?>) o).isEmpty()) ||
                  (o instanceof Collection && !((Collection<?>) o).isEmpty()) ||
                  (o instanceof CharSequence && ((CharSequence) o).length() > 0) || o != null;
         }
       }
     ```
 * Git rebase OR merge
   * [Why you should stop using Git rebase](https://medium.com/@fredrikmorken/why-you-should-stop-using-git-rebase-5552bee4fed1)
   * [Merge `master` into `development` first, as alternative](https://stackoverflow.com/questions/14168677/merge-development-branch-with-master)

Grammar rules
- Which person? (1st, 3rd, sg, pl)
- Which writing style?

Categorizing blog entries

Inspiration
- Baeldung
- Nicolas Frankel
- Marco Behler
- Pascal Precht

Tools to use

Process to use

Automate notifications/posting to social media
