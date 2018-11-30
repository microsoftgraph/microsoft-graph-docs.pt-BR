---
title: Obter plannerPlanDetails
description: Recupere as propriedades e os relacionamentos de um objeto **plannerplandetails**.
ms.openlocfilehash: 652ba06541562f059c7e2b690b99b595e47331c2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006914"
---
# <a name="get-plannerplandetails"></a><span data-ttu-id="83cda-103">Obter plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="83cda-103">Get plannerPlanDetails</span></span>

<span data-ttu-id="83cda-104">Recupere as propriedades e os relacionamentos de um objeto **plannerplandetails**.</span><span class="sxs-lookup"><span data-stu-id="83cda-104">Retrieve the properties and relationships of **plannerplandetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="83cda-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="83cda-105">Permissions</span></span>
<span data-ttu-id="83cda-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83cda-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83cda-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="83cda-108">Permission type</span></span>      | <span data-ttu-id="83cda-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="83cda-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="83cda-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="83cda-110">Delegated (work or school account)</span></span> | <span data-ttu-id="83cda-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83cda-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="83cda-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="83cda-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83cda-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="83cda-113">Not supported.</span></span>    |
|<span data-ttu-id="83cda-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="83cda-114">Application</span></span> | <span data-ttu-id="83cda-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="83cda-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="83cda-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="83cda-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans/{id}/details
```

## <a name="request-headers"></a><span data-ttu-id="83cda-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="83cda-117">Request headers</span></span>
| <span data-ttu-id="83cda-118">Nome</span><span class="sxs-lookup"><span data-stu-id="83cda-118">Name</span></span>      |<span data-ttu-id="83cda-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="83cda-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="83cda-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="83cda-120">Authorization</span></span>  | <span data-ttu-id="83cda-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="83cda-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="83cda-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="83cda-123">Request body</span></span>
<span data-ttu-id="83cda-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="83cda-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83cda-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="83cda-125">Response</span></span>

<span data-ttu-id="83cda-126">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [plannerPlanDetails](../resources/plannerplandetails.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="83cda-126">If successful, this method returns a `200 OK` response code and [plannerPlanDetails](../resources/plannerplandetails.md) object in the response body.</span></span>

<span data-ttu-id="83cda-p103">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="83cda-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="83cda-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="83cda-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="83cda-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="83cda-131">Request</span></span>
<span data-ttu-id="83cda-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="83cda-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannerplandetails"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/plans/{plan-id}/details
```
##### <a name="response"></a><span data-ttu-id="83cda-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="83cda-133">Response</span></span>
<span data-ttu-id="83cda-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="83cda-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlanDetails"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 373

{
  "sharedWith": {
    "aaa27244-1db4-476a-a5cb-004607466324" : true,
    "6463a5ce-2119-4198-9f2a-628761df4a62" : true
  },
  "categoryDescriptions": {
    "category1": "Indoors",
    "category2": "Outdoors",
    "category3": null,
    "category4": null,
    "category5": "Needs materials",
    "category6": "Needs equipment"
  },
  "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerPlanDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->