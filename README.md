# Swagger 2

<h2>Swagger 2 in Spring Boot</h2>

Swagger 2 is an open source project used to describe and document RESTful APIs. It is language-agnostic and is extensible into new technologies and protocols beyond HTTP. The current version defines a set HTML, JavaScript, and CSS assets to dynamically generate documentation from a Swagger-compliant API. These files are bundled by the Swagger UI project to display the API on browser. Besides rendering documentation, Swagger UI allows other API developers or consumers to interact with the API’s resources without having any of the implementation logic in place.

The Swagger 2 specification, which is known as OpenAPI specification, has several implementations. Currently, Springfox, that has replaced Swagger-SpringMVC (Swagger 1.2 and older), is popular for Spring Boot applications. Springfox supports both Swagger 1.2 and 2.0.

<li>
<strong>Add following dependency in Maven POM</strong>
<img src="https://github.com/ShahbazHaroon/Swagger-2/blob/master/springfox.JPG" alt="springfox">
</li>

<li>
In addition to Springfox, we also require Swagger UI
<img src="https://github.com/ShahbazHaroon/Swagger-2/blob/master/Swagger-UI.JPG" alt="swaggerUI">
</li>

<h2>Configuring Swagger 2 in the Application</h2>

We need to create a Docket bean in a Spring Boot configuration to configure Swagger 2 for the application. A Springfox Docket instance provides the primary API configuration with sensible defaults and convenience methods for configuration

<strong>At this point, you should be able to test the configuration by starting the app and pointing your browser to</strong>

<li>http://localhost:8080/v2/api-docs</li>
<br/>

<p>The JSON dump, that Swagger 2 generates for our endpoints, is not something we want.
What we want is some nice human readable structured documentation, and this is where Swagger UI takes over</p>

On pointing your browser to
<li>http://localhost:8080/swagger-ui.html</li>
<br/>
you will see the generated documentation rendered by Swagger UI
