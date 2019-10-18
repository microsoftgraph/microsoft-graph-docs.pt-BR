---
title: Chamando a API do Microsoft Graph
description: 'Para acessar e manipular um recurso do Microsoft Graph, você chama e especifica as URLs de recurso usando uma das operações a seguir:   '
localization_priority: Normal
author: VinodRavichandran
ms.prod: microsoft-teams
ms.openlocfilehash: b2b1af0aa2d2e31bbaa4fd70ef87a2dddef5284f
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778625"
---
# <a name="calling-the-microsoft-graph-api"></a><span data-ttu-id="8d04a-103">Chamando a API do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8d04a-103">Calling the Microsoft Graph API</span></span>

<span data-ttu-id="8d04a-104">Para acessar e manipular um recurso do Microsoft Graph, você chama e especifica as URLs de recurso usando uma das operações a seguir:</span><span class="sxs-lookup"><span data-stu-id="8d04a-104">To access and manipulate a Microsoft Graph resource, you call and specify the resource URLs using one of the following operations:</span></span>   

- <span data-ttu-id="8d04a-105">GET</span><span class="sxs-lookup"><span data-stu-id="8d04a-105">GET</span></span>
- <span data-ttu-id="8d04a-106">POST</span><span class="sxs-lookup"><span data-stu-id="8d04a-106">POST</span></span>
- <span data-ttu-id="8d04a-107">PATCH</span><span class="sxs-lookup"><span data-stu-id="8d04a-107">PATCH</span></span>
- <span data-ttu-id="8d04a-108">PUT</span><span class="sxs-lookup"><span data-stu-id="8d04a-108">PUT</span></span>
- <span data-ttu-id="8d04a-109">DELETE</span><span class="sxs-lookup"><span data-stu-id="8d04a-109">DELETE</span></span> 

<span data-ttu-id="8d04a-110">Todas as solicitações de API do Microsoft Graph usam o seguinte padrão de URL básico:</span><span class="sxs-lookup"><span data-stu-id="8d04a-110">All Microsoft Graph API requests use the following basic URL pattern:</span></span>

```
    https://graph.microsoft.com/{version}/{resource}?[query_parameters]
```

<span data-ttu-id="8d04a-111">Para esta URL:</span><span class="sxs-lookup"><span data-stu-id="8d04a-111">For this URL:</span></span>

- <span data-ttu-id="8d04a-112">`https://graph.microsoft.com` é o ponto de extremidade da API do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8d04a-112">`https://graph.microsoft.com` is the Microsoft Graph API endpoint.</span></span>
- <span data-ttu-id="8d04a-113">`{version}` é a versão de serviço de destino, por exemplo, `v1.0` ou `beta`.</span><span class="sxs-lookup"><span data-stu-id="8d04a-113">`{version}` is the target service version, for example, `v1.0` or `beta`.</span></span>
- <span data-ttu-id="8d04a-114">`{resource}` é o caminho ou o segmento de recursos, como:</span><span class="sxs-lookup"><span data-stu-id="8d04a-114">`{resource}` is resource segment or path, such as:</span></span>
  - <span data-ttu-id="8d04a-115">`users`, `groups`, `devices`, `organization`</span><span class="sxs-lookup"><span data-stu-id="8d04a-115"></span></span>
  - <span data-ttu-id="8d04a-116">O alias `me`, que é resolvido como o usuário conectado</span><span class="sxs-lookup"><span data-stu-id="8d04a-116">The alias `me`, which resolves to the signed-in user</span></span>
  - <span data-ttu-id="8d04a-117">Os recursos que pertencem a um usuário, como `me/events`, `me/drive` ou `me/messages`</span><span class="sxs-lookup"><span data-stu-id="8d04a-117">The resources belonging to a user, such as `me/events`, `me/drive` or `me/messages`</span></span>
  - <span data-ttu-id="8d04a-118">O alias `myOrganization`, que é resolvido como o locatário do usuário conectado da organização</span><span class="sxs-lookup"><span data-stu-id="8d04a-118">The alias `myOrganization`, which resolves to the tenant of the organization signed-in user</span></span>
- <span data-ttu-id="8d04a-119">`[query_parameters]` representa os parâmetros de consulta adicionais, como `$filter` e `$select`.</span><span class="sxs-lookup"><span data-stu-id="8d04a-119">`[query_parameters]` represents additional query parameters such as `$filter` and `$select`.</span></span>

<span data-ttu-id="8d04a-p101">Opcionalmente, você também pode especificar o locatário como parte da sua solicitação. Ao usar `me`, não especifique o locatário. Para obter uma lista com as solicitações comuns, consulte [Visão geral do Microsoft Graph](overview.md).</span><span class="sxs-lookup"><span data-stu-id="8d04a-p101">Optionally, you can also specify the tenant as part of your request. When using `me`, do not specify the tenant. For a list of common requests, see [Overview of Microsoft Graph](overview.md).</span></span>

## <a name="microsoft-graph-api-metadata"></a><span data-ttu-id="8d04a-123">Metadados da API do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8d04a-123">Microsoft Graph API metadata</span></span>
<span data-ttu-id="8d04a-p102">O documento de metadados ($metadata) é publicado na raiz do serviço. Por exemplo, você pode exibir o documento de serviço para as versões 1.0 e beta com as URLs a seguir.</span><span class="sxs-lookup"><span data-stu-id="8d04a-p102">The metadata document ($metadata) is published at the service root. For example, you can view the service document for the v1.0 and beta versions via the following URLs.</span></span>

<span data-ttu-id="8d04a-126">Metadados `v1.0` da API do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8d04a-126">Microsoft Graph API `v1.0` metadata.</span></span>
```
    https://graph.microsoft.com/v1.0/$metadata
```
<span data-ttu-id="8d04a-127">Metadados `beta` da API do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8d04a-127">Microsoft Graph API `beta` metadata.</span></span>
```
    https://graph.microsoft.com/beta/$metadata
```

<span data-ttu-id="8d04a-128">Os metadados permitem que você veja e entenda o modelo de dados do Microsoft Graph, incluindo os tipos de entidade e conjuntos, os tipos complexos e as enums que compõem os pacotes de solicitação e resposta enviados para e do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8d04a-128">The metadata allows you to see and understand the data model of Microsoft Graph, including the entity types and sets, complex types, and enums that make up the request and response packets sent to and from Microsoft Graph.</span></span>
<span data-ttu-id="8d04a-129">Você pode usar os metadados para compreender as relações entre entidades no Microsoft Graph e estabelecer URLs que navegam entre entidades.</span><span class="sxs-lookup"><span data-stu-id="8d04a-129">You can use the metadata to understand the realtionships between entities in Microsoft Graph and establish URLs that navigate between entities.</span></span>
<span data-ttu-id="8d04a-130">Essa capacidade de interconexão baseada em navegação dá ao Microsoft Graph seu caráter exclusivo.</span><span class="sxs-lookup"><span data-stu-id="8d04a-130">This navigation-based interconnectedness gives Microsoft Graph its unique character.</span></span>

<span data-ttu-id="8d04a-131">Os nomes de recursos e parâmetros de consulta da URL do caminho e os parâmetros e valores de ação não diferenciam maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="8d04a-131">Path URL resource names, query parameters, and action parameters and values are case insensitive.</span></span> <span data-ttu-id="8d04a-132">No entanto, os valores que atribuir, as IDs de entidade e outros valores codificados na base 64 diferenciam maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="8d04a-132">However, values you assign, entity IDs, and other base64-encoded values are case-sensitive.</span></span>

<span data-ttu-id="8d04a-133">As seguintes seções mostram algumas chamadas básicas de padrão de programação para a API do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8d04a-133">The following sections show a few basic programming pattern calls to the Microsoft Graph API.</span></span>

## <a name="navigate-from-a-set-to-a-member"></a><span data-ttu-id="8d04a-134">Navegar de uma coleção para um membro</span><span class="sxs-lookup"><span data-stu-id="8d04a-134">Navigate from a set to a member</span></span>

<span data-ttu-id="8d04a-p105">Para exibir as informações sobre um usuário, você obtém a entidade `User` da coleção `users` para o usuário específico identificado por seu identificador usando uma solicitação HTTPS GET. Para uma entidade `User`, tanto a propriedade `id` quanto a `userPrincipalName` podem ser usadas como o identificador. A solicitação de exemplo a seguir usa o valor `userPrincipalName` como ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="8d04a-p105">To view the information about a user, you get the `User` entity from the `users` collection to the specific user identified by its identifier, using an HTTPS GET request. For a `User` entity, either the `id` or `userPrincipalName` property can be used as the identifier. The following example request uses the `userPrincipalName` value as the user's id.</span></span> 

```no-highlight 
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com HTTP/1.1
Authorization : Bearer <access_token>
```

<span data-ttu-id="8d04a-138">Se tiver êxito, você obterá uma resposta 200 OK contendo a representação de recursos do usuário na carga, conforme mostrado abaixo:</span><span class="sxs-lookup"><span data-stu-id="8d04a-138">If successful, you should get a 200 OK response containing the user resource representation in the payload, as shown as follows:</span></span>

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


## <a name="project-from-an-entity-to-properties"></a><span data-ttu-id="8d04a-139">Projetar de uma entidade para as propriedades</span><span class="sxs-lookup"><span data-stu-id="8d04a-139">Project from an entity to properties</span></span>
<span data-ttu-id="8d04a-p106">Para recuperar apenas os dados biográficos do usuário, conforme fornecido por ele na descrição _Sobre mim_, e suas habilidades, você pode adicionar o parâmetro de consulta _select_ à solicitação anterior. Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="8d04a-p106">To retrieve only the user's biographical data, such as the user's provided _About me_ description and their skill set, you can add the _select_ query parameter to the previous request. For example:</span></span>

```no-highlight 
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com?$select=displayName,aboutMe,skills HTTP/1.1
Authorization : Bearer <access_token>
```

<span data-ttu-id="8d04a-142">A resposta bem-sucedida retorna o status 200 OK e uma carga com o seguinte formato:</span><span class="sxs-lookup"><span data-stu-id="8d04a-142">The successful response returns the 200 OK status and a payload of the following format:</span></span>

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

<span data-ttu-id="8d04a-143">Aqui, em vez de todos os conjuntos de propriedade na entidade `user`, somente as propriedades `aboutMe`, `displayName` e `skills` são retornadas.</span><span class="sxs-lookup"><span data-stu-id="8d04a-143">Here, instead of the entire property sets on the `user` entity, only the `aboutMe`, `displayName`, and `skills` properties are returned.</span></span>

## <a name="traverse-to-another-resource-via-relationship"></a><span data-ttu-id="8d04a-144">Passar para outro recurso por meio de relação</span><span class="sxs-lookup"><span data-stu-id="8d04a-144">Traverse to another resource via relationship</span></span>
<span data-ttu-id="8d04a-p107">Um gerente tem uma relação `directReports` com outros usuários diretamente subordinados a ele. Para consultar a lista de subordinados de um usuário, você pode usar a solicitação HTTPS GET a seguir para navegar para o destino pretendido via passagem de relação.</span><span class="sxs-lookup"><span data-stu-id="8d04a-p107">A manager holds a `directReports` relationship with the other users reporting to him or her. To query the list of the direct reports of a user, you can use the following HTTPS GET request to navigate to the intended target via relationship traversal.</span></span> 

```no-highlight 
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com/directReports HTTP/1.1
Authorization : Bearer <access_token>
```

<span data-ttu-id="8d04a-147">A resposta bem-sucedida retorna o status 200 OK e uma carga com o seguinte formato:</span><span class="sxs-lookup"><span data-stu-id="8d04a-147">The successful response returns the 200 OK status and a payload of the following format:</span></span>

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

<span data-ttu-id="8d04a-p108">Da mesma forma, você pode seguir um relacionamento para navegar até os recursos relacionados. Por exemplo, a relação `user => messages` habilita a passagem de um usuário do Azure AD para um conjunto de mensagens de email do Outlook. O exemplo a seguir mostra como fazer isso em uma chamada à API REST:</span><span class="sxs-lookup"><span data-stu-id="8d04a-p108">Similarly, you can follow a relationship to navigate to related resources. For example, the `user => messages` relationship enables traversal from an Azure AD User to a set of Outlook mail messages. The following example shows how to do this in a REST API call:</span></span>


```no-highlight 
GET https://graph.microsoft.com/v1.0/me/messages HTTP/1.1
Authorization : Bearer <access_token>
```

    
<span data-ttu-id="8d04a-151">A resposta bem-sucedida retorna o status 200 OK e uma carga com o seguinte formato:</span><span class="sxs-lookup"><span data-stu-id="8d04a-151">The successful response returns the 200 OK status and a payload of the following format:</span></span>


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

## <a name="project-from-entities-to-properties"></a><span data-ttu-id="8d04a-152">Projetar das entidades para as propriedades</span><span class="sxs-lookup"><span data-stu-id="8d04a-152">Project from entities to properties</span></span>
<span data-ttu-id="8d04a-p109">Além da projeção de uma entidade única em suas propriedades, você também pode aplicar a opção de consulta `select` semelhante a uma coleção de entidades para projetá-las em uma coleção de algumas de suas propriedades. Por exemplo, para consultar o nome dos itens na unidade do usuário conectado, você pode enviar a seguinte solicitação HTTPS GET:</span><span class="sxs-lookup"><span data-stu-id="8d04a-p109">In addition to projection from a single entity to its properties, you can also apply the similar `select` query option to an entity collection to project them to a collection of some of their properties. For example, to query the name of the signed-in user's drive items, you can submit the following HTTPS GET request:</span></span>

```no-highlight 
GET https://graph.microsoft.com/v1.0/me/drive/root/children?$select=name HTTP/1.1
Authorization : Bearer <access_token>
```

<span data-ttu-id="8d04a-155">A resposta bem-sucedida retorna um código de status OK 200 e uma carga que contém os nomes e os tipos de arquivos compartilhados, conforme mostrado no exemplo abaixo:</span><span class="sxs-lookup"><span data-stu-id="8d04a-155">The successful response returns a 200 OK status code and a payload containing the names and types of the shared files, as shown in the following example:</span></span>

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

## <a name="query-a-subset-of-users-with-the-filtering-query-option"></a><span data-ttu-id="8d04a-156">Consulta um subconjunto de usuários com a opção de filtragem de consulta</span><span class="sxs-lookup"><span data-stu-id="8d04a-156">Query a subset of users with the filtering query option</span></span>
<span data-ttu-id="8d04a-p110">Para encontrar os funcionários em um determinado cargo dentro de uma organização, você pode navegar de uma coleção de usuários e especificar uma opção de consulta _filter_. Um exemplo é mostrado da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="8d04a-p110">To find the employees of a specific job title within an organization, you can navigate from the users collection and then specify a _filter_ query option. An example is shown as follows:</span></span>

    
```no-highlight 
GET https://graph.microsoft.com/v1.0/users/?$filter=jobTitle+eq+%27Helper%27 HTTP/1.1
Authorization : Bearer <access_token>
```

<span data-ttu-id="8d04a-159">A resposta bem-sucedida retorna o código de status OK 200 e uma lista de usuários com o cargo especificado (`'Helper'`), conforme mostrado no exemplo abaixo:</span><span class="sxs-lookup"><span data-stu-id="8d04a-159">The successful response returns the 200 OK status code and a list of users with the specified job title (`'Helper'`), as shown in the following example:</span></span>

```no-highlight 
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal;odata.streaming=true;IEEE754Compatible=false;charset=utf-8
odata-version: 4.0
content-length: 986

{
    "@odata.context": "https://graph.microsoft.com/v1.0/contoso.onmicrosoft.com/$metadata#users",
    "value": [
        {
            "id": "c95e3b3a-c33b-48da-a6e9-eb101e8a4205",
            "city": "Redmond",
            "country": "USA",
            "department": "Help Center",
            "displayName": "Jane Doe",
            "givenName": "Jane",
            "jobTitle": "Helper",
            ......
            "mailNickname": "Jane",
            "mobile": null,
            "otherMails": [
                "jane.doe@contoso.onmicrosoft.com"
            ],
            ......
            "surname": "Doe",
            "usageLocation": "US",
            "userPrincipalName": "help@contoso.onmicrosoft.com",
            "userType": "Member"
        },
        
        ...
    ]
}
```

## <a name="call-actions-or-functions"></a><span data-ttu-id="8d04a-160">Chamar funções ou ações</span><span class="sxs-lookup"><span data-stu-id="8d04a-160">Call actions or functions</span></span>
<span data-ttu-id="8d04a-p111">O Microsoft Graph também oferece suporte a _ações_ e _funções_ para manipular os recursos de maneiras que não sejam um simples ajuste com métodos HTTP padrão. Por exemplo, a seguinte solicitação HTTPS POST permite que o usuário conectado (`me`) envie uma mensagem de email:</span><span class="sxs-lookup"><span data-stu-id="8d04a-p111">Microsoft Graph also supports _actions_ and _functions_ to manipulate resources in ways that are not a simple fit with standard HTTP methods. For example, the following HTTPS POST request lets the signed-in user (`me`) send an email message:</span></span>
```no-highlight 
POST https://graph.microsoft.com/v1.0/me/sendMail HTTP/1.1
authorization: bearer <access_token>
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
          "address": "garthf@a830edad9050849NDA1.onmicrosoft.com"
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

<span data-ttu-id="8d04a-163">A carga de solicitação contém a entrada para a ação `sendMail`, que também é definida no $metadata.</span><span class="sxs-lookup"><span data-stu-id="8d04a-163">The request payload contains the input to the `sendMail` action, which is also defined in the $metadata.</span></span>

## <a name="use-microsoft-graph-client-libraries"></a><span data-ttu-id="8d04a-164">Usar as bibliotecas de cliente do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8d04a-164">Use Microsoft Graph client libraries</span></span>
<span data-ttu-id="8d04a-p112">Como o poder e a facilidade dos SDKs? Enquanto você sempre pode chamar o Microsoft Graph usando a API REST, fornecemos também SDKs para muitas plataformas populares.</span><span class="sxs-lookup"><span data-stu-id="8d04a-p112">Like the power and ease of SDKs? While you can always call Microsoft Graph using the REST API, we also provide SDKs for many popular platforms.</span></span>

<span data-ttu-id="8d04a-167">Explore os nossos [exemplos de código e SDKs](https://developer.microsoft.com/graph/code-samples-and-sdks).</span><span class="sxs-lookup"><span data-stu-id="8d04a-167">Explore our [code samples and SDKs](https://developer.microsoft.com/graph/code-samples-and-sdks).</span></span>
