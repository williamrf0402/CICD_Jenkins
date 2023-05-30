pipeline
{
agent any
stages
{
    stage("Dias de la semana")
    {
        steps
        {
            
            script
            {
                def dia = new Date().getDay()
                def map = [1: "Lunes", 2: "Martes", 3: "Miercoles", 4:"Jueves", 5:"Viernes", 6:"Sabado", 7: "Domingo"]
                if(dia == 2) {
                    println "El usuario que inicio el trabajo es ${env.USER}"
                } else if(dia == 3) {
                    clima = "En estos momentos está nublado con una temperatura de 20 grados. Se esperan cielos parcialmente nublados desde media tarde. Hoy la temperatura máxima será de 20 grados y la mínima de 15 grados."
                    println clima
                } else if(dia == 4) {
                    git branch: "main", url: "https://github.com/williamrf0402/CICD_Jenkins.git"
                }
                
                
            }
        }
        
    }
}
    
}
