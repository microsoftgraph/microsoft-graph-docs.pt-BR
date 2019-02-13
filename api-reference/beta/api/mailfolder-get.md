---
title: Obter mailFolder
description: Recupere as propriedades e os relacionamentos de um objeto da pasta de mensagens.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: af2cc42c2ee72f1a57a1e0f9402209c107e259f4
ms.sourcegitcommit: bdbc68ed8eaf43386d2cdf7b79e64ebbe1e860c0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/13/2019
ms.locfileid: "29967295"
---
# <a name="get-mailfolder"></a><span data-ttu-id="90edf-103">Obter mailFolder</span><span class="sxs-lookup"><span data-stu-id="90edf-103">Get mailFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90edf-104">Recupere as propriedades e os relacionamentos de um objeto da pasta de mensagens.</span><span class="sxs-lookup"><span data-stu-id="90edf-104">Retrieve the properties and relationships of a message folder object.</span></span>

<span data-ttu-id="90edf-105">Há dois cenários onde um aplicativo pode obter a pasta de correio de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="90edf-105">There are two scenarios where an app can get another user's mail folder:</span></span>

* <span data-ttu-id="90edf-106">Se o aplicativo tem permissões de aplicativo ou</span><span class="sxs-lookup"><span data-stu-id="90edf-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="90edf-107">Se o aplicativo tiver apropriada [permissões](#permissions) delegadas de um usuário, e outro usuário compartilhou uma pasta de email com que o usuário ou, tem acesso delegado a esse usuário.</span><span class="sxs-lookup"><span data-stu-id="90edf-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="90edf-108">Confira os [detalhes e um exemplo](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="90edf-108">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

## <a name="permissions"></a><span data-ttu-id="90edf-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="90edf-109">Permissions</span></span>

<span data-ttu-id="90edf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90edf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90edf-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="90edf-112">Permission type</span></span>      | <span data-ttu-id="90edf-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="90edf-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="90edf-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="90edf-114">Delegated (work or school account)</span></span> | <span data-ttu-id="90edf-115">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="90edf-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="90edf-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="90edf-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90edf-117">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="90edf-117">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="90edf-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="90edf-118">Application</span></span> | <span data-ttu-id="90edf-119">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="90edf-119">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="90edf-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="90edf-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="90edf-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="90edf-121">Optional query parameters</span></span>

<span data-ttu-id="90edf-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="90edf-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="90edf-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="90edf-123">Request headers</span></span>

| <span data-ttu-id="90edf-124">Nome</span><span class="sxs-lookup"><span data-stu-id="90edf-124">Name</span></span>          | <span data-ttu-id="90edf-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="90edf-125">Type</span></span>   | <span data-ttu-id="90edf-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="90edf-126">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="90edf-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="90edf-127">Authorization</span></span> | <span data-ttu-id="90edf-128">string</span><span class="sxs-lookup"><span data-stu-id="90edf-128">string</span></span> | <span data-ttu-id="90edf-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90edf-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="90edf-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="90edf-131">Request body</span></span>

<span data-ttu-id="90edf-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="90edf-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90edf-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="90edf-133">Response</span></span>

<span data-ttu-id="90edf-134">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [mailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="90edf-134">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="90edf-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="90edf-135">Examples</span></span>

### <a name="example-1-get-a-mail-folder"></a><span data-ttu-id="90edf-136">O exemplo 1: Obtenha uma pasta de email</span><span class="sxs-lookup"><span data-stu-id="90edf-136">Example 1: Get a mail folder</span></span>

#### <a name="request"></a><span data-ttu-id="90edf-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="90edf-137">Request</span></span>

<span data-ttu-id="90edf-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="90edf-138">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_mailfolder"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="90edf-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="90edf-139">Response</span></span>

<span data-ttu-id="90edf-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="90edf-140">The following is an example of the response.</span></span>

> <span data-ttu-id="90edf-141">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="90edf-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="90edf-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="90edf-142">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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

### <a name="example-2-get-a-mail-search-folder"></a><span data-ttu-id="90edf-143">Exemplo 2: Obter uma pasta de pesquisa de email</span><span class="sxs-lookup"><span data-stu-id="90edf-143">Example 2: Get a mail search folder</span></span>

#### <a name="request"></a><span data-ttu-id="90edf-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="90edf-144">Request</span></span>

<span data-ttu-id="90edf-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="90edf-145">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_mailSearchfolder"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzN
```

#### <a name="response"></a><span data-ttu-id="90edf-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="90edf-146">Response</span></span>

<span data-ttu-id="90edf-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="90edf-147">The following is an example of the response.</span></span>

> <span data-ttu-id="90edf-148">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="90edf-148">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="90edf-149">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="90edf-149">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.type": "#microsoft.graph.mailSearchFolder",
  "id": "AAMkAGVmMDEzN",
  "displayName": "Get MyAnalytics",
  "parentFolderId": "AAMkAGVmMDEzI",
  "childFolderCount": 0,
  "unreadItemCount": 6,
  "totalItemCount": 6,
  "wellKnownName": null,
  "isSupported": true,
  "includeNestedFolders": true,
  "sourceFolderIDs": [
    "AAMkAGVmMDEzM"
  ],
  "filterQuery": "contains(subject, 'MyAnalytics')"
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
