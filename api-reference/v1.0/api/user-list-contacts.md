---
title: Listar contatos
description: Obter uma coleção de contato da pasta padrão Contatos do usuário conectado.
ms.openlocfilehash: 296844eb4eea93c5bd46e8028f3423fe797142ab
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005628"
---
# <a name="list-contacts"></a><span data-ttu-id="7a460-103">Listar contatos</span><span class="sxs-lookup"><span data-stu-id="7a460-103">List contacts</span></span>

<span data-ttu-id="7a460-104">Obter uma coleção de contato da pasta padrão Contatos do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="7a460-104">Get a contact collection from the default contacts folder of the signed-in user.</span></span>

<span data-ttu-id="7a460-105">Há dois cenários onde um aplicativo pode obter contatos na pasta de contatos de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="7a460-105">There are two scenarios where an app can get contacts in another user's contact folder:</span></span>

* <span data-ttu-id="7a460-106">Se o aplicativo tem permissões de aplicativo, ou,</span><span class="sxs-lookup"><span data-stu-id="7a460-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="7a460-107">Se o aplicativo tiver apropriada [permissões](#permissions) delegadas de um usuário, e outro usuário compartilhou uma pasta de contato com que o usuário ou, tem acesso delegado a esse usuário.</span><span class="sxs-lookup"><span data-stu-id="7a460-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="7a460-108">Consulte os [detalhes e um exemplo](/graph/outlook-get-shared-contacts-folders).</span><span class="sxs-lookup"><span data-stu-id="7a460-108">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="7a460-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="7a460-109">Permissions</span></span>
<span data-ttu-id="7a460-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a460-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a460-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7a460-112">Permission type</span></span>      | <span data-ttu-id="7a460-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7a460-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7a460-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7a460-114">Delegated (work or school account)</span></span> | <span data-ttu-id="7a460-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7a460-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="7a460-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7a460-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a460-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7a460-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="7a460-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7a460-118">Application</span></span> | <span data-ttu-id="7a460-119">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7a460-119">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7a460-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7a460-120">HTTP request</span></span>

<span data-ttu-id="7a460-121">Para obter todos os contatos na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="7a460-121">To get all the contacts in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

<span data-ttu-id="7a460-122">Para obter os contatos em uma pasta específica na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="7a460-122">To get contacts in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7a460-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7a460-123">Optional query parameters</span></span>
<span data-ttu-id="7a460-124">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7a460-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="7a460-125">Por exemplo, você pode usar o parâmetro de consulta `$filter` para filtrar os contatos com base no domínio dos endereços de email deles:</span><span class="sxs-lookup"><span data-stu-id="7a460-125">For example, you can use the `$filter` query parameter to filter contacts based on the domain of their email addresses:</span></span>

`https://graph.microsoft.com/v1.0/me/contacts?$filter=emailAddresses/any(a:a/address eq '@domain.com')`



## <a name="request-headers"></a><span data-ttu-id="7a460-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7a460-126">Request headers</span></span>
| <span data-ttu-id="7a460-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7a460-127">Header</span></span>       | <span data-ttu-id="7a460-128">Valor</span><span class="sxs-lookup"><span data-stu-id="7a460-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7a460-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="7a460-129">Authorization</span></span>  | <span data-ttu-id="7a460-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a460-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7a460-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7a460-132">Content-Type</span></span>   | <span data-ttu-id="7a460-133">application/json</span><span class="sxs-lookup"><span data-stu-id="7a460-133">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7a460-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7a460-134">Request body</span></span>
<span data-ttu-id="7a460-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7a460-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a460-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a460-136">Response</span></span>

<span data-ttu-id="7a460-137">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Contact](../resources/contact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7a460-137">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7a460-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7a460-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7a460-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7a460-139">Request</span></span>
<span data-ttu-id="7a460-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7a460-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contacts
```


##### <a name="response"></a><span data-ttu-id="7a460-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a460-141">Response</span></span>
<span data-ttu-id="7a460-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7a460-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "birthday": "datetime-value",
      "fileAs": "fileAs-value",
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "initials": "initials-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List contacts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
