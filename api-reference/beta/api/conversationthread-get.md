---
title: Obter conversationThread
description: 'Obtenha um thread específico pertencente a um grupo. Você pode especificar a conversa pai e o thread ou, '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: f53afdd5416e2973c79ce3ec47e5101d3126d20f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32455605"
---
# <a name="get-conversationthread"></a><span data-ttu-id="1d464-104">Obter conversationThread</span><span class="sxs-lookup"><span data-stu-id="1d464-104">Get conversationThread</span></span>

<span data-ttu-id="1d464-p102">Obtenha um thread específico pertencente a um grupo. Você pode especificar a conversa pai e o thread ou apenas o thread, sem fazer referência à conversa pai.</span><span class="sxs-lookup"><span data-stu-id="1d464-p102">Get a specific thread that belongs to a group. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span> 
## <a name="permissions"></a><span data-ttu-id="1d464-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="1d464-107">Permissions</span></span>
<span data-ttu-id="1d464-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d464-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d464-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1d464-110">Permission type</span></span>      | <span data-ttu-id="1d464-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1d464-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d464-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1d464-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1d464-113">Group. ReadWrite. All, Group. Read. All</span><span class="sxs-lookup"><span data-stu-id="1d464-113">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="1d464-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1d464-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d464-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d464-115">Not supported.</span></span>    |
|<span data-ttu-id="1d464-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1d464-116">Application</span></span> | <span data-ttu-id="1d464-117">Group. ReadWrite. All, Group. Read. All</span><span class="sxs-lookup"><span data-stu-id="1d464-117">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1d464-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1d464-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
GET /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="1d464-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1d464-119">Optional query parameters</span></span>
<span data-ttu-id="1d464-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1d464-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1d464-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1d464-121">Request headers</span></span>
| <span data-ttu-id="1d464-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1d464-122">Header</span></span>       | <span data-ttu-id="1d464-123">Valor</span><span class="sxs-lookup"><span data-stu-id="1d464-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1d464-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="1d464-124">Authorization</span></span>  | <span data-ttu-id="1d464-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1d464-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1d464-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1d464-127">Request body</span></span>
<span data-ttu-id="1d464-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1d464-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d464-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d464-129">Response</span></span>

<span data-ttu-id="1d464-130">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [conversationThread](../resources/conversationthread.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1d464-130">If successful, this method returns a `200 OK` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1d464-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1d464-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1d464-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1d464-132">Request</span></span>
<span data-ttu-id="1d464-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1d464-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversationthread"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}
```
##### <a name="response"></a><span data-ttu-id="1d464-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d464-134">Response</span></span>
<span data-ttu-id="1d464-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1d464-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 419

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
  "lastDeliveredDateTime": "datetime-value",
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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get conversationThread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
