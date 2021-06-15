pipeline {
   agent any

   stages {
       stage ('Nuget Restore') {
         steps {
          bat '"C:\\nuget\\nuget.exe" restore ".\\alac\\alac.sln"'
         }
      }
      
      stage ('Build') {
         steps {
          bat '"C:\\Program Files (x86)\\Microsoft Visual Studio\\2019\\BuildTools\\MSBuild\\Current\\Bin\\msbuild.exe" ".\\alac\\alac.sln" /property:Configuration=Release /p:OutputPath="C:\\release\\alac"'
         }
      }
     
      }
   }
}
