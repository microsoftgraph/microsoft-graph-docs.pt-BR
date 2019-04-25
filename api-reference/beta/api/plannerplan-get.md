---
title: Obter plannerPlan
description: Recupere as propriedades e os relacionamentos do objeto **plannerplan** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 8859452848f8459cba596b95503a8355c331c05d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547099"
---
# <a name="get-plannerplan"></a><span data-ttu-id="648b2-103">Obter plannerPlan</span><span class="sxs-lookup"><span data-stu-id="648b2-103">Get plannerPlan</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="648b2-104">Recupere as propriedades e os relacionamentos do objeto **plannerplan** .</span><span class="sxs-lookup"><span data-stu-id="648b2-104">Retrieve the properties and relationships of **plannerplan** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="648b2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="648b2-105">Permissions</span></span>
<span data-ttu-id="648b2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="648b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="648b2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="648b2-108">Permission type</span></span>      | <span data-ttu-id="648b2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="648b2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="648b2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="648b2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="648b2-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="648b2-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="648b2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="648b2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="648b2-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="648b2-113">Not supported.</span></span>    |
|<span data-ttu-id="648b2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="648b2-114">Application</span></span> | <span data-ttu-id="648b2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="648b2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="648b2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="648b2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans/<id>
```
## <a name="request-headers"></a><span data-ttu-id="648b2-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="648b2-117">Request headers</span></span>
| <span data-ttu-id="648b2-118">Nome</span><span class="sxs-lookup"><span data-stu-id="648b2-118">Name</span></span>      |<span data-ttu-id="648b2-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="648b2-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="648b2-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="648b2-120">Authorization</span></span>  | <span data-ttu-id="648b2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="648b2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="648b2-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="648b2-123">Request body</span></span>
<span data-ttu-id="648b2-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="648b2-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="648b2-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="648b2-125">Response</span></span>

<span data-ttu-id="648b2-126">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [plannerPlan](../resources/plannerplan.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="648b2-126">If successful, this method returns a `200 OK` response code and [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="648b2-127">Este método pode retornar qualquer um dos [códigos de status http](/graph/errors).</span><span class="sxs-lookup"><span data-stu-id="648b2-127">This method can return any of the [HTTP status codes](/graph/errors).</span></span> <span data-ttu-id="648b2-128">Os erros mais comuns que os aplicativos devem lidar com esse método são as respostas 403 e 404.</span><span class="sxs-lookup"><span data-stu-id="648b2-128">The most common errors that apps should handle for this method are the 403 and 404 responses.</span></span> <span data-ttu-id="648b2-129">Para obter mais informações sobre esses erros, confira [condições de erro do planejador comum](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="648b2-129">For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="648b2-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="648b2-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="648b2-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="648b2-131">Request</span></span>
<span data-ttu-id="648b2-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="648b2-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannerplan"
}-->
```http
GET https://graph.microsoft.com/beta/planner/plans/<id>
```
##### <a name="response"></a><span data-ttu-id="648b2-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="648b2-133">Response</span></span>
<span data-ttu-id="648b2-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="648b2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 357

{
  "createdBy": {
    "application": {
      "id": "95e27074-6c4a-447a-aa24-9d718a0b86fa"
    },
    "user": {
      "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
    }
  },
  "createdDateTime": "2015-03-30T18:36:49.2407981Z",
  "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
  "title": "title-value",
  "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get plannerPlan",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/plannerplan-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
