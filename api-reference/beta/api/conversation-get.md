---
title: Obter conversa
description: Recuperar as propriedades e os relacionamentos do objeto conversation.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 08059625838d6a60489820b2369768c6a3fca071
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931717"
---
# <a name="get-conversation"></a><span data-ttu-id="2ae8e-103">Obter conversation</span><span class="sxs-lookup"><span data-stu-id="2ae8e-103">Get conversation</span></span>

> <span data-ttu-id="2ae8e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2ae8e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2ae8e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2ae8e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2ae8e-106">Recuperar as propriedades e os relacionamentos do objeto conversation.</span><span class="sxs-lookup"><span data-stu-id="2ae8e-106">Retrieve the properties and relationships of conversation object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2ae8e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="2ae8e-107">Permissions</span></span>
<span data-ttu-id="2ae8e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ae8e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ae8e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2ae8e-110">Permission type</span></span>      | <span data-ttu-id="2ae8e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2ae8e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ae8e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2ae8e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2ae8e-113">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ae8e-113">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="2ae8e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2ae8e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ae8e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ae8e-115">Not supported.</span></span>    |
|<span data-ttu-id="2ae8e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2ae8e-116">Application</span></span> | <span data-ttu-id="2ae8e-117">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ae8e-117">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ae8e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ae8e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="2ae8e-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2ae8e-119">Optional query parameters</span></span>
<span data-ttu-id="2ae8e-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2ae8e-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2ae8e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2ae8e-121">Request headers</span></span>
| <span data-ttu-id="2ae8e-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2ae8e-122">Header</span></span>       | <span data-ttu-id="2ae8e-123">Valor</span><span class="sxs-lookup"><span data-stu-id="2ae8e-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2ae8e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="2ae8e-124">Authorization</span></span>  | <span data-ttu-id="2ae8e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ae8e-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2ae8e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2ae8e-127">Request body</span></span>
<span data-ttu-id="2ae8e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2ae8e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ae8e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ae8e-129">Response</span></span>

<span data-ttu-id="2ae8e-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [conversation](../resources/conversation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2ae8e-130">If successful, this method returns a `200 OK` response code and [conversation](../resources/conversation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2ae8e-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2ae8e-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2ae8e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ae8e-132">Request</span></span>
<span data-ttu-id="2ae8e-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2ae8e-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversation"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/conversations/{id}
```
##### <a name="response"></a><span data-ttu-id="2ae8e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ae8e-134">Response</span></span>
<span data-ttu-id="2ae8e-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2ae8e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
