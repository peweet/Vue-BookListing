        <template>

        <div>
            <h1>{{title}}</h1>
            <ul>

                <li v-for="book in books">{{books.title}}:{{books.author}}</li>

            </ul>

        </div>
            
        </template>
        
        <script>
        export default {
            name: 'Booklist',
            data() {
                return {
                    title: 'All Books',
                    books: [
                    {title:'Lord of the Rings', author: 'Tolkien'},
                    {title:'Lord of the Flies', author: 'William Golding'},
                    {title:'Lord of the Flies', author: 'William Golding'}
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



        