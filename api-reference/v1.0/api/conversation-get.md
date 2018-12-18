---
title: Obter conversa
description: Recuperar as propriedades e os relacionamentos do objeto conversation.
author: dkershaw10
ms.openlocfilehash: 505ea763be6c9a29cad962939ed59ff3e72f2b2e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27363680"
---
# <a name="get-conversation"></a><span data-ttu-id="88d11-103">Obter conversa</span><span class="sxs-lookup"><span data-stu-id="88d11-103">Get conversation</span></span>

<span data-ttu-id="88d11-104">Recuperar as propriedades e os relacionamentos do objeto conversation.</span><span class="sxs-lookup"><span data-stu-id="88d11-104">Retrieve the properties and relationships of conversation object.</span></span>
## <a name="permissions"></a><span data-ttu-id="88d11-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="88d11-105">Permissions</span></span>
<span data-ttu-id="88d11-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88d11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88d11-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="88d11-108">Permission type</span></span>      | <span data-ttu-id="88d11-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="88d11-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="88d11-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="88d11-110">Delegated (work or school account)</span></span> | <span data-ttu-id="88d11-111">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="88d11-111">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="88d11-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="88d11-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88d11-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="88d11-113">Not supported.</span></span>    |
|<span data-ttu-id="88d11-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="88d11-114">Application</span></span> | <span data-ttu-id="88d11-115">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="88d11-115">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="88d11-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="88d11-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="88d11-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="88d11-117">Optional query parameters</span></span>
<span data-ttu-id="88d11-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="88d11-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="88d11-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="88d11-119">Request headers</span></span>
| <span data-ttu-id="88d11-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="88d11-120">Header</span></span>       | <span data-ttu-id="88d11-121">Valor</span><span class="sxs-lookup"><span data-stu-id="88d11-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="88d11-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="88d11-122">Authorization</span></span>  | <span data-ttu-id="88d11-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="88d11-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="88d11-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="88d11-125">Request body</span></span>
<span data-ttu-id="88d11-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="88d11-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88d11-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="88d11-127">Response</span></span>

<span data-ttu-id="88d11-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [conversation](../resources/conversation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="88d11-128">If successful, this method returns a `200 OK` response code and [conversation](../resources/conversation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="88d11-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="88d11-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="88d11-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="88d11-130">Request</span></span>
<span data-ttu-id="88d11-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="88d11-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversation"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}
```
##### <a name="response"></a><span data-ttu-id="88d11-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="88d11-132">Response</span></span>
<span data-ttu-id="88d11-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="88d11-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "lastDeliveredDateTime": "datetime-value",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "preview": "preview-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
