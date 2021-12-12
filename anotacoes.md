<body>
    <h1>Anotações - Módulo 01</h1>
    <h1>TAGs</h1>
    <p>! → Indicar que o documento é um HTML</p>
    <p>&lt;h1&gt; → Título 01</p>
    <p>&lt;hr&gt; → Linha horizontal</p>
    <p>&lt;p&gt; → Parágrafo</p>
    <p>&lt;br&gt; → Quebra de linha</p>
    <p>&#x + → Escolher emoji na <a href="https://emojipedia.org/">Emojipedia</a></p>
    <p>&lt;h1&gt; → Título 01</p>
    <p>link:favicon → Favicon</p>
    <p>strong → <strong>Negrito</strong>
    <p>em → <em>Itálico</em></p>
    <p>mark → <mark>Marca-texto</mark></p>
    <p>small → <smalll>Letra pequena</smalll></p>
    <p>del → <del>Texto taxado / excluido</del></p>
    <p>ins → <ins>Texto sublinhado</ins></p>
    <p>sup → Texto sobrescrito → X<sup>2</sup></p>
    <p>sub → Texto subscrito → H<sub>2</sub>O</p>
    <p>code → <code>Fonte para código</code></p>
    <p>pre → Escrever com identação</p>
    <p>q → <q>Aspas</q></p>
    <p>blockquote → <blockquote>Citação</blockquote></p>
    <p>abbr → <abbr title="Use esta TAG para abreviações">Abreviação</abbr></p>
    <p>bdo dir="rtr" → Texto invertido → <bdo dir="rtl">Texto invertido</bdo></p>
    <p>ol → Lista ordenada</p>
    <p>ul → Lista não ordenada</p>
    <p>li → Listar</p>
    <h1>Links</h1>
    <p>link interno ou externo → a</p>
    <p>target="_blank" → Abrir link em uma nova aba</p>
    <p>rel="external" → Referência externa</p>
    <p>../ → Voltar para pasta anterior</p>
    <h1>Simbolos</h1>
    <p>Para escrever simbolos no código como &lt;, &gt;, &amp;, &cent;... Pesquisar por <a href="https://www.w3schools.com/html/html_entities.asp">HTML Entities</a>. </p>
    <h1>Imagens</h1>
    <p>JPEG → Mais leve</p>
    <p>PNG → Transparência</p>
    <p>GIF → Transparência + Animação</p>
    <h1>Atalhos do Visual Code</h1>
    <p>ctrl+shift+P → Insere a TAG no texto selecionado</p>
    <ul>
        <li>Para configurar precisa ir em pesquisar e procurar por Emmet: <em>Wrap With Abbreviation</em></li>
    <p>Word Wrap → Para quebra de linha automática</p>
    </ul>
    <h1>Imagens Dinâmicas</h1>
    <p>&lt;picture&gt; → Para informar o espaçõ de imagem</p>
    <p>Source Media Yype → Para informar os tipos e tamanhos de imagenss</p>
    <p>As mídias precisam ser inseridas em ordem, da menor para a maior, sendo que a maior (padrão) ficará na Tag principal &lt;img&gt;</p>
    <p>Então o código ficará assim:</p>
    <pre>
        <code>
    &lt;picture&gt;
        &lt;source media="(max-width: 750px)" srcset="imagens/foto-p.jpg" type="image/jpg"&gt;
        &lt;source media="(max-width: 1050px)" srcset="imagens/foto-m.jpg" type="image/jpg"&gt;
        &lt;img src="imagens/foto-g.jpg" alt="Imagem flexível"&gt;
    &lt;/picture&gt;
        </code>
    </pre>
    <h1>Áudios</h1>
    <p>&lt;audio&gt; → TAG para inserção de um arquivo direto</p>
    <p>controls → Inserir ao lado e dentro da TAG audio para exibir o player dentro do site</p>
    <p>source:src → Para a inserção de várias extensões de audio para maior compatibilidade de navegadores</p>
    <h2>Exemplos:</h2>
    <h3>Para inserção de um áudio</h3>
<pre>
<code>
    &lt;audio src="midia/Calvin Harris - josh pan.mp3" controls &gt;&lt;/audio&gt;
</code>
</pre>
    <h3>Para inserção de várias extenções</h3>
<pre>
<code>
    &lt;audio preload="metadata" controls&gt;
        &lt;source src="midia/Calvin Harris - josh pan.mp3" type="audio/mpeg"&gt;
        &lt;source src="midia/manchetes.wav" type="audio/wave"&gt;
    &lt;/audio&gt;
</code>
</pre>
    <h1>Vídeos</h1>
    <p>Conversor de vídeos: <a href="https://handbrake.fr/">HandBrack</a></p>
    <p>&lt;video&gt; → Título 01</p>
    <p>controls → Inserir ao lado e dentro da TAG video para exibir o player dentro do site</p>
    <p>source:src → Para a inserção de várias extensões de vídeo para maior compatibilidade de navegadores</p>
    <p>poster → Para inserir a Thumb no vídeo</p>
    <p>width → Para definir o tamanho do vídeo na página</p>

    <h2>Exemplos:</h2>
    <h3>Para inserção de um único vídeo - Servidor próprio</h3>
<pre>
<code>
    &lt;video poster="imagens/thumb.png" controls src="media/pexels-artem-podrez-7233556.mp4" width="560"&gt;&lt;/video&gt;
</code>
</pre>
<h3>Para inserção de várias extensões de vídeos - Servidor próprio</h3>
<pre>
    <code>
    &lt;video width="560" poster="imagens/thumb.png" controls&gt;
    &lt;source src="media/pexels-artem-podrez-7233556.mp4" type="video/mp4"&gt;
    &lt;source src="media/pexels-artem-podrez-7233556.mp4" type="video/webm"&gt;
    &lt;source src="media/pexels-artem-podrez-7233556.mp4" type="video/ogg"&gt;
    &lt;/video&gt;
    </code>
</pre>
    <h1>CSS</h1>
    <h2>Páginas Únicas</h2>
    <p>Para incluir os estilos CSS o ideal - para páginas únicas - é inserir a tag logo abaixo do título, antes de fechar a seção head</p>
    <p>A tag é aberta com &lt;style&gt; e abaixo dela é declarado o nome da seção e é aberta uma chave {, com isso começamos a digitar os valores dos estilos, como por exemplo:</p>
    <pre>
    <code>
    &lt;style&gt;
    body&lcub;
        background-color&colon; darkturquoise;
        font-family&colon; sans-serif&semi;
        font-size&colon; 20px&semi;
    &rcub;
    h1&lcub;
        color&colon; dodgerblue;
        background-color&colon; ghostwhite&semi;
    &rcub;
    h2&lcub;
        color&colon; forestgreen&semi;
    &rcub;
    p&lcub;
        text-align&colon; justify&semi;
    &rcub;
    &lt;/style&gt;
    </code>
    </pre>
    <h2>Várias Páginas</h2>
    Usar a tag <strong>link:css</strong>, clicar em cima do link de página criado e criar uma nova página com base nele. A tag ficará assim
    <pre>
        <code>
    &lt;link rel="stylesheet" href="style.css"&gt;
        </code>
    </pre>
    <p>Com isso já podemos inserir os estilos dentro da folha de estilos e ela passará a valer para todas as páginas que contenham a referência.</p>
    <p>Para mexer nas configurações globais do arquivo, é utilizado a tag asterisco *.</p>
    <p>Para mexer no corpo do arquivo é usada a tag body dentro da sessão head.</p>
    <p>Toda a tag em css é seguida de chave <strong>{</strong></p>
    <h2>Cores Gradientes</h2>
    <p>Para usar as cores com gradientes no CSS é usada a tag <q>background-image: linear-gradient</q>, em seguida é dada a direção que o gradiente terá, como por exemplo <q>to bottom</q> para ir para o final da página, e em seguida são indicadas as cores, separadas por virula, sem limite de cores.</p>
    <p>Exemplo de um fundo transparente para o corpo da página:</p>
    <pre>
<code>
    body{
        background-image: linear-gradient(to bottom, #F24495, #181926);
        background-attachment: fixed;
    }
</code>
    </pre>

<h2>Fontes em CSS</h2>
<p>Para alterar a fonte no arquivo CSS é usado o comando font-family e selecionada a família de fontes que mais combina com o projeto.</p>
<p>Caso tenha dúvida sobre as fontes que combinam entre si, é possível consultar o CSS Web Safe Font</p>
<p>Ou ainda, utilizar após digitar o comando font-family: as teclas ctrl+espaço para que o VS Code sugira algumas famílias de fonte, como no exemplo abaixo</p>

<pre>
<code>
    body{
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
        }
</code>
</pre>

<p>No exemplo a família utilizada é a -apple-system
</body>