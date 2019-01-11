---
title: Listar threads
description: Obtém todos os threads em uma conversa de grupo.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: e1aacab39dfeae4dd9271ce5f3664c55eb80a583
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813304"
---
# <a name="list-threads"></a><span data-ttu-id="8826b-103">Listar threads</span><span class="sxs-lookup"><span data-stu-id="8826b-103">List threads</span></span>

> <span data-ttu-id="8826b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8826b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8826b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8826b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8826b-106">Obtém todos os threads em uma conversa de grupo.</span><span class="sxs-lookup"><span data-stu-id="8826b-106">Get all the threads in a group conversation.</span></span>
<span data-ttu-id="8826b-107">Observação: Você também pode [obter todos os threads de um grupo](group-list-threads.md).</span><span class="sxs-lookup"><span data-stu-id="8826b-107">Note: You can also [get all the threads of a group](group-list-threads.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="8826b-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="8826b-108">Permissions</span></span>
<span data-ttu-id="8826b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8826b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8826b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8826b-111">Permission type</span></span>      | <span data-ttu-id="8826b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8826b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8826b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8826b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="8826b-114">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8826b-114">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="8826b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8826b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8826b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8826b-116">Not supported.</span></span>    |
|<span data-ttu-id="8826b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8826b-117">Application</span></span> | <span data-ttu-id="8826b-118">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8826b-118">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8826b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8826b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}/threads
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8826b-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8826b-120">Optional query parameters</span></span>
<span data-ttu-id="8826b-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8826b-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8826b-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8826b-122">Request headers</span></span>
| <span data-ttu-id="8826b-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8826b-123">Header</span></span>       | <span data-ttu-id="8826b-124">Valor</span><span class="sxs-lookup"><span data-stu-id="8826b-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8826b-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="8826b-125">Authorization</span></span>  | <span data-ttu-id="8826b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8826b-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8826b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8826b-128">Request body</span></span>
<span data-ttu-id="8826b-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8826b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8826b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="8826b-130">Response</span></span>

<span data-ttu-id="8826b-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [conversationThread](../resources/conversationthread.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8826b-131">If successful, this method returns a `200 OK` response code and collection of [conversationThread](../resources/conversationthread.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8826b-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8826b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8826b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8826b-133">Request</span></span>
<span data-ttu-id="8826b-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8826b-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_threads"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/conversations/{id}/threads
```
##### <a name="response"></a><span data-ttu-id="8826b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="8826b-135">Response</span></span>
<span data-ttu-id="8826b-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8826b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List threads",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
