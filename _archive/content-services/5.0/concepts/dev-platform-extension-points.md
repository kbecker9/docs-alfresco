# Platform extension points

The Alfresco platform features a number of extension points that can be used to create customizations. The table of supported extension points includes links to more information.

The following table lists platform extension points and links to relevant documentation:

|Extension point|Description|Support Status|
|---------------|-----------|--------------|
|[Content Model](../references/dev-extension-points-content-model.md)|Content modeling provides a foundation for structuring and working with content. It is used to create a domain specific model that can be used to classify content and refine the search capabilities.|[Full Support](http://docs.alfresco.com/support/concepts/su-product-lifecycle.html)|
|[Data Lists](../references/dev-extension-points-data-lists.md)|Data lists are a useful feature available in sites. They can be used to keep records data. This is metadata that does not necessarily have any file content associated with it. It can be for example a to-do list or an event list.|[Full Support](http://docs.alfresco.com/support/concepts/su-product-lifecycle.html)|
|[Actions](../references/dev-extension-points-actions.md)|Actions are Spring beans that act upon a content node. You develop actions using Java and register them with the repository through a Spring configuration file. Actions provide a place to locate reusable business logic.|[Full Support](http://docs.alfresco.com/support/concepts/su-product-lifecycle.html)|
|[Workflow](../references/dev-extension-points-workflow.md)|Alfresco One embeds the Activiti Workflow Engine as standard. You can create custom business workflows to manage your content and processes.|[Full Support](http://docs.alfresco.com/support/concepts/su-product-lifecycle.html)|
|[Web scripts](../references/dev-extension-points-webscripts.md)|Web scripts provide the ability to create custom REST APIs. A web script is implemented in XML, JavaScript, and FreeMarker. Java can also be used to implement a web script if the business logic requires it. If written in JavaScript and FreeMarker it is possible to write new extensions that do not require a server restart to take effect.|[Full Support](http://docs.alfresco.com/support/concepts/su-product-lifecycle.html)|
|[JavaScript root objects](../references/dev-extension-points-javascript-root-objects.md)|The JavaScript root object collection provides a ready made set of objects you can access from your web scripts. These objects provide access to the repository content. It is also possible to extend the platform with new custom JavaScript root objects that can be used in for example Web Scripts controllers.|[Full Support](http://docs.alfresco.com/support/concepts/su-product-lifecycle.html)|
|[FreeMarker root objects](../references/dev-extension-points-freemarker-root-objects.md)|The FreeMarker root objects provide a collection of ready-made objects that you can work with from your FreeMarker code. These objects provides access to the Repository content. It is also possible to extend the platform with new custom FreeMarker root objects that can be used in for example Web Scripts templates.|[Full Support](http://docs.alfresco.com/support/concepts/su-product-lifecycle.html)|
|[Behaviors / policies](../references/dev-extension-points-behaviors.md)|Behaviors are logic that is tightly coupled to a repository event, such as adding content. Examples of out-of-the-box mechanisms that employ behaviors are versioning and auditing. Custom behaviors can be implemented to support features such as automatically adding a unique ID property to a content node when added to the repository, or automatically applying metadata attached to a folder to content stored in the folder.|[Full Support](http://docs.alfresco.com/support/concepts/su-product-lifecycle.html)|
|[Bootstrap content](../references/dev-extension-points-bootstrap.md)|Most content management solutions require some content to be available before the system is going live. This can be users, groups, files and folders, sites, and so on. This content can be imported into the repository using a bootstrapping procedure.|[Full Support](http://docs.alfresco.com/support/concepts/su-product-lifecycle.html)|
|[Permissions \(Custom Roles\)](../references/dev-extension-points-permissions.md)|Permissions and their groupings are defined in XML configuration files. The default files are found in the distribution configuration directory as permissionDefinitions.xml and sitePermissionDefinitions.xml. This configuration can be replaced or extended to create new roles.|[Full Support](http://docs.alfresco.com/support/concepts/su-product-lifecycle.html)|
|[MIME Types](../references/dev-extension-points-mimetypes.md)|Alfresco is able to automatically identify most file types and establish MIME type accordingly. However, if you have custom file types it is possible to add support for these by adding custom MIME types. You will typically also need to provide custom content transformations, and metadata extraction to fully support the content type.|[Full Support](http://docs.alfresco.com/support/concepts/su-product-lifecycle.html)|
|[Content Stores](../references/dev-extension-points-custom-content-store.md)|The repository has multiple content stores used for different purposes. By default, Alfresco is configured to save files or content items in the File Content Store. You can also have an encrypted content store, or a custom content store, depending on your requirements.|[Full Support](http://docs.alfresco.com/support/concepts/su-product-lifecycle.html)|
|[Audit Log](../references/dev-extension-points-audit.md)|The Audit service can be used to keep a record of all operations performed in the content repository. The audit information is stored in a database in a form that is designed to be simple for third-party reporting tools to consume. Custom audit applications can be configured.|[Full Support](http://docs.alfresco.com/support/concepts/su-product-lifecycle.html)|
|[Metadata Extractors](../references/dev-extension-points-custom-metadata-extractor.md)|Alfresco performs metadata extraction on content automatically, however, you may wish to create custom metadata extractors to handle custom file properties and custom content models.|[Full Support](http://docs.alfresco.com/support/concepts/su-product-lifecycle.html)|
|[Admin Console Component](../references/dev-extension-points-custom-admin-console.md)|The [Admin Console](at-adminconsole.md) provides a way of managing services integrated into Alfresco, or built on as extensions. Installed modules can have a custom Admin Console component, so that they can be managed from the well-known interface of the Admin Console.|[Full Support](http://docs.alfresco.com/support/concepts/su-product-lifecycle.html)|
|[Content Transformers \(and Renditions\)](../references/dev-extension-points-content-transformer.md)|Content transformers transform one type of content into another. Transformations can also be chained together. You can create custom content transformers to transform one type of content into another, where that transformation is not already supported. Closely related to transformations are renditions, which can be used to generate another version of the content, such as a preview, thumbnail, HTML etc.|[Full Support](http://docs.alfresco.com/support/concepts/su-product-lifecycle.html)|
|[Scheduled jobs](../references/dev-extension-points-scheduled-jobs.md)|Alfresco automatically runs a number of [scheduled jobs](scheduled-jobs.md), for example the content store cleaner job and temporary file cleaner job. It is possible to configure new scheduled jobs.|[Full Support](http://docs.alfresco.com/support/concepts/su-product-lifecycle.html)|
|[Authentication](../references/dev-extension-points-authentication.md)|Alfresco includes multiple authentication systems, including Active Directory, LDAP, Kerberos and so on, which you can opt to use. You can also create and plug in your own custom authentication system.|[Full Support](http://docs.alfresco.com/support/concepts/su-product-lifecycle.html)|
|[Subsystems](../references/dev-extension-points-custom-subsystem.md)|Implementing a customization as a subsystem allows a more fully decoupled customization. It is, for example, possible to disable the customization at run time.|[Full Support](http://docs.alfresco.com/support/concepts/su-product-lifecycle.html)|
|[Module Components](../references/dev-extension-points-module-component.md)|A Module Component executes code and is tied to a specific Module. It is packed with the rest of the module files in an AMP or JAR.|[Full Support](http://docs.alfresco.com/support/concepts/su-product-lifecycle.html)|
|[Ratings](../references/dev-extension-points-ratings.md)|A rating scheme is a defined system of ratings for content which is identified by a unique name and which provides a minimum and maximum allowed rating. There are out of the box ratings facilities, but as a developer you can also implement your own.|[Full Support](http://docs.alfresco.com/support/concepts/su-product-lifecycle.html)|
|[Form processors](../references/dev-extension-points-form-processors.md)|Custom Form Processor implementations can be implemented and integrated using a small amount of Spring configuration. Typically you will do this to support a new kind of form.|[Full Support](http://docs.alfresco.com/support/concepts/su-product-lifecycle.html)|
|[Form Filters](dev-extensions-share-form-filters.md)|Form filters can be used to modify the properties that are available to the form control implementation. They are often used to set up properties that should control some behaviour in a custom form control implementation.|[Full Support](http://docs.alfresco.com/support/concepts/su-product-lifecycle.html)|
|[Patch](../references/dev-extension-points-patch.md)|A patch executes a piece of Java code when Alfresco starts up, and logs the result in `ALF_APPLIED_PATCHES` database table.|[Full Support](http://docs.alfresco.com/support/concepts/su-product-lifecycle.html)|
