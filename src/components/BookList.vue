        <template>

        <div>
            <h1>{{title}}</h1>
            <ul>
                <li v-for="book in books">{{book.title}}:{{book.author}}</li>
            </ul>

        </div>
            
        </template>
        
        <script>
        export default {
            name: 'BookList',
            data() {
                return {
                    title: 'All Books',
                    books: [
                    {title: 'Lord of the Rings', author: 'Tolkien'},
                    {title: 'Lord of the Flies', author: 'William Golding'},
                    {title: 'Lord of the Flies', author: 'William Golding'},
                    ]
                }
            }
        }
        </script>
        
        <style>
          h1, h2 {
              font-weight: normal
          }

          ul {
                list-style-type: none;
                padding: 0;

          }

        li {
            display: block;
            margin: 0 10px;
            }
        
        </style>



        