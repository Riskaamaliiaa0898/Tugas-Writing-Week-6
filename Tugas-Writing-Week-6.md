# REACT JS DASAR

> React JS adalah library JavaScript yang biasa digunakan saat membangun UI suatu website atau aplikasi web. React JS bisa dianggap seperti perpustakaan yang berisi berbagai kode JavaScript yang sudah tertulis (pre-written). Anda tinggal mengambil kode yang ingin Anda gunakan. Sehingga, ini membuat proses coding menjadi lebih efisien dengan framework JavaScript tersebut.

#### Kenapa kita harus menggunakan React JS

1. React JS is Fast => membuat aplikasi fornt-end menjadi lebih cepat walaupun menghandle banyak data.

2. React JS is Modular => membagi 1 tampilan web menjadi komponen-komponen kecil.

3. React JS is Scalable => dapat digunakan dalam aplikasi berskala kecil, besar hingga komplek.

4. React JS is Popular => komunitasnya sangat besar dan luas.

## Cara Menginstall React JS

### Windows Version

1. Download Node JS version >= 12 (Terbaru)

   https://nodejs.org/en/download

2. Install Node JS
3. Check Node

   **node --version**

4. Check NPM

   **npm --version**

5. Install Create React App Library

   **npm install -g create-react-app**

### Inisialisasi Proyek

1. Buka Terminal atau Command Prompt (CMD)
2. Lakukan perintah pada terminal yang telah dibuka :

   **npx create-react-app [name-project]**

   **Contoh :
   npx create-react-app example-project-1**

3. Install library react-router

   **npm install react-router@5.3.3**

#### Terdapat dua fitur tambahan yang menjadi keunggulannya react js:

1.  JSX => SX adalah extension syntax JavaScript yang memungkinkan Anda untuk memodifikasi Document Object Model (DOM) dengan kode bergaya HTML. setiap jsx memiliki 1 parent element.
2.  Virtual DOM => Virtual DOM berguna untuk melihat bagian dari DOM asli yang berubah.

## React JS - Component

> Komponen adalah salah satu core dari react JS, komponen membagi UL dalam satuan-satuan kecil artinaya dalam 1 page ada beberapa document yang bisa kita buat. Komponen React menggunakan sebuah method bernama render() yang menerima masukan data dan mengembalikan sesuatu untuk ditampilkan.

### Membuat Component

Ada 2 Cara membuat component :

1. Function
2. class

StateFul Component and Stateless Component

> Stateless component atau functional component adalah sebuah fungsi javascript yang hanya mengambil sebuah inputan, biasanya functional component ini digunakan untuk membungkus component kecil seperti component table, button dan lainnya. **Stateless Component** — tidak memiliki state hanya prop. Umumnya component ini di buat dengan function karena codenya lebih ringkas

Contoh penulisan stateless component atau functional component

      const HelloComponent () => {
         return <p>Hello Functional Component</p>
      }

> Stateful component digunakan untuk membungkus kode dari stateless component dengan cakupan yang lebih banyak dan besar. **Statefull Component** — memiliki state & props. Component ini dibuat dengan class. Kelebihan dari class component adalah memiliki lifecycle

Contoh penulisan Stateful component atau functional component

      class Hello extends React.Component {
         render() {
            return(
                  <div>
                     Hello Statefull Component
                  </div>
            )
            }
         }

### State And Props

Props

> Prop singkatan dari Property. Prop umumnya digunakan untuk komunikasi data component dari parent komponent ke child component.Prop itu read-only function ini hanya bisa membaca parameter props tetapi tidak bisa merubahnya.

State

> State adalah data private sebuah component. Data ini hanya tersedia untuk component tersebut dan tidak bisa di akses dari component lain. Component dapat merubah statenya sendiri.
