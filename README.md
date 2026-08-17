# Rotas.html
‹!DOCTYPE html>

<title>Sistema de Rotas de Transporte</title> <style> *{ margin: 0; padding:0; box-sizing border-box: tont-family: Anal: body! background:#eef3f7: header! background:#1565C0; color: white; padding:20px; text-align.center; .containerf width: 95%; max-width: 1200px; margin: auto; margin-top:20px; •card‹ background: white; padding:20px; border-radius: 10px; box-shadow:Opx 2px 10px gba(0,0,0, 2); . griak display: grid; grid-template-columns:repeat(auto-fit, minmax(250px, 1 fr)); дар: 15px; labek font-weight:bold; display: block; margem superior: 10px; input( width: 100%; padding: 10px; border: 1px solid #ccc; border-radius:5px; } button padding: 12px; border:none; border-radius:5px; cursor: pointer; font-size: 15px; } .salvari background:#2E7D32; color: white; editart background #FB8C00; color:white; } excluir{ background:#C62828; color:white; table width: 100%; margin-top:20px; border-collapse: collapse, thị background:#1565C0; color white; padding: 10px; ta{ padding: 10px; border-bottom: 1px solid #ddd; } tr.hover{ background:#f5f5f5; #pesquisai margin-bottom:20px; </style> Sistema de Rotas de Transporte
<div class="grid">
‹label>Girar
<div> Motorista
< div> Veículo sinput id="veiculo">
<div><label>Saída ‹input type="time" id="hora">
Parada 1
Parada 2
Parada 3
<|abel>Destino ‹input id="destino">

Salvar Rota
‹div class="card"> sinput id="pesquisa" placeholder="Pesquisar..' onkeyup="'istar)">
Rota	Motorista	Veículo	Horário	Percurso	Ações
<script> let rotas = JSON.parse(localStorage.getElementByld("rotas")) || []; let editarlndice = -1; function salvar(){ let rota=document.getElementByld("rota").value; let motorista=document.getElementByld("motorista").value; let veiculo=document.getElementByld('veiculo").value; „t nora=document.getElementByld("hora") value; et p1=document.getElementByld("p1") value; iet p2=document.getElementByld('p2") value; let p3=document.getElementByld("p3"), value: let destino=document.getElementByld "destino) value; let dados={ rota, motorista, veiculo,hora,p1 ,p2,p3,destino }; if(editarlndice==-1X rotas.push(dados); Jelse{ rotas[editarIndicel=dados; editarlndice=-1; } localStorage.setltem('rotas", ,JSON.stringify(rotas)); limpar(); listar(); function listar() let=document.getElementByld("pesquisa"). value.toLowerCase(); let tabela=document.getElementByld("tabela); tabela.innerHTML=™️''; busca=(r.rota+r.motorista+r.veiculo+r.destino). toLowerCase(); if(busca.includes(texto)x tabela.innerHTML+=* ${r.rota} ${r.motorista} ${r. veiculo) $(r.hora} S(r.p1) → S(r.p2) → $(r.p3) → s(r.destino) button class="editar" onclick="editar($(1)"> Editar ‹button class="excluir" onclick="excluir($(i)">Excluir aterAll("inpu }); function editar(i){ let r=rotas[]; document.getElementByld("rota"). value=r.rota; document.getElementByld("motorista"). value=r.motorista; document.getElementByld ("veiculo"). value=r.veiculo; document.getElementByld ("hora"). value=r.hora; document.getElementByld("p1").value=r.p1; document.getElementByld("p2").value=r.p2; document.getElementByld("p3").value=r.p3; document.getElementByld("destino").value=r.destino; editarlndice=i; } function excluir(i) if(confirm("Excluir rota?")! rotas.splice (i,1); localStorage.setltem("rotas", JSON.stringify(rotas)); listar(); function limpark document.query SelectorAll ("input").forEach(c=>{ if(c.type!="search") c.value''; }); listar();
  </script>
 </body>
 </HTML>
 
