---
title: Obter conversationThread
description: 'Obtenha um thread específico pertencente a um grupo. Você pode especificar tanto a conversa pai e o thread, ou, '
localization_priority: Normal
ms.openlocfilehash: 61ec38651274cf71e87f362927de66873a6cca24
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894237"
---
# <a name="get-conversationthread"></a><span data-ttu-id="cf7f0-104">Obter conversationThread</span><span class="sxs-lookup"><span data-stu-id="cf7f0-104">Get conversationThread</span></span>

<span data-ttu-id="cf7f0-p102">Obtenha um thread específico pertencente a um grupo. Você pode especificar a conversa pai e o thread ou apenas o thread, sem fazer referência à conversa pai.</span><span class="sxs-lookup"><span data-stu-id="cf7f0-p102">Get a specific thread that belongs to a group. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span> 
## <a name="permissions"></a><span data-ttu-id="cf7f0-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="cf7f0-107">Permissions</span></span>
<span data-ttu-id="cf7f0-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf7f0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf7f0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cf7f0-110">Permission type</span></span>      | <span data-ttu-id="cf7f0-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cf7f0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf7f0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cf7f0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cf7f0-113">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf7f0-113">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="cf7f0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cf7f0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf7f0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf7f0-115">Not supported.</span></span>    |
|<span data-ttu-id="cf7f0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cf7f0-116">Application</span></span> | <span data-ttu-id="cf7f0-117">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf7f0-117">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cf7f0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cf7f0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
GET /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="cf7f0-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cf7f0-119">Optional query parameters</span></span>
<span data-ttu-id="cf7f0-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cf7f0-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="cf7f0-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cf7f0-121">Request headers</span></span>
| <span data-ttu-id="cf7f0-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cf7f0-122">Header</span></span>       | <span data-ttu-id="cf7f0-123">Valor</span><span class="sxs-lookup"><span data-stu-id="cf7f0-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cf7f0-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="cf7f0-124">Authorization</span></span>  | <span data-ttu-id="cf7f0-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cf7f0-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cf7f0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cf7f0-127">Request body</span></span>
<span data-ttu-id="cf7f0-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cf7f0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf7f0-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf7f0-129">Response</span></span>

<span data-ttu-id="cf7f0-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [conversationThread](../resources/conversationthread.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cf7f0-130">If successful, this method returns a `200 OK` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cf7f0-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cf7f0-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cf7f0-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cf7f0-132">Request</span></span>
<span data-ttu-id="cf7f0-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cf7f0-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversationthread"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}
```
##### <a name="response"></a><span data-ttu-id="cf7f0-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf7f0-134">Response</span></span>
<span data-ttu-id="cf7f0-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cf7f0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
