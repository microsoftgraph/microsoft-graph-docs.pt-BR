---
title: Obter conversationThread
description: 'Obtenha um thread específico pertencente a um grupo. Você pode especificar tanto a conversa pai e o thread, ou, '
localization_priority: Normal
ms.openlocfilehash: 8c9dce87a1e3a4a9fd07c97c1b472d2e4e57ffcc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854506"
---
# <a name="get-conversationthread"></a><span data-ttu-id="8e495-104">Obter conversationThread</span><span class="sxs-lookup"><span data-stu-id="8e495-104">Get conversationThread</span></span>

> <span data-ttu-id="8e495-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8e495-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8e495-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8e495-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8e495-p103">Obtenha um thread específico pertencente a um grupo. Você pode especificar a conversa pai e o thread ou apenas o thread, sem fazer referência à conversa pai.</span><span class="sxs-lookup"><span data-stu-id="8e495-p103">Get a specific thread that belongs to a group. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span> 
## <a name="permissions"></a><span data-ttu-id="8e495-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="8e495-109">Permissions</span></span>
<span data-ttu-id="8e495-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e495-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e495-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8e495-112">Permission type</span></span>      | <span data-ttu-id="8e495-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8e495-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e495-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8e495-114">Delegated (work or school account)</span></span> | <span data-ttu-id="8e495-115">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8e495-115">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="8e495-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8e495-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e495-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e495-117">Not supported.</span></span>    |
|<span data-ttu-id="8e495-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8e495-118">Application</span></span> | <span data-ttu-id="8e495-119">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8e495-119">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e495-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8e495-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
GET /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="8e495-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8e495-121">Optional query parameters</span></span>
<span data-ttu-id="8e495-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8e495-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8e495-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8e495-123">Request headers</span></span>
| <span data-ttu-id="8e495-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8e495-124">Header</span></span>       | <span data-ttu-id="8e495-125">Valor</span><span class="sxs-lookup"><span data-stu-id="8e495-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8e495-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="8e495-126">Authorization</span></span>  | <span data-ttu-id="8e495-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e495-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8e495-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8e495-129">Request body</span></span>
<span data-ttu-id="8e495-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8e495-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e495-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e495-131">Response</span></span>

<span data-ttu-id="8e495-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [conversationThread](../resources/conversationthread.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8e495-132">If successful, this method returns a `200 OK` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8e495-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8e495-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8e495-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e495-134">Request</span></span>
<span data-ttu-id="8e495-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e495-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversationthread"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/threads/{id}
```
##### <a name="response"></a><span data-ttu-id="8e495-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e495-136">Response</span></span>
<span data-ttu-id="8e495-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8e495-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
