  new vue({
      el: 'all',
      date:{
           l ={ dateO: d.innerText, timeO: t.innerText, teskO: tk.innerText},
      },
      methods: {
           add: function () {
            localStorage.setItem("tesk", this.l);
             tk.innerText= "good";             
           }     
      }
  })