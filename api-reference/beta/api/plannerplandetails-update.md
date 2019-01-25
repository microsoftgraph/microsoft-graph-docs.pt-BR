---
title: Atualizar plannerplandetails
description: Atualize as propriedades do objeto **plannerplandetails**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: cf54e7c357d1682c904306333e3127cd2276b10f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521941"
---
# <a name="update-plannerplandetails"></a><span data-ttu-id="402c9-103">Atualizar plannerplandetails</span><span class="sxs-lookup"><span data-stu-id="402c9-103">Update plannerplandetails</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="402c9-104">Atualize as propriedades do objeto **plannerplandetails**.</span><span class="sxs-lookup"><span data-stu-id="402c9-104">Update the properties of **plannerplandetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="402c9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="402c9-105">Permissions</span></span>
<span data-ttu-id="402c9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="402c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="402c9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="402c9-108">Permission type</span></span>      | <span data-ttu-id="402c9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="402c9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="402c9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="402c9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="402c9-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="402c9-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="402c9-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="402c9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="402c9-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="402c9-113">Not supported.</span></span>    |
|<span data-ttu-id="402c9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="402c9-114">Application</span></span> | <span data-ttu-id="402c9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="402c9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="402c9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="402c9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/plans/<id>/details
```
## <a name="optional-request-headers"></a><span data-ttu-id="402c9-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="402c9-117">Optional request headers</span></span>
| <span data-ttu-id="402c9-118">Nome</span><span class="sxs-lookup"><span data-stu-id="402c9-118">Name</span></span>       | <span data-ttu-id="402c9-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="402c9-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="402c9-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="402c9-120">Authorization</span></span>  | <span data-ttu-id="402c9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="402c9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="402c9-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="402c9-123">If-Match</span></span>  | <span data-ttu-id="402c9-p103">O último valor ETag conhecido do objeto plannerPlanDetails a ser atualizado. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="402c9-p103">Last known ETag value for the plannerPlanDetails to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="402c9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="402c9-126">Request body</span></span>
<span data-ttu-id="402c9-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="402c9-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="402c9-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="402c9-130">Property</span></span>     | <span data-ttu-id="402c9-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="402c9-131">Type</span></span>   |<span data-ttu-id="402c9-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="402c9-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="402c9-133">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="402c9-133">categoryDescriptions</span></span>|[<span data-ttu-id="402c9-134">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="402c9-134">plannerCategoryDescriptions</span></span>](../resources/plannercategorydescriptions.md)|<span data-ttu-id="402c9-135">Um objeto que especifica as descrições das seis categorias que podem ser associadas a tarefas no plano</span><span class="sxs-lookup"><span data-stu-id="402c9-135">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="402c9-136">sharedWith</span><span class="sxs-lookup"><span data-stu-id="402c9-136">sharedWith</span></span>|[<span data-ttu-id="402c9-137">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="402c9-137">plannerUserIds</span></span>](../resources/planneruserids.md)|<span data-ttu-id="402c9-p105">Conjunto de identificações de usuários com o qual esse plano é compartilhado. Se você estiver aproveitando os Grupos do Office 365, use a API de Grupos para gerenciar a associação a um grupo para compartilhar o plano [do grupo](../resources/group.md). Você também pode adicionar membros existentes do grupo a essa coleção, embora isso não seja necessário para que eles possam acessar o plano do grupo.</span><span class="sxs-lookup"><span data-stu-id="402c9-p105">Set of user ids that this plan is shared with. If you are leveraging Office 365 Groups, use the Groups API to manage group membership to share the [group's](../resources/group.md) plan. You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span>|

## <a name="response"></a><span data-ttu-id="402c9-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="402c9-141">Response</span></span>

<span data-ttu-id="402c9-142">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [plannerPlanDetails](../resources/plannerplandetails.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="402c9-142">If successful, this method returns a `200 OK` response code and updated [plannerPlanDetails](../resources/plannerplandetails.md) object in the response body.</span></span>

<span data-ttu-id="402c9-p106">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="402c9-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="402c9-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="402c9-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="402c9-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="402c9-147">Request</span></span>
<span data-ttu-id="402c9-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="402c9-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerplandetails"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/plans/xqQg5FS2LkCp935s-FIFm2QAFkHM/details
Content-type: application/json
Content-length: 212
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "sharedWith": {
    "6463a5ce-2119-4198-9f2a-628761df4a62" : true,
    "d95e6152-f683-4d78-9ff5-67ad180fea4a" : false,
  },
  "categoryDescriptions": {
    "category1": "Indoors",
    "category3": null,
  }
}
```
##### <a name="response"></a><span data-ttu-id="402c9-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="402c9-149">Response</span></span>
<span data-ttu-id="402c9-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="402c9-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update plannerplandetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/plannerplandetails-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
