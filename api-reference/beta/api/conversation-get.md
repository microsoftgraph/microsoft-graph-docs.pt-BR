---
title: Obter conversa
description: Recuperar as propriedades e os relacionamentos do objeto conversation.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 781bb0ff01a2c5efb469e91824a7ee9c3b5036cd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507870"
---
# <a name="get-conversation"></a><span data-ttu-id="b3e3b-103">Obter conversa</span><span class="sxs-lookup"><span data-stu-id="b3e3b-103">Get conversation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3e3b-104">Recuperar as propriedades e os relacionamentos do objeto conversation.</span><span class="sxs-lookup"><span data-stu-id="b3e3b-104">Retrieve the properties and relationships of conversation object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b3e3b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b3e3b-105">Permissions</span></span>
<span data-ttu-id="b3e3b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3e3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3e3b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b3e3b-108">Permission type</span></span>      | <span data-ttu-id="b3e3b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b3e3b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3e3b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b3e3b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b3e3b-111">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="b3e3b-111">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="b3e3b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b3e3b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3e3b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3e3b-113">Not supported.</span></span>    |
|<span data-ttu-id="b3e3b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b3e3b-114">Application</span></span> | <span data-ttu-id="b3e3b-115">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="b3e3b-115">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3e3b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b3e3b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="b3e3b-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b3e3b-117">Optional query parameters</span></span>
<span data-ttu-id="b3e3b-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b3e3b-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b3e3b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b3e3b-119">Request headers</span></span>
| <span data-ttu-id="b3e3b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b3e3b-120">Header</span></span>       | <span data-ttu-id="b3e3b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b3e3b-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b3e3b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b3e3b-122">Authorization</span></span>  | <span data-ttu-id="b3e3b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3e3b-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b3e3b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b3e3b-125">Request body</span></span>
<span data-ttu-id="b3e3b-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b3e3b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3e3b-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3e3b-127">Response</span></span>

<span data-ttu-id="b3e3b-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [conversation](../resources/conversation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b3e3b-128">If successful, this method returns a `200 OK` response code and [conversation](../resources/conversation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b3e3b-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b3e3b-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b3e3b-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b3e3b-130">Request</span></span>
<span data-ttu-id="b3e3b-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b3e3b-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversation"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/conversations/{id}
```
##### <a name="response"></a><span data-ttu-id="b3e3b-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3e3b-132">Response</span></span>
<span data-ttu-id="b3e3b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b3e3b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "2016-10-19T10:37:00Z",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "preview": "preview-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/conversation-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
