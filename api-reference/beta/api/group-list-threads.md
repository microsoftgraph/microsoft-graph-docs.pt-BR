---
title: Listar threads
description: Obter todos os threads de um grupo.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: a79a6fc2568ae550d2323a401c4e0fd22b6d9b09
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984495"
---
# <a name="list-threads"></a><span data-ttu-id="c28d1-103">Listar threads</span><span class="sxs-lookup"><span data-stu-id="c28d1-103">List threads</span></span>

> <span data-ttu-id="c28d1-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c28d1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c28d1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c28d1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c28d1-106">Obter todos os threads de um grupo.</span><span class="sxs-lookup"><span data-stu-id="c28d1-106">Get all the threads of a group.</span></span>

<span data-ttu-id="c28d1-107">Observação: você também pode [obter todos os threads de uma conversa](conversation-list-threads.md).</span><span class="sxs-lookup"><span data-stu-id="c28d1-107">Note: You can also [get all the threads of a conversation](conversation-list-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c28d1-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="c28d1-108">Permissions</span></span>
<span data-ttu-id="c28d1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c28d1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c28d1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c28d1-111">Permission type</span></span>      | <span data-ttu-id="c28d1-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c28d1-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c28d1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c28d1-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c28d1-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c28d1-114">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c28d1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c28d1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c28d1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c28d1-116">Not supported.</span></span>    |
|<span data-ttu-id="c28d1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c28d1-117">Application</span></span> | <span data-ttu-id="c28d1-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c28d1-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c28d1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c28d1-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c28d1-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c28d1-120">Optional query parameters</span></span>
<span data-ttu-id="c28d1-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c28d1-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c28d1-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c28d1-122">Request headers</span></span>
| <span data-ttu-id="c28d1-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c28d1-123">Header</span></span>       | <span data-ttu-id="c28d1-124">Valor</span><span class="sxs-lookup"><span data-stu-id="c28d1-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c28d1-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c28d1-125">Authorization</span></span>  | <span data-ttu-id="c28d1-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c28d1-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c28d1-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c28d1-128">Request body</span></span>
<span data-ttu-id="c28d1-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c28d1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c28d1-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c28d1-130">Response</span></span>
<span data-ttu-id="c28d1-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [conversationThread](../resources/conversationthread.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c28d1-131">If successful, this method returns a `200 OK` response code and collection of [conversationThread](../resources/conversationthread.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c28d1-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c28d1-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c28d1-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c28d1-133">Request</span></span>
<span data-ttu-id="c28d1-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c28d1-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_threads"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/threads
```

#### <a name="response"></a><span data-ttu-id="c28d1-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c28d1-135">Response</span></span>
<span data-ttu-id="c28d1-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c28d1-136">The following is an example of the response.</span></span>
><span data-ttu-id="c28d1-137">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c28d1-137">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c28d1-138">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c28d1-138">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List group threads",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
