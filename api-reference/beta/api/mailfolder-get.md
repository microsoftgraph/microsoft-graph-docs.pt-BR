---
title: Obter mailFolder
description: Recupere as propriedades e os relacionamentos de um objeto da pasta de mensagens.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 8301f5ff1cef7602b3e9d488c67daec8ac277cce
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856642"
---
# <a name="get-mailfolder"></a><span data-ttu-id="ce660-103">Obter mailFolder</span><span class="sxs-lookup"><span data-stu-id="ce660-103">Get mailFolder</span></span>

> <span data-ttu-id="ce660-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ce660-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ce660-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ce660-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ce660-106">Recupere as propriedades e os relacionamentos de um objeto da pasta de mensagens.</span><span class="sxs-lookup"><span data-stu-id="ce660-106">Retrieve the properties and relationships of a message folder object.</span></span>

<span data-ttu-id="ce660-107">Há dois cenários onde um aplicativo pode obter a pasta de correio de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="ce660-107">There are two scenarios where an app can get another user's mail folder:</span></span>

* <span data-ttu-id="ce660-108">Se o aplicativo tem permissões de aplicativo, ou,</span><span class="sxs-lookup"><span data-stu-id="ce660-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="ce660-109">Se o aplicativo tiver apropriada [permissões](#permissions) delegadas de um usuário, e outro usuário compartilhou uma pasta de email com que o usuário ou, tem acesso delegado a esse usuário.</span><span class="sxs-lookup"><span data-stu-id="ce660-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="ce660-110">Consulte os [detalhes e um exemplo](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="ce660-110">See [details and an example](/graph/outlook-share-messages-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="ce660-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="ce660-111">Permissions</span></span>
<span data-ttu-id="ce660-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce660-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce660-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ce660-114">Permission type</span></span>      | <span data-ttu-id="ce660-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ce660-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce660-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ce660-116">Delegated (work or school account)</span></span> | <span data-ttu-id="ce660-117">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ce660-117">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ce660-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ce660-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce660-119">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ce660-119">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ce660-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ce660-120">Application</span></span> | <span data-ttu-id="ce660-121">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ce660-121">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce660-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ce660-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ce660-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ce660-123">Optional query parameters</span></span>
<span data-ttu-id="ce660-124">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ce660-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ce660-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ce660-125">Request headers</span></span>
| <span data-ttu-id="ce660-126">Nome</span><span class="sxs-lookup"><span data-stu-id="ce660-126">Name</span></span>       | <span data-ttu-id="ce660-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce660-127">Type</span></span> | <span data-ttu-id="ce660-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce660-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ce660-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="ce660-129">Authorization</span></span>  | <span data-ttu-id="ce660-130">string</span><span class="sxs-lookup"><span data-stu-id="ce660-130">string</span></span>  | <span data-ttu-id="ce660-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ce660-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ce660-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ce660-133">Request body</span></span>
<span data-ttu-id="ce660-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ce660-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce660-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce660-135">Response</span></span>
<span data-ttu-id="ce660-136">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [mailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ce660-136">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example-1"></a><span data-ttu-id="ce660-137">Exemplo 1</span><span class="sxs-lookup"><span data-stu-id="ce660-137">Example 1</span></span>
#### <a name="request-1"></a><span data-ttu-id="ce660-138">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="ce660-138">Request 1</span></span>
<span data-ttu-id="ce660-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ce660-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailfolder"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
```

#### <a name="response-1"></a><span data-ttu-id="ce660-140">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="ce660-140">Response 1</span></span>
<span data-ttu-id="ce660-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ce660-141">The following is an example of the response.</span></span>
 ><span data-ttu-id="ce660-142">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ce660-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ce660-143">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ce660-143">All the properties will be returned from an actual call.</span></span>
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

## <a name="example-2"></a><span data-ttu-id="ce660-144">Exemplo 2</span><span class="sxs-lookup"><span data-stu-id="ce660-144">Example 2</span></span>
#### <a name="request-2"></a><span data-ttu-id="ce660-145">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="ce660-145">Request 2</span></span>
<span data-ttu-id="ce660-146">O exemplo a seguir é um exemplo de pasta de pesquisa da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ce660-146">The following is a search folder example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailSearchfolder"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
```

#### <a name="response-2"></a><span data-ttu-id="ce660-147">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="ce660-147">Response 2</span></span>
<span data-ttu-id="ce660-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ce660-148">The following is an example of the response.</span></span>
 ><span data-ttu-id="ce660-149">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ce660-149">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ce660-150">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ce660-150">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
