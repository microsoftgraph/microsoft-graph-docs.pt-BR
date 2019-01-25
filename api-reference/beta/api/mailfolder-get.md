---
title: Obter mailFolder
description: Recupere as propriedades e os relacionamentos de um objeto da pasta de mensagens.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: eee7adf677696fbf2dc969262604b817c7cddabe
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529905"
---
# <a name="get-mailfolder"></a><span data-ttu-id="7812d-103">Obter mailFolder</span><span class="sxs-lookup"><span data-stu-id="7812d-103">Get mailFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7812d-104">Recupere as propriedades e os relacionamentos de um objeto da pasta de mensagens.</span><span class="sxs-lookup"><span data-stu-id="7812d-104">Retrieve the properties and relationships of a message folder object.</span></span>

<span data-ttu-id="7812d-105">Há dois cenários onde um aplicativo pode obter a pasta de correio de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="7812d-105">There are two scenarios where an app can get another user's mail folder:</span></span>

* <span data-ttu-id="7812d-106">Se o aplicativo tem permissões de aplicativo, ou,</span><span class="sxs-lookup"><span data-stu-id="7812d-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="7812d-107">Se o aplicativo tiver apropriada [permissões](#permissions) delegadas de um usuário, e outro usuário compartilhou uma pasta de email com que o usuário ou, tem acesso delegado a esse usuário.</span><span class="sxs-lookup"><span data-stu-id="7812d-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="7812d-108">Consulte os [detalhes e um exemplo](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="7812d-108">See [details and an example](/graph/outlook-share-messages-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="7812d-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="7812d-109">Permissions</span></span>
<span data-ttu-id="7812d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7812d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7812d-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7812d-112">Permission type</span></span>      | <span data-ttu-id="7812d-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7812d-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7812d-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7812d-114">Delegated (work or school account)</span></span> | <span data-ttu-id="7812d-115">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7812d-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="7812d-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7812d-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7812d-117">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7812d-117">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="7812d-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7812d-118">Application</span></span> | <span data-ttu-id="7812d-119">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7812d-119">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7812d-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7812d-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7812d-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7812d-121">Optional query parameters</span></span>
<span data-ttu-id="7812d-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7812d-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7812d-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7812d-123">Request headers</span></span>
| <span data-ttu-id="7812d-124">Nome</span><span class="sxs-lookup"><span data-stu-id="7812d-124">Name</span></span>       | <span data-ttu-id="7812d-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="7812d-125">Type</span></span> | <span data-ttu-id="7812d-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="7812d-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7812d-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="7812d-127">Authorization</span></span>  | <span data-ttu-id="7812d-128">string</span><span class="sxs-lookup"><span data-stu-id="7812d-128">string</span></span>  | <span data-ttu-id="7812d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7812d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7812d-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7812d-131">Request body</span></span>
<span data-ttu-id="7812d-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7812d-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7812d-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="7812d-133">Response</span></span>
<span data-ttu-id="7812d-134">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [mailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7812d-134">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example-1"></a><span data-ttu-id="7812d-135">Exemplo 1</span><span class="sxs-lookup"><span data-stu-id="7812d-135">Example 1</span></span>
#### <a name="request-1"></a><span data-ttu-id="7812d-136">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="7812d-136">Request 1</span></span>
<span data-ttu-id="7812d-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7812d-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailfolder"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
```

#### <a name="response-1"></a><span data-ttu-id="7812d-138">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="7812d-138">Response 1</span></span>
<span data-ttu-id="7812d-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7812d-139">The following is an example of the response.</span></span>
 ><span data-ttu-id="7812d-140">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7812d-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7812d-141">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7812d-141">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
    "id": "AAMkAGVmMDEzM",
    "displayName": "Inbox",
    "parentFolderId": "AAMkAGVmMDEzI",
    "childFolderCount": 2,
    "unreadItemCount": 59,
    "totalItemCount": 60,
    "wellKnownName": "inbox"
}
```

## <a name="example-2"></a><span data-ttu-id="7812d-142">Exemplo 2</span><span class="sxs-lookup"><span data-stu-id="7812d-142">Example 2</span></span>
#### <a name="request-2"></a><span data-ttu-id="7812d-143">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="7812d-143">Request 2</span></span>
<span data-ttu-id="7812d-144">O exemplo a seguir é um exemplo de pasta de pesquisa da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7812d-144">The following is a search folder example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailSearchfolder"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
```

#### <a name="response-2"></a><span data-ttu-id="7812d-145">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="7812d-145">Response 2</span></span>
<span data-ttu-id="7812d-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7812d-146">The following is an example of the response.</span></span>
 ><span data-ttu-id="7812d-147">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7812d-147">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7812d-148">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7812d-148">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
    "id": "AAMkAGVmMDEzM",
    "displayName": "Inbox",
    "parentFolderId": "AAMkAGVmMDEzI",
    "childFolderCount": 2,
    "unreadItemCount": 59,
    "totalItemCount": 60,
    "wellKnownName": "inbox"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/mailfolder-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
