---
title: Listar conversas
description: Recupere a lista de conversas desse grupo.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 4a548144e7db3cd3bf7732437784fd8fa51a21f2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985337"
---
# <a name="list-conversations"></a><span data-ttu-id="3e6c1-103">Listar conversas</span><span class="sxs-lookup"><span data-stu-id="3e6c1-103">List conversations</span></span>

> <span data-ttu-id="3e6c1-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3e6c1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3e6c1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3e6c1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3e6c1-106">Recupere a lista de [conversas](../resources/conversation.md) desse grupo.</span><span class="sxs-lookup"><span data-stu-id="3e6c1-106">Retrieve the list of [conversations](../resources/conversation.md) in this group.</span></span>

## <a name="permissions"></a><span data-ttu-id="3e6c1-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="3e6c1-107">Permissions</span></span>
<span data-ttu-id="3e6c1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e6c1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e6c1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3e6c1-110">Permission type</span></span>      | <span data-ttu-id="3e6c1-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3e6c1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e6c1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3e6c1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3e6c1-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e6c1-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3e6c1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3e6c1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e6c1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e6c1-115">Not supported.</span></span>    |
|<span data-ttu-id="3e6c1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3e6c1-116">Application</span></span> | <span data-ttu-id="3e6c1-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e6c1-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e6c1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3e6c1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3e6c1-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3e6c1-119">Optional query parameters</span></span>
<span data-ttu-id="3e6c1-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3e6c1-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3e6c1-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3e6c1-121">Request headers</span></span>
| <span data-ttu-id="3e6c1-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3e6c1-122">Header</span></span>       | <span data-ttu-id="3e6c1-123">Valor</span><span class="sxs-lookup"><span data-stu-id="3e6c1-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3e6c1-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="3e6c1-124">Authorization</span></span>  | <span data-ttu-id="3e6c1-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3e6c1-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3e6c1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3e6c1-127">Request body</span></span>
<span data-ttu-id="3e6c1-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3e6c1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e6c1-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e6c1-129">Response</span></span>
<span data-ttu-id="3e6c1-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [conversation](../resources/conversation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3e6c1-130">If successful, this method returns a `200 OK` response code and collection of [conversation](../resources/conversation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e6c1-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3e6c1-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="3e6c1-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3e6c1-132">Request</span></span>
<span data-ttu-id="3e6c1-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3e6c1-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversations"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/conversations
```

#### <a name="response"></a><span data-ttu-id="3e6c1-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e6c1-134">Response</span></span>
<span data-ttu-id="3e6c1-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3e6c1-135">The following is an example of the response.</span></span>
><span data-ttu-id="3e6c1-136">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3e6c1-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3e6c1-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3e6c1-137">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 262

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List conversations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
