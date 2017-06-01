This package is still in development.  It is a client wrapper for Openx3 based heavily on the Openx3 Python Client.  This package relies on [github.com/sirupsen/logrus](github.com/sirupsen/logrus) and [github.com/mrjones/oauth](github.com/mrjones/oauth).

**This is still in development and test phase. This code and I have 0 officiations with Openx3.**


----------


At the moment this package can be installed via (subject to change):
**go get github.com/marcsantiago/OX3-Go-API-Client/openx**


----------

use 'godoc cmd/github.com/marcsantiago/OX3-Go-API-Client/openx' for documentation on the github.com/marcsantiago/OX3-Go-API-Client/openx command 

<!--
	Copyright 2009 The Go Authors. All rights reserved.
	Use of this source code is governed by a BSD-style
	license that can be found in the LICENSE file.
-->
<!--
	Note: Static (i.e., not template-generated) href and id
	attributes start with "pkg-" to make it impossible for
	them to conflict with generated attributes (some of which
	correspond to Go identifiers).
-->

	<script type='text/javascript'>
	document.ANALYSIS_DATA = ;
	document.CALLGRAPH = ;
	</script>

	
		
		<div id="short-nav">
			<dl>
			<dd><code>import "github.com/marcsantiago/OX3-Go-API-Client/openx"</code></dd>
			</dl>
			<dl>
			<dd><a href="#pkg-overview" class="overviewLink">Overview</a></dd>
			<dd><a href="#pkg-index" class="indexLink">Index</a></dd>
			
			
			</dl>
		</div>
		<!-- The package's Name is printed as title by the top-level template -->
		<div id="pkg-overview" class="toggleVisible">
			<div class="collapsed">
				<h2 class="toggleButton" title="Click to show Overview section">Overview ▹</h2>
			</div>
			<div class="expanded">
				<h2 class="toggleButton" title="Click to hide Overview section">Overview ▾</h2>
				
			</div>
		</div>
		

		<div id="pkg-index" class="toggleVisible">
		<div class="collapsed">
			<h2 class="toggleButton" title="Click to show Index section">Index ▹</h2>
		</div>
		<div class="expanded">
			<h2 class="toggleButton" title="Click to hide Index section">Index ▾</h2>

		<!-- Table of contents for API; must be named manual-nav to turn off auto nav. -->
			<div id="manual-nav">
			<dl>
			
			
			
			
				
				<dd><a href="#Client">type Client</a></dd>
				
					
					<dd>&nbsp; &nbsp; <a href="#NewClient">func NewClient(domain, realm, consumerKey, consumerSecrect, email, password string, debug bool) (*Client, error)</a></dd>
				
				
					
					<dd>&nbsp; &nbsp; <a href="#Client.Delete">func (c *Client) Delete(url string, data io.Reader) (res *http.Response, err error)</a></dd>
				
					
					<dd>&nbsp; &nbsp; <a href="#Client.Get">func (c *Client) Get(url string, urlParms map[string]interface{}) (res *http.Response, err error)</a></dd>
				
					
					<dd>&nbsp; &nbsp; <a href="#Client.LogOff">func (c *Client) LogOff() (res *http.Response, err error)</a></dd>
				
					
					<dd>&nbsp; &nbsp; <a href="#Client.Options">func (c *Client) Options(url string) (res *http.Response, err error)</a></dd>
				
					
					<dd>&nbsp; &nbsp; <a href="#Client.Post">func (c *Client) Post(url string, contentType string, data io.Reader) (res *http.Response, err error)</a></dd>
				
					
					<dd>&nbsp; &nbsp; <a href="#Client.PostForm">func (c *Client) PostForm(url string, data url.Values) (res *http.Response, err error)</a></dd>
				
					
					<dd>&nbsp; &nbsp; <a href="#Client.Put">func (c *Client) Put(url string, data io.Reader) (res *http.Response, err error)</a></dd>
				
			
			
			</dl>
			</div><!-- #manual-nav -->

		

		
			<h4>Package files</h4>
			<p>
			<span style="font-size:90%">
			
				<a href="/src/github.com/marcsantiago/OX3-Go-API-Client/openx/openx.go">openx.go</a>
			
			</span>
			</p>
		
		</div><!-- .expanded -->
		</div><!-- #pkg-index -->

		<div id="pkg-callgraph" class="toggle" style="display: none">
		<div class="collapsed">
			<h2 class="toggleButton" title="Click to show Internal Call Graph section">Internal call graph ▹</h2>
		</div> <!-- .expanded -->
		<div class="expanded">
			<h2 class="toggleButton" title="Click to hide Internal Call Graph section">Internal call graph ▾</h2>
			<p>
			  In the call graph viewer below, each node
			  is a function belonging to this package
			  and its children are the functions it
			  calls&mdash;perhaps dynamically.
			</p>
			<p>
			  The root nodes are the entry points of the
			  package: functions that may be called from
			  outside the package.
			  There may be non-exported or anonymous
			  functions among them if they are called
			  dynamically from another package.
			</p>
			<p>
			  Click a node to visit that function's source code.
			  From there you can visit its callers by
			  clicking its declaring <code>func</code>
			  token.
			</p>
			<p>
			  Functions may be omitted if they were
			  determined to be unreachable in the
			  particular programs or tests that were
			  analyzed.
			</p>
			<!-- Zero means show all package entry points. -->
			<ul style="margin-left: 0.5in" id="callgraph-0" class="treeview"></ul>
		</div>
		</div> <!-- #pkg-callgraph -->

		
		
		
		
			
			
			<h2 id="Client">type <a href="/src/target/openx.go?s=737:1002#L23">Client</a>
				<a class="permalink" href="#Client">&#xb6;</a>
			</h2>
			<p>
Client holds all the user information, all of it is private however and
as a result only the defined methods below are used to interact with the data
</p>

			<pre>type Client struct {
    <span class="comment">// contains filtered or unexported fields</span>
}</pre>

			

			

			
			
			

			
				
				<h3 id="NewClient">func <a href="/src/target/openx.go?s=5395:5507#L178">NewClient</a>
					<a class="permalink" href="#NewClient">&#xb6;</a>
				</h3>
				<pre>func NewClient(domain, realm, consumerKey, consumerSecrect, email, password <a href="/pkg/builtin/#string">string</a>, debug <a href="/pkg/builtin/#bool">bool</a>) (*<a href="#Client">Client</a>, <a href="/pkg/builtin/#error">error</a>)</pre>
				<p>
NewClient creates the basic Openx3 *Client via oauth1
</p>

				
				
			

			
				
				<h3 id="Client.Delete">func (*Client) <a href="/src/target/openx.go?s=1893:1976#L65">Delete</a>
					<a class="permalink" href="#Client.Delete">&#xb6;</a>
				</h3>
				<pre>func (c *<a href="#Client">Client</a>) Delete(url <a href="/pkg/builtin/#string">string</a>, data <a href="/pkg/io/">io</a>.<a href="/pkg/io/#Reader">Reader</a>) (res *<a href="/pkg/net/http/">http</a>.<a href="/pkg/net/http/#Response">Response</a>, err <a href="/pkg/builtin/#error">error</a>)</pre>
				<p>
Delete creates a delete request which the Openx3 API uses, but that is not defined by Go
</p>

				
				
				
			
				
				<h3 id="Client.Get">func (*Client) <a href="/src/target/openx.go?s=1147:1244#L38">Get</a>
					<a class="permalink" href="#Client.Get">&#xb6;</a>
				</h3>
				<pre>func (c *<a href="#Client">Client</a>) Get(url <a href="/pkg/builtin/#string">string</a>, urlParms map[<a href="/pkg/builtin/#string">string</a>]interface{}) (res *<a href="/pkg/net/http/">http</a>.<a href="/pkg/net/http/#Response">Response</a>, err <a href="/pkg/builtin/#error">error</a>)</pre>
				<p>
Get is simailiar to the normal Go *http.Client.Get
except string parameters can be pass in in the url or the as a map[string]interface{}
</p>

				
				
				
			
				
				<h3 id="Client.LogOff">func (*Client) <a href="/src/target/openx.go?s=3367:3424#L107">LogOff</a>
					<a class="permalink" href="#Client.LogOff">&#xb6;</a>
				</h3>
				<pre>func (c *<a href="#Client">Client</a>) LogOff() (res *<a href="/pkg/net/http/">http</a>.<a href="/pkg/net/http/#Response">Response</a>, err <a href="/pkg/builtin/#error">error</a>)</pre>
				<p>
LogOff sets the created session to an empty http.Client, destorying the stored cookie
</p>

				
				
				
			
				
				<h3 id="Client.Options">func (*Client) <a href="/src/target/openx.go?s=2261:2329#L75">Options</a>
					<a class="permalink" href="#Client.Options">&#xb6;</a>
				</h3>
				<pre>func (c *<a href="#Client">Client</a>) Options(url <a href="/pkg/builtin/#string">string</a>) (res *<a href="/pkg/net/http/">http</a>.<a href="/pkg/net/http/#Response">Response</a>, err <a href="/pkg/builtin/#error">error</a>)</pre>
				<p>
Options is a wrapper for a GET request that has the /options endpoint already passed in
</p>

				
				
				
			
				
				<h3 id="Client.Post">func (*Client) <a href="/src/target/openx.go?s=2877:2978#L94">Post</a>
					<a class="permalink" href="#Client.Post">&#xb6;</a>
				</h3>
				<pre>func (c *<a href="#Client">Client</a>) Post(url <a href="/pkg/builtin/#string">string</a>, contentType <a href="/pkg/builtin/#string">string</a>, data <a href="/pkg/io/">io</a>.<a href="/pkg/io/#Reader">Reader</a>) (res *<a href="/pkg/net/http/">http</a>.<a href="/pkg/net/http/#Response">Response</a>, err <a href="/pkg/builtin/#error">error</a>)</pre>
				<p>
Post is a wrapper for the basic Go *http.Client.Post
</p>

				
				
				
			
				
				<h3 id="Client.PostForm">func (*Client) <a href="/src/target/openx.go?s=3122:3208#L101">PostForm</a>
					<a class="permalink" href="#Client.PostForm">&#xb6;</a>
				</h3>
				<pre>func (c *<a href="#Client">Client</a>) PostForm(url <a href="/pkg/builtin/#string">string</a>, data <a href="/pkg/net/url/">url</a>.<a href="/pkg/net/url/#Values">Values</a>) (res *<a href="/pkg/net/http/">http</a>.<a href="/pkg/net/http/#Response">Response</a>, err <a href="/pkg/builtin/#error">error</a>)</pre>
				<p>
PostForm is a wrapper for the basic Go *http.Client.PostForm
</p>

				
				
				
			
				
				<h3 id="Client.Put">func (*Client) <a href="/src/target/openx.go?s=2553:2633#L84">Put</a>
					<a class="permalink" href="#Client.Put">&#xb6;</a>
				</h3>
				<pre>func (c *<a href="#Client">Client</a>) Put(url <a href="/pkg/builtin/#string">string</a>, data <a href="/pkg/io/">io</a>.<a href="/pkg/io/#Reader">Reader</a>) (res *<a href="/pkg/net/http/">http</a>.<a href="/pkg/net/http/#Response">Response</a>, err <a href="/pkg/builtin/#error">error</a>)</pre>
				<p>
Put creates a put request which the Openx3 API uses, but that is not defined by Go
</p>