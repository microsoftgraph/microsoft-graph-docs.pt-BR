---
title: Listar threads
description: Obtém todos os threads em uma conversa de grupo.
ms.openlocfilehash: 85d694261b71e0aa6eb68d9c2e2db00794c20f4c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037789"
---
# <a name="list-threads"></a><span data-ttu-id="05c38-103">Listar threads</span><span class="sxs-lookup"><span data-stu-id="05c38-103">List threads</span></span>

> <span data-ttu-id="05c38-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="05c38-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="05c38-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="05c38-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="05c38-106">Obtém todos os threads em uma conversa de grupo.</span><span class="sxs-lookup"><span data-stu-id="05c38-106">Get all the threads in a group conversation.</span></span>
<span data-ttu-id="05c38-107">Observação: Você também pode [obter todos os threads de um grupo](group-list-threads.md).</span><span class="sxs-lookup"><span data-stu-id="05c38-107">Note: You can also [get all the threads of a group](group-list-threads.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="05c38-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="05c38-108">Permissions</span></span>
<span data-ttu-id="05c38-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05c38-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05c38-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="05c38-111">Permission type</span></span>      | <span data-ttu-id="05c38-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="05c38-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="05c38-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="05c38-113">Delegated (work or school account)</span></span> | <span data-ttu-id="05c38-114">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="05c38-114">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="05c38-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="05c38-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05c38-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05c38-116">Not supported.</span></span>    |
|<span data-ttu-id="05c38-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="05c38-117">Application</span></span> | <span data-ttu-id="05c38-118">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="05c38-118">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="05c38-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="05c38-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}/threads
```
## <a name="optional-query-parameters"></a><span data-ttu-id="05c38-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="05c38-120">Optional query parameters</span></span>
<span data-ttu-id="05c38-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="05c38-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="05c38-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="05c38-122">Request headers</span></span>
| <span data-ttu-id="05c38-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="05c38-123">Header</span></span>       | <span data-ttu-id="05c38-124">Valor</span><span class="sxs-lookup"><span data-stu-id="05c38-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="05c38-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="05c38-125">Authorization</span></span>  | <span data-ttu-id="05c38-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="05c38-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="05c38-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="05c38-128">Request body</span></span>
<span data-ttu-id="05c38-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="05c38-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="05c38-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="05c38-130">Response</span></span>

<span data-ttu-id="05c38-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [conversationThread](../resources/conversationthread.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="05c38-131">If successful, this method returns a `200 OK` response code and collection of [conversationThread](../resources/conversationthread.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="05c38-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="05c38-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="05c38-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="05c38-133">Request</span></span>
<span data-ttu-id="05c38-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="05c38-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_threads"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/conversations/{id}/threads
```
##### <a name="response"></a><span data-ttu-id="05c38-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="05c38-135">Response</span></span>
<span data-ttu-id="05c38-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="05c38-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
