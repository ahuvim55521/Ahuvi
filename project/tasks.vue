    new vue({
       el: 'd',
       date: {
          tasks= localStorage.getItem("tesk")
       },
       methods:{
        add: function () {            
            tasks = (tasks) ? JSON.parse(tasks) : [];
            let userList = "";
            for(let singleUser of tasks) {
        
            userList += `<li>
            <ol style="date:${singleUser.dateO}">
            <li><h2>time: </h2> ${singleUser.timeO}</li>
            <li><h2>tesk: </h2> ${singleUser.teskO}</li>
            </ol>
            </li>`;
                } 
        }
       }
    })