---
title: Listar threads
description: Obter todos os threads de um grupo.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: a4d0e0404828bda0aebe745d0b6413963d79a7ac
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32502077"
---
# <a name="list-threads"></a><span data-ttu-id="1cb02-103">Listar threads</span><span class="sxs-lookup"><span data-stu-id="1cb02-103">List threads</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1cb02-104">Obter todos os threads de um grupo.</span><span class="sxs-lookup"><span data-stu-id="1cb02-104">Get all the threads of a group.</span></span>

<span data-ttu-id="1cb02-105">Observação: você também pode [obter todos os threads de uma conversa](conversation-list-threads.md).</span><span class="sxs-lookup"><span data-stu-id="1cb02-105">Note: You can also [get all the threads of a conversation](conversation-list-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1cb02-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1cb02-106">Permissions</span></span>
<span data-ttu-id="1cb02-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1cb02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1cb02-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1cb02-109">Permission type</span></span>      | <span data-ttu-id="1cb02-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1cb02-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1cb02-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1cb02-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1cb02-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cb02-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1cb02-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1cb02-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1cb02-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1cb02-114">Not supported.</span></span>    |
|<span data-ttu-id="1cb02-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1cb02-115">Application</span></span> | <span data-ttu-id="1cb02-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1cb02-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1cb02-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1cb02-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1cb02-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1cb02-118">Optional query parameters</span></span>
<span data-ttu-id="1cb02-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1cb02-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1cb02-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1cb02-120">Request headers</span></span>
| <span data-ttu-id="1cb02-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1cb02-121">Header</span></span>       | <span data-ttu-id="1cb02-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1cb02-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1cb02-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1cb02-123">Authorization</span></span>  | <span data-ttu-id="1cb02-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1cb02-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1cb02-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1cb02-126">Request body</span></span>
<span data-ttu-id="1cb02-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1cb02-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1cb02-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cb02-128">Response</span></span>
<span data-ttu-id="1cb02-129">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [conversationThread](../resources/conversationthread.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1cb02-129">If successful, this method returns a `200 OK` response code and collection of [conversationThread](../resources/conversationthread.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1cb02-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1cb02-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="1cb02-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1cb02-131">Request</span></span>
<span data-ttu-id="1cb02-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1cb02-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_threads"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/threads
```

#### <a name="response"></a><span data-ttu-id="1cb02-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cb02-133">Response</span></span>
<span data-ttu-id="1cb02-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1cb02-134">The following is an example of the response.</span></span>
><span data-ttu-id="1cb02-135">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1cb02-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1cb02-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1cb02-136">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 536

{
  "value": [
    {
      "toRecipients": [
        {
          "emailAddress": {
            "name": "name-value",
            "address": "address-value"
          }
        }
      ],
      "topic": "topic-value",
      "hasAttachments": true,
      "lastDeliveredDateTime": "2016-10-19T10:37:00Z",
      "uniqueSenders": [
        "uniqueSenders-value"
      ],
      "ccRecipients": [
        {
          "emailAddress": {
            "name": "name-value",
            "address": "address-value"
          }
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List group threads",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-list-threads.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
