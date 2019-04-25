---
title: Listar buckets
description: Recupere uma lista de objetos **plannerbucket** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 9c5da6e715ae49539a31078e1e9ece9c85e1d861
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32538978"
---
# <a name="list-buckets"></a><span data-ttu-id="fe4ea-103">Listar buckets</span><span class="sxs-lookup"><span data-stu-id="fe4ea-103">List buckets</span></span>

<span data-ttu-id="fe4ea-104">Recupere uma lista de objetos **plannerbucket** .</span><span class="sxs-lookup"><span data-stu-id="fe4ea-104">Retrieve a list of **plannerbucket** objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe4ea-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="fe4ea-105">Permissions</span></span>
<span data-ttu-id="fe4ea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe4ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe4ea-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fe4ea-108">Permission type</span></span>      | <span data-ttu-id="fe4ea-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fe4ea-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe4ea-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fe4ea-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fe4ea-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe4ea-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="fe4ea-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fe4ea-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe4ea-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe4ea-113">Not supported.</span></span>    |
|<span data-ttu-id="fe4ea-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fe4ea-114">Application</span></span> | <span data-ttu-id="fe4ea-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe4ea-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe4ea-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fe4ea-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/buckets
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fe4ea-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fe4ea-117">Optional query parameters</span></span>
<span data-ttu-id="fe4ea-118">Este método requer que o [filtro](https://developer.microsoft.com/graph/docs/concepts/query_parameters) de PlanID seja especificado.</span><span class="sxs-lookup"><span data-stu-id="fe4ea-118">This method requires planId [filter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to be specified.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fe4ea-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fe4ea-119">Request headers</span></span>
| <span data-ttu-id="fe4ea-120">Nome</span><span class="sxs-lookup"><span data-stu-id="fe4ea-120">Name</span></span>      |<span data-ttu-id="fe4ea-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe4ea-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fe4ea-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fe4ea-122">Authorization</span></span>  | <span data-ttu-id="fe4ea-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fe4ea-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fe4ea-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fe4ea-125">Request body</span></span>
<span data-ttu-id="fe4ea-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fe4ea-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe4ea-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe4ea-127">Response</span></span>

<span data-ttu-id="fe4ea-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [plannerBucket](../resources/plannerbucket.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fe4ea-128">If successful, this method returns a `200 OK` response code and collection of [plannerBucket](../resources/plannerbucket.md) objects in the response body.</span></span>

<span data-ttu-id="fe4ea-129">Este método pode retornar qualquer um dos [códigos de status http](/graph/errors).</span><span class="sxs-lookup"><span data-stu-id="fe4ea-129">This method can return any of the [HTTP status codes](/graph/errors).</span></span> <span data-ttu-id="fe4ea-130">Os erros mais comuns que os aplicativos devem lidar com esse método são as respostas 403 e 404.</span><span class="sxs-lookup"><span data-stu-id="fe4ea-130">The most common errors that apps should handle for this method are the 403 and 404 responses.</span></span> <span data-ttu-id="fe4ea-131">Para obter mais informações sobre esses erros, confira [condições de erro do planejador comum](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="fe4ea-131">For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="fe4ea-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fe4ea-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fe4ea-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fe4ea-133">Request</span></span>
<span data-ttu-id="fe4ea-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fe4ea-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_buckets"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/buckets
```
##### <a name="response"></a><span data-ttu-id="fe4ea-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe4ea-135">Response</span></span>
<span data-ttu-id="fe4ea-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fe4ea-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
