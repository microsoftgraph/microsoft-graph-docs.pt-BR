---
title: Listar buckets
description: Recupere uma lista de objetos **plannerbucket**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: c0648d659dbb33c3e7d51b38999648637721ca7b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928728"
---
# <a name="list-buckets"></a><span data-ttu-id="d7a27-103">Listar buckets</span><span class="sxs-lookup"><span data-stu-id="d7a27-103">List buckets</span></span>

> <span data-ttu-id="d7a27-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d7a27-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d7a27-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d7a27-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d7a27-106">Recupere uma lista de objetos **plannerbucket**.</span><span class="sxs-lookup"><span data-stu-id="d7a27-106">Retrieve a list of **plannerbucket** objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="d7a27-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d7a27-107">Permissions</span></span>
<span data-ttu-id="d7a27-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7a27-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7a27-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d7a27-110">Permission type</span></span>      | <span data-ttu-id="d7a27-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d7a27-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7a27-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d7a27-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d7a27-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7a27-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d7a27-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d7a27-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7a27-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7a27-115">Not supported.</span></span>    |
|<span data-ttu-id="d7a27-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d7a27-116">Application</span></span> | <span data-ttu-id="d7a27-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7a27-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7a27-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d7a27-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/buckets
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d7a27-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d7a27-119">Optional query parameters</span></span>
<span data-ttu-id="d7a27-120">Este método requer que o [filtro](https://developer.microsoft.com/graph/docs/concepts/query_parameters) de planId seja especificado.</span><span class="sxs-lookup"><span data-stu-id="d7a27-120">This method requires planId [filter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to be specified.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d7a27-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d7a27-121">Request headers</span></span>
| <span data-ttu-id="d7a27-122">Nome</span><span class="sxs-lookup"><span data-stu-id="d7a27-122">Name</span></span>      |<span data-ttu-id="d7a27-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7a27-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d7a27-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d7a27-124">Authorization</span></span>  | <span data-ttu-id="d7a27-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d7a27-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d7a27-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d7a27-127">Request body</span></span>
<span data-ttu-id="d7a27-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d7a27-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7a27-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7a27-129">Response</span></span>

<span data-ttu-id="d7a27-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [plannerBucket](../resources/plannerbucket.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d7a27-130">If successful, this method returns a `200 OK` response code and collection of [plannerBucket](../resources/plannerbucket.md) objects in the response body.</span></span>

<span data-ttu-id="d7a27-p104">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="d7a27-p104">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="d7a27-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d7a27-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d7a27-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d7a27-135">Request</span></span>
<span data-ttu-id="d7a27-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d7a27-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_buckets"
}-->
```http
GET https://graph.microsoft.com/beta/planner/buckets
```
##### <a name="response"></a><span data-ttu-id="d7a27-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7a27-137">Response</span></span>
<span data-ttu-id="d7a27-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d7a27-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
