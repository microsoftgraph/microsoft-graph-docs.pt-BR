---
title: Criar thread de chat
description: Crie um novo thread de chat no canal especificado ao fornecer as mensagens raiz.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: ef8d341310296c810c433a23f0d29be166ca47c5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511244"
---
# <a name="create-chat-thread"></a><span data-ttu-id="f0316-103">Criar thread de chat</span><span class="sxs-lookup"><span data-stu-id="f0316-103">Create chat thread</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0316-104">Crie um novo thread de chat no [canal especificado](../resources/channel.md) ao fornecer as mensagens raiz.</span><span class="sxs-lookup"><span data-stu-id="f0316-104">Create a new chat thread in the specified [channel](../resources/channel.md) by supplying the root messages.</span></span>

## <a name="permissions"></a><span data-ttu-id="f0316-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f0316-105">Permissions</span></span>
<span data-ttu-id="f0316-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0316-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0316-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f0316-108">Permission type</span></span>      | <span data-ttu-id="f0316-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f0316-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0316-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f0316-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f0316-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0316-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f0316-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f0316-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0316-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0316-113">Not supported.</span></span>    |
|<span data-ttu-id="f0316-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0316-114">Application</span></span> | <span data-ttu-id="f0316-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0316-115">Not supported.</span></span> |

> <span data-ttu-id="f0316-116">Atualmente, há suporte apenas para [permissões delegadas](/graph/permissions-reference) para essa operação.</span><span class="sxs-lookup"><span data-stu-id="f0316-116">Currently, only [delegated permissions](/graph/permissions-reference) are supported for this operation.</span></span>  <span data-ttu-id="f0316-117">Versões futuras terão suporte para permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f0316-117">Future releases will support application permissions.</span></span> 

## <a name="http-request"></a><span data-ttu-id="f0316-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f0316-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/chatThreads
```
## <a name="request-headers"></a><span data-ttu-id="f0316-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f0316-119">Request headers</span></span>
| <span data-ttu-id="f0316-120">Nome</span><span class="sxs-lookup"><span data-stu-id="f0316-120">Name</span></span>       | <span data-ttu-id="f0316-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0316-121">Type</span></span> | <span data-ttu-id="f0316-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0316-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f0316-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f0316-123">Authorization</span></span>  | <span data-ttu-id="f0316-124">string</span><span class="sxs-lookup"><span data-stu-id="f0316-124">string</span></span>  | <span data-ttu-id="f0316-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f0316-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f0316-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f0316-127">Request body</span></span>
<span data-ttu-id="f0316-128">No corpo da solicitação, fornece uma representação JSON de um objeto [chatThread](../resources/chatthread.md) que contém a propriedade rootMessage.</span><span class="sxs-lookup"><span data-stu-id="f0316-128">In the request body, supply a JSON representation of a [chatThread](../resources/chatthread.md) object that contains the rootMessage property.</span></span>

## <a name="response"></a><span data-ttu-id="f0316-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0316-129">Response</span></span>

<span data-ttu-id="f0316-130">Se bem-sucedido, esse método retornará um código de resposta `201 Created` com um corpo de resposta vazio.</span><span class="sxs-lookup"><span data-stu-id="f0316-130">If successful, this method returns a `201 Created` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0316-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f0316-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f0316-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0316-132">Request</span></span>
<span data-ttu-id="f0316-133">Eis um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f0316-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chatthread_from_channel"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/chatThreads
Content-type: application/json

{
  "rootMessage": {
      "body": {
        "contentType": 1,
        "content": "<h1>Hello world</h1>"
      }
  }
}
```

> <span data-ttu-id="f0316-134">Atualmente, o contentType deve ser especificado como um inteiro em vez de uma cadeia de caracteres: 0 para “texto” ou 1 para “html”.</span><span class="sxs-lookup"><span data-stu-id="f0316-134">Currently, the contentType must be specified as an integer rather than a string: 0 for "text" or 1 for "html".</span></span>  <span data-ttu-id="f0316-135">As versões futuras da API corrigirão isso.</span><span class="sxs-lookup"><span data-stu-id="f0316-135">Future API releases will fix this.</span></span>

##### <a name="response"></a><span data-ttu-id="f0316-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0316-136">Response</span></span>

<span data-ttu-id="f0316-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f0316-137">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatThread"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 160

{
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-post-chatthreads.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
