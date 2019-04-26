---
title: Listar threads
description: Obtenha todos os threads em uma conversa de grupo.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 3a33038abbcdf32178612278dc7f0f029cfdde1f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33326685"
---
# <a name="list-threads"></a><span data-ttu-id="1c697-103">Listar threads</span><span class="sxs-lookup"><span data-stu-id="1c697-103">List threads</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c697-104">Obtém todos os threads em uma conversa de grupo.</span><span class="sxs-lookup"><span data-stu-id="1c697-104">Get all the threads in a group conversation.</span></span>
<span data-ttu-id="1c697-105">Observação: Você também pode [obter todos os threads de um grupo](group-list-threads.md).</span><span class="sxs-lookup"><span data-stu-id="1c697-105">Note: You can also [get all the threads of a group](group-list-threads.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="1c697-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1c697-106">Permissions</span></span>
<span data-ttu-id="1c697-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c697-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c697-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1c697-109">Permission type</span></span>      | <span data-ttu-id="1c697-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1c697-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c697-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1c697-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1c697-112">Group. ReadWrite. All, Group. Read. All</span><span class="sxs-lookup"><span data-stu-id="1c697-112">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="1c697-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1c697-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c697-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c697-114">Not supported.</span></span>    |
|<span data-ttu-id="1c697-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1c697-115">Application</span></span> | <span data-ttu-id="1c697-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c697-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c697-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c697-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}/threads
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1c697-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1c697-118">Optional query parameters</span></span>
<span data-ttu-id="1c697-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1c697-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1c697-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1c697-120">Request headers</span></span>
| <span data-ttu-id="1c697-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1c697-121">Header</span></span>       | <span data-ttu-id="1c697-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1c697-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1c697-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1c697-123">Authorization</span></span>  | <span data-ttu-id="1c697-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c697-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1c697-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1c697-126">Request body</span></span>
<span data-ttu-id="1c697-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1c697-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c697-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c697-128">Response</span></span>

<span data-ttu-id="1c697-129">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [conversationThread](../resources/conversationthread.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c697-129">If successful, this method returns a `200 OK` response code and collection of [conversationThread](../resources/conversationthread.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1c697-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1c697-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1c697-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c697-131">Request</span></span>
<span data-ttu-id="1c697-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c697-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_threads"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/conversations/{id}/threads
```
##### <a name="response"></a><span data-ttu-id="1c697-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c697-133">Response</span></span>
<span data-ttu-id="1c697-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1c697-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List threads",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
