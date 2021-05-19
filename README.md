# frontend-patterns

https://www.adictosaltrabajo.com/2019/02/14/patrones-de-diseno-en-el-frontend/

<div class="td-post-featured-image"></div>
        <p>El mundo frontend es conocido por su gran <em>volatilidad</em>, sin embargo poco hacemos para que esta volatilidad no afecte a nuestros desarrollos. Nos importa últimamente estar más <strong>a la última del framework del momento que aprender a hacer nuestro código más mantenible</strong>. Así que este tutorial irá en pos de hacer una aplicación lo más <em>«Frameworkless»</em> posible.</p>
<p><!-- more --></p>
<h2><a href="" name="-ndice"></a><br />
Índice</h2>
<ul>
<li><a href="https://www.adictosaltrabajo.com/2019/02/14/patrones-de-diseno-en-el-frontend/#problema">Problema</a></li>
<li><a href="https://www.adictosaltrabajo.com/2019/02/14/patrones-de-diseno-en-el-frontend/#soluci%C3%B3n">Solución</a>
<ul>
<li><a href="https://www.adictosaltrabajo.com/2019/02/14/patrones-de-diseno-en-el-frontend/#chain-of-responsibility">Chain of responsibility</a></li>
<li><a href="https://www.adictosaltrabajo.com/2019/02/14/patrones-de-diseno-en-el-frontend/#proxy">Proxy</a></li>
<li><a href="https://www.adictosaltrabajo.com/2019/02/14/patrones-de-diseno-en-el-frontend/#observador">Observador</a></li>
</ul>
</li>
<li><a href="https://www.adictosaltrabajo.com/2019/02/14/patrones-de-diseno-en-el-frontend/#singleton">Singleton</a></li>
<li><a href="https://www.adictosaltrabajo.com/2019/02/14/patrones-de-diseno-en-el-frontend/#react">React</a>
<ul>
<li><a href="https://www.adictosaltrabajo.com/2019/02/14/patrones-de-diseno-en-el-frontend/#context">Context</a></li>
<li><a href="https://www.adictosaltrabajo.com/2019/02/14/patrones-de-diseno-en-el-frontend/#observadores">Observadores</a></li>
</ul>
</li>
<li><a href="https://www.adictosaltrabajo.com/2019/02/14/patrones-de-diseno-en-el-frontend/#nueva-feature">Nueva feature</a></li>
<li><a href="https://www.adictosaltrabajo.com/2019/02/14/patrones-de-diseno-en-el-frontend/#conclusi%C3%B3n">Conclusión</a></li>
</ul>

<a href="https://www.adictosaltrabajo.com/wp-content/uploads/2019/01/samuel-zeller-34751-unsplash.jpg" data-caption=""><img width="1068" height="712" class="entry-thumb td-modal-image" src="https://www.adictosaltrabajo.com/wp-content/uploads/2019/01/samuel-zeller-34751-unsplash-1068x712.jpg" srcset="https://www.adictosaltrabajo.com/wp-content/uploads/2019/01/samuel-zeller-34751-unsplash-1068x712.jpg 1068w, https://www.adictosaltrabajo.com/wp-content/uploads/2019/01/samuel-zeller-34751-unsplash-150x100.jpg 150w, https://www.adictosaltrabajo.com/wp-content/uploads/2019/01/samuel-zeller-34751-unsplash-300x200.jpg 300w, https://www.adictosaltrabajo.com/wp-content/uploads/2019/01/samuel-zeller-34751-unsplash-768x512.jpg 768w, https://www.adictosaltrabajo.com/wp-content/uploads/2019/01/samuel-zeller-34751-unsplash-1024x683.jpg 1024w, https://www.adictosaltrabajo.com/wp-content/uploads/2019/01/samuel-zeller-34751-unsplash-696x464.jpg 696w, https://www.adictosaltrabajo.com/wp-content/uploads/2019/01/samuel-zeller-34751-unsplash-630x420.jpg 630w, https://www.adictosaltrabajo.com/wp-content/uploads/2019/01/samuel-zeller-34751-unsplash-1920x1280.jpg 1920w" sizes="(max-width: 1068px) 100vw, 1068px" alt="" title="samuel-zeller-34751-unsplash"/></a>
