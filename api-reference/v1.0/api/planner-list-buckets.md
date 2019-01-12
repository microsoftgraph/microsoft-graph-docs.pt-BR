---
title: Listar buckets
description: Recupere uma lista de objetos **plannerbucket**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 5a5115b7afffebcf663b01c3836ba718d896098e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27958219"
---
# <a name="list-buckets"></a><span data-ttu-id="1b2e2-103">Listar buckets</span><span class="sxs-lookup"><span data-stu-id="1b2e2-103">List buckets</span></span>

<span data-ttu-id="1b2e2-104">Recupere uma lista de objetos **plannerbucket**.</span><span class="sxs-lookup"><span data-stu-id="1b2e2-104">Retrieve a list of **plannerbucket** objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b2e2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="1b2e2-105">Permissions</span></span>
<span data-ttu-id="1b2e2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b2e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b2e2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1b2e2-108">Permission type</span></span>      | <span data-ttu-id="1b2e2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1b2e2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b2e2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1b2e2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1b2e2-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b2e2-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1b2e2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1b2e2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b2e2-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b2e2-113">Not supported.</span></span>    |
|<span data-ttu-id="1b2e2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1b2e2-114">Application</span></span> | <span data-ttu-id="1b2e2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b2e2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b2e2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1b2e2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/buckets
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1b2e2-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1b2e2-117">Optional query parameters</span></span>
<span data-ttu-id="1b2e2-118">Este método requer que o [filtro](https://developer.microsoft.com/graph/docs/concepts/query_parameters) de planId seja especificado.</span><span class="sxs-lookup"><span data-stu-id="1b2e2-118">This method requires planId [filter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to be specified.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1b2e2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1b2e2-119">Request headers</span></span>
| <span data-ttu-id="1b2e2-120">Nome</span><span class="sxs-lookup"><span data-stu-id="1b2e2-120">Name</span></span>      |<span data-ttu-id="1b2e2-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b2e2-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1b2e2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1b2e2-122">Authorization</span></span>  | <span data-ttu-id="1b2e2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b2e2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1b2e2-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1b2e2-125">Request body</span></span>
<span data-ttu-id="1b2e2-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1b2e2-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1b2e2-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b2e2-127">Response</span></span>

<span data-ttu-id="1b2e2-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [plannerBucket](../resources/plannerbucket.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1b2e2-128">If successful, this method returns a `200 OK` response code and collection of [plannerBucket](../resources/plannerbucket.md) objects in the response body.</span></span>

<span data-ttu-id="1b2e2-p103">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="1b2e2-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="1b2e2-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1b2e2-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1b2e2-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1b2e2-133">Request</span></span>
<span data-ttu-id="1b2e2-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1b2e2-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_buckets"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/buckets
```
##### <a name="response"></a><span data-ttu-id="1b2e2-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b2e2-135">Response</span></span>
<span data-ttu-id="1b2e2-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1b2e2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucket",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

{
  "value": [
    {
      "@odata.etag": "W/\"JzEtQnVja2V0QEBAQEBAQEBAQEBAQEBARCc=\"",
      "name": "To do",
      "planId": "2txjA-BMZEq-bKi6Wfj5aGQAB1OJ",
      "orderHint": "85752723360752+",
      "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List buckets",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
