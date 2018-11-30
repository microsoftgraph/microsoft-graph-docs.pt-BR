---
title: Obter contactFolder
description: Obtenha uma pasta de contatos usando a respectiva ID.
ms.openlocfilehash: f57471da55ea10128d0eaec4503c4f323a751fc0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033314"
---
# <a name="get-contactfolder"></a><span data-ttu-id="92d13-103">Obter contactFolder</span><span class="sxs-lookup"><span data-stu-id="92d13-103">Get contactFolder</span></span>

> <span data-ttu-id="92d13-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="92d13-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="92d13-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="92d13-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="92d13-106">Obtenha uma pasta de contatos usando a respectiva ID.</span><span class="sxs-lookup"><span data-stu-id="92d13-106">Get a contact folder by using the contact folder ID.</span></span>

<span data-ttu-id="92d13-107">Há dois cenários onde um aplicativo pode obter a pasta de contato do outro usuário:</span><span class="sxs-lookup"><span data-stu-id="92d13-107">There are two scenarios where an app can get another user's contact folder:</span></span>

* <span data-ttu-id="92d13-108">Se o aplicativo tem permissões de aplicativo, ou,</span><span class="sxs-lookup"><span data-stu-id="92d13-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="92d13-109">Se o aplicativo tiver apropriada [permissões](#permissions) delegadas de um usuário, e outro usuário compartilhou uma pasta de contato com que o usuário ou, tem acesso delegado a esse usuário.</span><span class="sxs-lookup"><span data-stu-id="92d13-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="92d13-110">Consulte os [detalhes e um exemplo](/graph/outlook-get-shared-contacts-folders).</span><span class="sxs-lookup"><span data-stu-id="92d13-110">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="92d13-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="92d13-111">Permissions</span></span>
<span data-ttu-id="92d13-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92d13-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92d13-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92d13-114">Permission type</span></span>      | <span data-ttu-id="92d13-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="92d13-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="92d13-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92d13-116">Delegated (work or school account)</span></span> | <span data-ttu-id="92d13-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="92d13-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="92d13-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92d13-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92d13-119">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="92d13-119">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="92d13-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92d13-120">Application</span></span> | <span data-ttu-id="92d13-121">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="92d13-121">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="92d13-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92d13-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="92d13-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="92d13-123">Optional query parameters</span></span>
<span data-ttu-id="92d13-124">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="92d13-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="92d13-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92d13-125">Request headers</span></span>
| <span data-ttu-id="92d13-126">Nome</span><span class="sxs-lookup"><span data-stu-id="92d13-126">Name</span></span>       | <span data-ttu-id="92d13-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="92d13-127">Type</span></span> | <span data-ttu-id="92d13-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="92d13-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="92d13-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="92d13-129">Authorization</span></span>  | <span data-ttu-id="92d13-130">string</span><span class="sxs-lookup"><span data-stu-id="92d13-130">string</span></span>  | <span data-ttu-id="92d13-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92d13-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="92d13-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92d13-133">Request body</span></span>
<span data-ttu-id="92d13-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="92d13-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92d13-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="92d13-135">Response</span></span>

<span data-ttu-id="92d13-136">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [contactFolder](../resources/contactfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92d13-136">If successful, this method returns a `200 OK` response code and [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="92d13-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="92d13-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="92d13-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92d13-138">Request</span></span>
<span data-ttu-id="92d13-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="92d13-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contactfolder"
}-->
```http
GET https://graph.microsoft.com/beta/me/contactFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="92d13-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="92d13-140">Response</span></span>
<span data-ttu-id="92d13-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="92d13-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 104

{
  "displayName": "Finance",
  "id": "AAMkAGI2TKI5AAA=",
  "parentFolderId": "AAMkAGI2AAEOAAA=",
  "wellKnownName": null
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
