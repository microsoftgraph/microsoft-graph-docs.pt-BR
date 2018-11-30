---
title: Obter mailFolder
description: Recupere as propriedades e os relacionamentos de um objeto da pasta de mensagens.
ms.openlocfilehash: 394fe948b67dbfded176eff27aaa6222856e69ee
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006915"
---
# <a name="get-mailfolder"></a><span data-ttu-id="9e2c0-103">Obter mailFolder</span><span class="sxs-lookup"><span data-stu-id="9e2c0-103">Get mailFolder</span></span>

<span data-ttu-id="9e2c0-104">Recupere as propriedades e os relacionamentos de um objeto da pasta de mensagens.</span><span class="sxs-lookup"><span data-stu-id="9e2c0-104">Retrieve the properties and relationships of a message folder object.</span></span>

<span data-ttu-id="9e2c0-105">Há dois cenários onde um aplicativo pode obter a pasta de correio de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="9e2c0-105">There are two scenarios where an app can get another user's mail folder:</span></span>

* <span data-ttu-id="9e2c0-106">Se o aplicativo tem permissões de aplicativo, ou,</span><span class="sxs-lookup"><span data-stu-id="9e2c0-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="9e2c0-107">Se o aplicativo tiver apropriada [permissões](#permissions) delegadas de um usuário, e outro usuário compartilhou uma pasta de email com que o usuário ou, tem acesso delegado a esse usuário.</span><span class="sxs-lookup"><span data-stu-id="9e2c0-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="9e2c0-108">Consulte os [detalhes e um exemplo](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="9e2c0-108">See [details and an example](/graph/outlook-share-messages-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="9e2c0-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="9e2c0-109">Permissions</span></span>
<span data-ttu-id="9e2c0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e2c0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e2c0-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9e2c0-112">Permission type</span></span>      | <span data-ttu-id="9e2c0-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9e2c0-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e2c0-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9e2c0-114">Delegated (work or school account)</span></span> | <span data-ttu-id="9e2c0-115">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9e2c0-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9e2c0-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9e2c0-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e2c0-117">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9e2c0-117">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9e2c0-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9e2c0-118">Application</span></span> | <span data-ttu-id="9e2c0-119">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9e2c0-119">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9e2c0-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9e2c0-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9e2c0-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9e2c0-121">Optional query parameters</span></span>
<span data-ttu-id="9e2c0-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9e2c0-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9e2c0-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9e2c0-123">Request headers</span></span>
| <span data-ttu-id="9e2c0-124">Nome</span><span class="sxs-lookup"><span data-stu-id="9e2c0-124">Name</span></span>       | <span data-ttu-id="9e2c0-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e2c0-125">Type</span></span> | <span data-ttu-id="9e2c0-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e2c0-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9e2c0-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="9e2c0-127">Authorization</span></span>  | <span data-ttu-id="9e2c0-128">string</span><span class="sxs-lookup"><span data-stu-id="9e2c0-128">string</span></span>  | <span data-ttu-id="9e2c0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9e2c0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9e2c0-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9e2c0-131">Request body</span></span>
<span data-ttu-id="9e2c0-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9e2c0-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e2c0-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e2c0-133">Response</span></span>

<span data-ttu-id="9e2c0-134">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [mailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9e2c0-134">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9e2c0-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9e2c0-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9e2c0-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e2c0-136">Request</span></span>
<span data-ttu-id="9e2c0-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9e2c0-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailfolder"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="9e2c0-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e2c0-138">Response</span></span>
<span data-ttu-id="9e2c0-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9e2c0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
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
