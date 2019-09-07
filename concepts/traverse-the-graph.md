---
title: Acessar dados e métodos ao navegar no Microsoft Graph
description: Além de usar a API do Microsoft Graph para ler e gravar dados, você pode usar diversos padrões de solicitação para desviar pelos recursos no Microsoft Graph. O documento de metadados também ajuda a entender o modelo de dados dos recursos e das relações no Microsoft Graph.
localization_priority: Priority
scenarios: getting-started
ms.openlocfilehash: 581efe1b14bb156b3ac53a6a06bf731f11150cb0
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/07/2019
ms.locfileid: "36791040"
---
# <a name="access-data-and-methods-by-navigating-microsoft-graph"></a><span data-ttu-id="7512c-104">Acessar dados e métodos ao navegar no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7512c-104">Access data and methods by navigating Microsoft Graph</span></span>

<span data-ttu-id="7512c-p102">Além de usar a API do Microsoft Graph para ler e gravar dados, você pode usar diversos padrões de solicitação para desviar pelos recursos no Microsoft Graph. O documento de metadados também ajuda a entender o modelo de dados dos recursos e das relações no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7512c-p102">In addition to using the Microsoft Graph API to read and write data, you can use a number of request patterns to traverse through the resources in Microsoft Graph. The metadata document also helps you to understand the data model of the resources and relationships in Microsoft Graph.</span></span>

## <a name="microsoft-graph-api-metadata"></a><span data-ttu-id="7512c-107">Metadados da API do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7512c-107">Microsoft Graph API metadata</span></span>

<span data-ttu-id="7512c-p103">O documento de metadados ($metadata) é publicado na raiz do serviço. Você pode exibir o documento de serviço das versões 1.0 e beta da API Microsoft Graph com as URLs a seguir.</span><span class="sxs-lookup"><span data-stu-id="7512c-p103">The metadata document ($metadata) is published at the service root. You can view the service document for the v1.0 and beta versions of the Microsoft Graph API via the following URLs.</span></span>

<span data-ttu-id="7512c-110">**Metadados 1.0 da API do Microsoft Graph**</span><span class="sxs-lookup"><span data-stu-id="7512c-110">**Microsoft Graph API v1.0 metadata**</span></span>
```
    https://graph.microsoft.com/v1.0/$metadata
```

<span data-ttu-id="7512c-111">**Metadados beta da API do Microsoft Graph**</span><span class="sxs-lookup"><span data-stu-id="7512c-111">**Microsoft Graph API beta metadata**</span></span>

```
    https://graph.microsoft.com/beta/$metadata
```

<span data-ttu-id="7512c-112">Com os metadados, você pode exibir e entender o modelo de dados do Microsoft Graph, inclusive os tipos de entidade, os tipos complexos e as enumerações que compõem os recursos representados nos pacotes de solicitação e resposta.</span><span class="sxs-lookup"><span data-stu-id="7512c-112">The metadata allows you to see and understand the Microsoft Graph data model, including the entity types, complex types, and enumerations that make up the resources represented in the request and response packets.</span></span>

<span data-ttu-id="7512c-113">Você pode usar os metadados para compreender as relações entre entidades no Microsoft Graph e estabelecer URLs que navegam entre essas entidades.</span><span class="sxs-lookup"><span data-stu-id="7512c-113">You can use the metadata to learn the realtionships between entities in Microsoft Graph and establish URLs that navigate between those entities.</span></span>

> [!NOTE]
> - <span data-ttu-id="7512c-114">Use as IDs de recurso no mesmo caso de serem retornadas das APIs do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7512c-114">Use resource IDs in the same case as they are returned from Microsoft Graph APIs.</span></span>
> - <span data-ttu-id="7512c-115">Presuma as IDs de recurso, os valores atribuídos e outros valores Codificados em Base 64 _diferenciam maiúsculas de minúsculas_.</span><span class="sxs-lookup"><span data-stu-id="7512c-115">Assume resource IDs, values you assign, and other base-64-encoded values are _case-sensitive_.</span></span>
> - <span data-ttu-id="7512c-116">Os nomes de recursos, parâmetros de consulta, parâmetros de ação e valores da URL do caminho _não diferenciam maiúsculas de minúsculas_.</span><span class="sxs-lookup"><span data-stu-id="7512c-116">The path URL resource names, query parameters, and action parameters and values are case insensitive.</span></span>

## <a name="view-a-collection-of-resources"></a><span data-ttu-id="7512c-117">Exibir uma coleção de recursos</span><span class="sxs-lookup"><span data-stu-id="7512c-117">View a collection of resources</span></span>

<span data-ttu-id="7512c-118">O Microsoft Graph permite exibir recursos em um locatário usando consultas HTTP `GET`.</span><span class="sxs-lookup"><span data-stu-id="7512c-118">Microsoft Graph lets you view resources in a tenant using HTTP `GET` queries.</span></span> <span data-ttu-id="7512c-119">A resposta de consulta inclui as propriedades de cada recurso.</span><span class="sxs-lookup"><span data-stu-id="7512c-119">The query response includes properties of each resource.</span></span> <span data-ttu-id="7512c-120">Os recursos de entidade são todos identificados pela sua ID.</span><span class="sxs-lookup"><span data-stu-id="7512c-120">Entity resources are each identified by its ID.</span></span> <span data-ttu-id="7512c-121">O formato da ID do recurso pode ser um GUID e normalmente varia de acordo com o tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="7512c-121">The format of a resource ID can be a GUID, and generally varies according to the resource type.</span></span>

<span data-ttu-id="7512c-122">Por exemplo, você pode obter uma coleção de recursos de [user](/graph/api/resources/user?view=graph-rest-1.0) definida no locatário:</span><span class="sxs-lookup"><span data-stu-id="7512c-122">For example, you can get the collection of users defined in a tenant:</span></span>

```no-highlight
GET https://graph.microsoft.com/v1.0/users HTTP/1.1
Authorization : Bearer {access_token}
```

<span data-ttu-id="7512c-p105">Se tiver êxito, você receberá uma resposta 200 OK que contém a coleção de recursos **user** no payload. Cada usuário será identificado pela propriedade **id** e acompanhado pelas respectivas propriedades padrão. O payload exibido abaixo foi truncado por uma questão de resumo.</span><span class="sxs-lookup"><span data-stu-id="7512c-p105">If successful, you'll get a 200 OK response that contains the collection of **user** resources in the payload. Each user is identified by the **id** property and accompanied by its default properties. The payload shown below is truncated for brevity.</span></span>

```no-highlight
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "value":[
    {
      "id":"f71f1f74-bf1f-4e6b-b266-c777ea76e2c7",
      "businessPhones":[

      ],
      "displayName":"CIE Administrator",
      "givenName":"CIE",
      "jobTitle":null,
      "mail":"admin@contoso.onmicrosoft.com",
      "mobilePhone":"+1 3528700812",
      "officeLocation":null,
      "preferredLanguage":"en-US",
      "surname":"Administrator",
      "userPrincipalName":"admin@contoso.onmicrosoft.com"
    },
    {
      "id":"d66f2902-9d12-4ff8-ab01-21ec6706079f",
      "businessPhones":[

      ],
      "displayName":"Alan Steiner",
      "givenName":"Alan",
      "jobTitle":"VP Corporate Marketing",
      "mail":"alans@contoso.onmicrosoft.com",
      "mobilePhone":null,
      "officeLocation":null,
      "preferredLanguage":"en-US",
      "surname":"Steiner",
      "userPrincipalName":"alans@contoso.onmicrosoft.com"
    }
  ]
}
```

<span data-ttu-id="7512c-p106">O Microsoft Graph também permite exibir coleções navegando entre as relações de um recurso com o outro. Por exemplo, por meio de uma propriedade de navegação **mailFolders**,você pode consultar uma coleção de recursos [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0), na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="7512c-p106">Microsoft Graph also lets you view collections by navigating the relationships of one resource with another. For example, through a user's **mailFolders** navigation property, you can query for the collection of [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0) resources in the user's mailbox:</span></span>

```no-highlight
GET https://graph.microsoft.com/v1.0/me/mailfolders HTTP/1.1
Authorization : Bearer {access_token}
```

<span data-ttu-id="7512c-p107">Se tiver êxito, você receberá uma resposta 200 OK que contém a coleção de recursos [mailFolder](/graph/api/resources/user?view=graph-rest-1.0) no payload. Cada recurso **mailFolder** será identificado pela propriedade **id** e acompanhado pelas respectivas propriedades. O payload exibido abaixo foi truncado por uma questão de resumo.</span><span class="sxs-lookup"><span data-stu-id="7512c-p107">If successful, you'll get a 200 OK response that contains the collection of [mailFolder](/graph/api/resources/user?view=graph-rest-1.0) resources in the payload. Each **mailFolder** is identified by the **id** property and accompanied by its properties. The payload shown below is truncated for brevity.</span></span>

```no-highlight
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('16f5a7b6-5a15-4568-aa5a-31bb117e9967')/mailFolders",
  "value":[
    {
      "id":"AAMkADRm9AABDGisXAAA=",
      "displayName":"Archive",
      "parentFolderId":"AQMkADRmZWj0AAAIBCAAAAA==",
      "childFolderCount":0,
      "unreadItemCount":0,
      "totalItemCount":0
    },
    {
      "id":"AQMkADRm0AAAIBXAAAAA==",
      "displayName":"Sales reports",
      "parentFolderId":"AQMkADRmZWj0AAAIBCAAAAA==",
      "childFolderCount":0,
      "unreadItemCount":0,
      "totalItemCount":0
    },
    {
      "id":"AAMkADRCxI9AAAT6CAIAAA=",
      "displayName":"Conversation History",
      "parentFolderId":"AQMkADRmZWj0AAAIBCAAAAA==",
      "childFolderCount":1,
      "unreadItemCount":0,
      "totalItemCount":0
    }
  ]
}
```




## <a name="view-a-specific-resource-from-a-collection-by-id"></a><span data-ttu-id="7512c-131">Exibir um recurso específico de uma coleção pela ID</span><span class="sxs-lookup"><span data-stu-id="7512c-131">View a specific resource from a collection by ID</span></span>

<span data-ttu-id="7512c-132">Para exibir as informações sobre um usuário, ainda com o uso do recurso **user** como exemplo, use uma solicitação GET HTTPS para chegar a um usuário específico pela ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="7512c-132">Continuing with using **user** as an example - to view the information about a user, use an HTTPS GET request to get a specific user by the user's ID. For a user entity, you can use either the id or userPrincipalName property as the identifier. The following request example uses the userPrincipalName value as the user's ID.</span></span> <span data-ttu-id="7512c-133">No caso de uma entidade **user**, você pode usar a propriedade **id** ou **userPrincipalName** como identificador.</span><span class="sxs-lookup"><span data-stu-id="7512c-133">For a **user** entity, you can use either the **id** or **userPrincipalName** property as the identifier.</span></span>

<span data-ttu-id="7512c-134">A solicitação de exemplo a seguir usa o valor **userPrincipalName** como ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="7512c-134">The following example request uses the \*\*\*\* value as the user's id.</span></span>

```no-highlight
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com HTTP/1.1
Authorization : Bearer {access_token}
```

<span data-ttu-id="7512c-135">Se tiver êxito, você obterá uma resposta 200 OK que contém a representação do recurso do usuário na carga, conforme mostrado.</span><span class="sxs-lookup"><span data-stu-id="7512c-135">If successful, you'll get a 200 OK response that contains the user resource representation in the payload, as shown.</span></span>

```no-highlight
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal
content-length: 982

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
    "id": "c95e3b3a-c33b-48da-a6e9-eb101e8a4205",
    "city": "Redmond",
    "country": "USA",
    "department": "Help Center",
    "displayName": "John Doe",
    "givenName": "John",
    "userPrincipalName": "john.doe@contoso.onmicrosoft.com",

    ...
}
```

## <a name="read-specific-properties-of-a-resource"></a><span data-ttu-id="7512c-136">Ler propriedades específicas de um recurso</span><span class="sxs-lookup"><span data-stu-id="7512c-136">Read specific properties of a resource</span></span>
<span data-ttu-id="7512c-137">Para recuperar apenas os dados biográficos do usuário, conforme fornecido por ele na descrição _Sobre mim_, e suas habilidades, você pode adicionar o parâmetro de consulta [$select](query-parameters.md) à solicitação anterior, como mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="7512c-137">To retrieve only the user's biographical data, such as the user's provided _About me_ description and their skill set, you can add the [$select](query-parameters.md) query parameter to the previous request, as shown in the following example.</span></span>

```no-highlight
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com?$select=displayName,aboutMe,skills HTTP/1.1
Authorization : Bearer {access_token}
```

<span data-ttu-id="7512c-138">A resposta bem-sucedida retorna o status 200 OK e uma carga, conforme mostrado.</span><span class="sxs-lookup"><span data-stu-id="7512c-138">The successful response returns the 200 OK status and a payload, as shown.</span></span>

```no-highlight
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal
content-length: 169

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
    "aboutMe": "A cool and nice guy.",
    "displayName": "John Doe",
    "skills": [
        "n-Lingual",
        "public speaking",
        "doodling"
    ]
}
```
<span data-ttu-id="7512c-139">Aqui, em vez de todos os conjuntos de propriedade na entidade **user**, somente as propriedades básicas **aboutMe**, **displayName** e **skills** são retornadas.</span><span class="sxs-lookup"><span data-stu-id="7512c-139">Here, instead of the entire property sets on the **user** entity, only the **aboutMe**, **displayName**, and **skills** basic properties are returned.</span></span>

## <a name="read-specific-properties-of-the-resources-in-a-collection"></a><span data-ttu-id="7512c-140">Ler propriedades específicas dos recursos em uma coleção</span><span class="sxs-lookup"><span data-stu-id="7512c-140">Read specific properties of the resources in a collection</span></span>
<span data-ttu-id="7512c-141">Além de ler propriedades específicas de um único recurso, você também pode aplicar o parâmetro de consulta [$select](query-parameters.md) semelhante a uma coleção para obter todos os recursos na coleção com apenas as propriedades específicas retornadas em cada um.</span><span class="sxs-lookup"><span data-stu-id="7512c-141">In addition to reading specific properties of a single resource, you can also apply the similar [$select](query-parameters.md) query parameter to a collection to get back all resources in the collection with just the specific properties returned on each. For example, to query the name of the signed-in user's drive items, you can submit the following HTTPS GET request.</span></span>

<span data-ttu-id="7512c-142">Por exemplo, para consultar o nome dos itens na unidade do usuário conectado, você pode enviar a seguinte solicitação HTTPS GET.</span><span class="sxs-lookup"><span data-stu-id="7512c-142">For example, to query the name of the signed-in user's drive items, you can submit the following HTTPS GET request:</span></span>

```no-highlight
GET https://graph.microsoft.com/v1.0/me/drive/root/children?$select=name HTTP/1.1
Authorization : Bearer {access_token}
```

<span data-ttu-id="7512c-143">A resposta bem-sucedida retorna um código de status 200 OK e uma carga que contém apenas os nomes dos arquivos compartilhados, conforme mostrado no exemplo abaixo.</span><span class="sxs-lookup"><span data-stu-id="7512c-143">The successful response returns a 200 OK status code and a payload that contains only the names of the shared files, as shown in the following example.</span></span>

```no-highlight
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('john.doe%40contoso.onmicrosoft.com')/drive/root/children(name,type)",
  "value": [
    {
      "@odata.etag": "\"{896A8E4D-27BF-424B-A0DA-F073AE6570E2},2\"",
      "name": "Shared with Everyone"
    },
    {
      "@odata.etag": "\"{B39D5D2E-E968-491A-B0EB-D5D0431CB423},1\"",
      "name": "Documents"
    },
    {
      "@odata.etag": "\"{9B51EA38-3EE6-4DC1-96A6-230E325EF054},2\"",
      "name": "newFile.txt"
    }
  ]
}
```

## <a name="traverse-from-one-resource-to-another-via-relationship"></a><span data-ttu-id="7512c-144">Passar de um recurso para outro pela relação</span><span class="sxs-lookup"><span data-stu-id="7512c-144">Traverse from one resource to another via relationship</span></span>
<span data-ttu-id="7512c-p109">Um gerente tem uma relação **directReports** com outros usuários diretamente subordinados a ele. Para consultar a lista de subordinados de um usuário, você pode usar a solicitação HTTPS GET a seguir para navegar para o destino pretendido via passagem de relação.</span><span class="sxs-lookup"><span data-stu-id="7512c-p109">A manager holds a **directReports** relationship with the other users reporting to him or her. To query the list of the direct reports of a user, you can use the following HTTPS GET request to navigate to the intended target via relationship traversal.</span></span>

```no-highlight
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com/directReports HTTP/1.1
Authorization : Bearer {access_token}
```

<span data-ttu-id="7512c-147">A resposta bem-sucedida retorna o status 200 OK e uma carga, conforme mostrado.</span><span class="sxs-lookup"><span data-stu-id="7512c-147">The successful response returns the 200 OK status and a payload, as shown.</span></span>

```no-highlight
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal
content-length: 152

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects/$entity",
    "@odata.type": "#microsoft.graph.user",
    "id": "c37b074d-fe9d-4e68-83ad-b4401d3be174",
    "department": "Sales & Marketing",
    "displayName": "Bonnie Kearney",

    ...
}
```

<span data-ttu-id="7512c-p110">Da mesma forma, você pode seguir um relacionamento para navegar até os recursos relacionados. Por exemplo, a relação mensagens-usuário habilita a passagem de um usuário do Azure Active Directory (Microsoft Azure AD) para um conjunto de mensagens de email do Outlook. O exemplo a seguir mostra como fazer isso em uma chamada à API REST.</span><span class="sxs-lookup"><span data-stu-id="7512c-p110">Similarly, you can follow a relationship to navigate to related resources. For example, the user-messages relationship enables traversal from an Azure Active Directory (Azure AD) User to a set of Outlook mail messages. The following example shows how to do this in a REST API call.</span></span>


```no-highlight
GET https://graph.microsoft.com/v1.0/me/messages HTTP/1.1
Authorization : Bearer {access_token}
```


<span data-ttu-id="7512c-151">A resposta bem-sucedida retorna o status 200 OK e uma carga, conforme mostrado.</span><span class="sxs-lookup"><span data-stu-id="7512c-151">The successful response returns the 200 OK status and a payload, as shown.</span></span>


```no-highlight
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal
odata-version: 4.0
content-length: 147

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('john.doe%40contoso.onmicrosoft.com')/Messages",
  "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/messages?$top=1&$skip=1",
  "value": [
    {
      "@odata.etag": "W/\"FwAAABYAAABMR67yw0CmT4x0kVgQUH/3AAJL+Kej\"",
      "id": "<id-value>",
      "createdDateTime": "2015-11-14T00:24:42Z",
      "lastModifiedDateTime": "2015-11-14T00:24:42Z",
      "changeKey": "FwAAABYAAABMR67yw0CmT4x0kVgQUH/3AAJL+Kej",
      "categories": [],
      "receivedDateTime": "2015-11-14T00:24:42Z",
      "sentDateTime": "2015-11-14T00:24:28Z",
      "hasAttachments": false,
      "subject": "Did you see last night's game?",
      "body": {
        "ContentType": "HTML",
        "Content": "<content>"
      },
      "BodyPreview": "it was great!",
      "Importance": "Normal",

       ...
    }
  ]
}
```
<span data-ttu-id="7512c-152">Você pode ver todas as relações em um determinado recurso indo para os metadados, localizando `EntityType` e examinando todas as`NavigationProperty` do `EntityType`.</span><span class="sxs-lookup"><span data-stu-id="7512c-152">You can see all the relationships on a given resource by going to the metadata, finding the EntityType, and looking at all NavigationProperties for that EntityType.</span></span>

## <a name="call-actions-and-functions"></a><span data-ttu-id="7512c-153">Funções e ações de chamada</span><span class="sxs-lookup"><span data-stu-id="7512c-153">Call actions or functions</span></span>
<span data-ttu-id="7512c-154">O Microsoft Graph também oferece suporte a _ações_ e _funções_ para manipular recursos de maneiras que não são apenas operações de criar, ler, atualizar e excluir (CRUD).</span><span class="sxs-lookup"><span data-stu-id="7512c-154">Microsoft Graph also supports _actions_ and _functions_ to manipulate resources in ways that are not simply create, read, update, and delete (CRUD) operations.</span></span> <span data-ttu-id="7512c-155">Eles normalmente estão na forma de solicitações de HTTPS POST para receber argumentos para ação e função.</span><span class="sxs-lookup"><span data-stu-id="7512c-155">They are often in the shape of HTTPS POST requests in order to intake arguments for the action or function.</span></span> <span data-ttu-id="7512c-156">Por exemplo, a seguinte ação permite que o usuário conectado (`me`) envie uma mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="7512c-156">For example, the following HTTPS POST request lets the signed-in user (`me`) send an email message:</span></span>

```no-highlight
POST https://graph.microsoft.com/v1.0/me/sendMail HTTP/1.1
authorization: bearer {access_token}
content-type: application/json
content-length: 96

{
  "message": {
    "subject": "Meet for lunch?",
    "body": {
      "contentType": "Text",
      "content": "The new cafeteria is open."
    },
    "toRecipients": [
      {
        "emailAddress": {
          "address": "garthf@contoso.onmicrosoft.com"
        }
      }
    ],
    "attachments": [
      {
        "@odata.type": "microsoft.graph.fileAttachment",
        "name": "menu.txt",
        "contentBytes": "bWFjIGFuZCBjaGVlc2UgdG9kYXk="
      }
    ]
  },
  "saveToSentItems": "false"
}
```

<span data-ttu-id="7512c-p112">Você pode ver todas as funções que estão disponíveis nos metadados. Eles aparecem como Funções ou Ações.</span><span class="sxs-lookup"><span data-stu-id="7512c-p112">You can see all the functions that are available in the metadata. They appear as Functions or Actions.</span></span>

## <a name="use-the-microsoft-graph-sdks"></a><span data-ttu-id="7512c-159">Usar os SDKs do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7512c-159">Use the Microsoft Graph SDKs</span></span>

<span data-ttu-id="7512c-p113">Como o poder e a facilidade dos SDKs? Enquanto você sempre pode usar APIs REST para chamar o Microsoft Graph, também fornecemos SDKs para muitas plataformas populares. Para explorar os SDKs disponíveis, veja [Amostras de código e SDKs](https://developer.microsoft.com/graph/code-samples-and-sdks).</span><span class="sxs-lookup"><span data-stu-id="7512c-p113">Like the power and ease of SDKs? While you can always use REST APIs to call Microsoft Graph, we also provide SDKs for many popular platforms. To explore the SDKs that are available, see [Code samples and SDKs](https://developer.microsoft.com/graph/code-samples-and-sdks).</span></span>

## <a name="see-also"></a><span data-ttu-id="7512c-163">Confira também</span><span class="sxs-lookup"><span data-stu-id="7512c-163">See also</span></span>

- [<span data-ttu-id="7512c-164">Usar a API do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7512c-164">Use the Microsoft Graph API</span></span>](use-the-api.md)
- [<span data-ttu-id="7512c-165">Obter tokens de autenticação</span><span class="sxs-lookup"><span data-stu-id="7512c-165">Get auth tokens</span></span>](/graph/auth)
