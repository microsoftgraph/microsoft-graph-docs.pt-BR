---
title: Atualizar plannerUser
description: Atualize as propriedades de um objeto plannerUser. Você pode usar essa operação para adicionar ou remover os planos da lista de planos de favoritos do usuário e indicar que o usuário estiver planejando acessou recentemente.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 95c631d39fb650dea0b87871bdd10d92a3ab31eb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508920"
---
# <a name="update-planneruser"></a><span data-ttu-id="7e5c3-104">Atualizar plannerUser</span><span class="sxs-lookup"><span data-stu-id="7e5c3-104">Update plannerUser</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e5c3-105">Atualize as propriedades de um objeto [plannerUser](../resources/planneruser.md) .</span><span class="sxs-lookup"><span data-stu-id="7e5c3-105">Update the properties of a [plannerUser](../resources/planneruser.md) object.</span></span> <span data-ttu-id="7e5c3-106">Você pode usar essa operação para adicionar ou remover os planos da lista de planos de favoritos do usuário e indicar que o usuário estiver planejando acessou recentemente.</span><span class="sxs-lookup"><span data-stu-id="7e5c3-106">You can use this operation to add or remove plans from a user's favorite plans list, and to indicate which plans the user has recently viewed.</span></span>

## <a name="permissions"></a><span data-ttu-id="7e5c3-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="7e5c3-107">Permissions</span></span>
<span data-ttu-id="7e5c3-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e5c3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e5c3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7e5c3-110">Permission type</span></span>      | <span data-ttu-id="7e5c3-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7e5c3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e5c3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7e5c3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7e5c3-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e5c3-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7e5c3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7e5c3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e5c3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7e5c3-115">Not supported.</span></span>    |
|<span data-ttu-id="7e5c3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7e5c3-116">Application</span></span> | <span data-ttu-id="7e5c3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7e5c3-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e5c3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7e5c3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/planner
```
## <a name="optional-request-headers"></a><span data-ttu-id="7e5c3-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="7e5c3-119">Optional request headers</span></span>
| <span data-ttu-id="7e5c3-120">Nome</span><span class="sxs-lookup"><span data-stu-id="7e5c3-120">Name</span></span>       | <span data-ttu-id="7e5c3-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e5c3-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="7e5c3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7e5c3-122">Authorization</span></span>  | <span data-ttu-id="7e5c3-p104">Portador {código}. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7e5c3-p104">Bearer {code}. Required.</span></span>|
| <span data-ttu-id="7e5c3-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="7e5c3-125">If-Match</span></span>  | <span data-ttu-id="7e5c3-126">Último valor conhecido do ETag para o **plannerUser** a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="7e5c3-126">Last known ETag value for the **plannerUser** to be updated.</span></span> <span data-ttu-id="7e5c3-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7e5c3-127">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e5c3-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7e5c3-128">Request body</span></span>
<span data-ttu-id="7e5c3-129">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="7e5c3-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="7e5c3-130">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações em outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="7e5c3-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="7e5c3-131">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="7e5c3-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7e5c3-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7e5c3-132">Property</span></span>     | <span data-ttu-id="7e5c3-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="7e5c3-133">Type</span></span>   |<span data-ttu-id="7e5c3-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e5c3-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7e5c3-135">favoritePlanReferences</span><span class="sxs-lookup"><span data-stu-id="7e5c3-135">favoritePlanReferences</span></span>|[<span data-ttu-id="7e5c3-136">plannerFavoritePlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="7e5c3-136">plannerFavoritePlanReferenceCollection</span></span>](../resources/plannerfavoriteplanreferencecollection.md)|<span data-ttu-id="7e5c3-137">Alterações à coleção que contém as referências para os planos de que o usuário tenha marcado como um favorito.</span><span class="sxs-lookup"><span data-stu-id="7e5c3-137">Changes to the collection containing the references to the plans that the user has marked as a favorite.</span></span>|
|<span data-ttu-id="7e5c3-138">recentPlanReferences</span><span class="sxs-lookup"><span data-stu-id="7e5c3-138">recentPlanReferences</span></span>|[<span data-ttu-id="7e5c3-139">plannerRecentPlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="7e5c3-139">plannerRecentPlanReferenceCollection</span></span>](../resources/plannerrecentplanreferencecollection.md)|<span data-ttu-id="7e5c3-140">Alterações à coleção que contém as referências para os planos de que o usuário acessou recentemente.</span><span class="sxs-lookup"><span data-stu-id="7e5c3-140">Changes to the collection containing the references to the plans that the user has recently viewed.</span></span>|

## <a name="response"></a><span data-ttu-id="7e5c3-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e5c3-141">Response</span></span>
<span data-ttu-id="7e5c3-142">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [plannerUser](../resources/planneruser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7e5c3-142">If successful, this method returns a `200 OK` response code and an updated [plannerUser](../resources/planneruser.md) object in the response body.</span></span>

<span data-ttu-id="7e5c3-p107">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="7e5c3-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="7e5c3-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7e5c3-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7e5c3-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7e5c3-147">Request</span></span>
<span data-ttu-id="7e5c3-148">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7e5c3-148">The following is an example of the request.</span></span> <span data-ttu-id="7e5c3-149">Essa solicitação adiciona o plano de "Próximo lançamento discussão" com o ID "jd8S5gOaFk2S8aWCIAJz42QAAxtD" como um favorito para o usuário e remove plano com ID "7oTB5aMIAE2rVo-1N-L7RmQAGX2q" da lista de planos favorito.</span><span class="sxs-lookup"><span data-stu-id="7e5c3-149">This request adds the plan "Next Release Discussion" with ID "jd8S5gOaFk2S8aWCIAJz42QAAxtD" as a favorite for the user, and removes plan with ID "7oTB5aMIAE2rVo-1N-L7RmQAGX2q" from the favorite plans list.</span></span>
<span data-ttu-id="7e5c3-150">Ele também atualiza a última vez em modo de exibição do plano de "jd8S5gOaFk2S8aWCIAJz42QAAxtD".</span><span class="sxs-lookup"><span data-stu-id="7e5c3-150">It also updates the last view time of the plan "jd8S5gOaFk2S8aWCIAJz42QAAxtD".</span></span>
<!-- {
  "blockType": "ignored",
  "name": "update_planneruser"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/planner
Content-type: application/json
Content-length: 504
If-Match: W/"JzEtVXNlckRldGFpbHMgQEBAQEBAQEBAQEBAQEBIWCc="

{
  "favoritePlanReferences": {
    "jd8S5gOaFk2S8aWCIAJz42QAAxtD": {
      "@odata.type": "#microsoft.graph.plannerFavoritePlanReference",
      "orderHint": " !",
      "planTitle": "Next Release Discussion"
    },
    "7oTB5aMIAE2rVo-1N-L7RmQAGX2q": null
  },
  "recentPlanReferences": {
    "jd8S5gOaFk2S8aWCIAJz42QAAxtD": {
      "@odata.type": "#microsoft.graph.plannerRecentPlanReference",
      "lastAccessedDateTime": "2018-01-02T22:49:46.155Z",
      "planTitle": "Next Release Discussion"
    }
  }
}
```
##### <a name="response"></a><span data-ttu-id="7e5c3-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e5c3-151">Response</span></span>
<span data-ttu-id="7e5c3-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7e5c3-152">The following is an example of the response.</span></span> 

><span data-ttu-id="7e5c3-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7e5c3-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 979

{
  "favoritePlanReferences": {
    "jd8S5gOaFk2S8aWCIAJz42QAAxtD": {
      "@odata.type": "#microsoft.graph.plannerFavoritePlanReference",
      "orderHint": "8586866870001551087",
      "planTitle": "Next Release Discussion"
    },
    "uZWtCtli30CGoWLIWSat1mQAC0ai": {
      "@odata.type": "#microsoft.graph.plannerFavoritePlanReference",
      "orderHint": "8586888705198093378",
      "planTitle": "Product Support"
    }
  },
  "recentPlanReferences": {
    "jd8S5gOaFk2S8aWCIAJz42QAAxtD": {
      "@odata.type": "#microsoft.graph.plannerRecentPlanReference",
      "lastAccessedDateTime": "2018-01-02T22:49:46.155Z",
      "planTitle": "Next Release Discussion"
    },
    "XYE5pqNJu0uuRC2PM4ZQrmQAF2Pn": {
      "@odata.type": "#microsoft.graph.plannerRecentPlanReference",
      "lastAccessedDateTime": "2018-01-01T19:39:17.57Z",
      "planTitle": "Success Metrics"
    }
  },
  "id": "-YPnMJRiIUSKFyaVjYEkBWQAAc47"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update planneruser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/planneruser-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
