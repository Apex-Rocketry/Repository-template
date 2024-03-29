# Repositório Template

### __O seguinte exemplo é um modelo para um repositório que possui três pilares__
* __PCB design__ (arquivos de esquemáticos e PCB [Altium])
* __Software__ (arquivos de texto)
* __Hardware__ (modelos 3D etc.)

### __A divisão do repositório será a seguinte:__
* __Master__ Ramo mestre básico usado com Dev_Software
* __Dev_Software__ Ramo normal criado a partir do commit inicial do Master, usado para arquivos de software
* __Dev_Hardware__ Ramo órfão usado para modelos 3D, desenhos e arquivos de saída.
* __Dev_PCB__ Ramo órfão usado para arquivos Alitum (arquivos de esquema/PCB/projetos)

Em cada ramo deste modelo, há um readme com mais detalhes

### __Como criar um ramo órfão__
    git checkout --orphan nome_orfao
    git rm -rf .
    rm '.gitignore'
    echo "#Título do Readme" > README.md
    git add README.md
    git commit -a -m "Commit Inicial"
    git push origin nome_orfao
    
![](print.png)

Para mais informações sobre Git [clique aqui](https://github.com/Apex-Rocketry/git-flight-rules)
