---
title: Atualizar plannerUser
description: Atualize as propriedades de um objeto plannerUser. Você pode usar essa operação para adicionar ou remover os planos da lista de planos de favoritos do usuário e indicar que o usuário estiver planejando acessou recentemente.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 733743ffee8e29d66f2ebe411d127161e7e8eb2a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925886"
---
# <a name="update-planneruser"></a><span data-ttu-id="4904e-104">Atualizar plannerUser</span><span class="sxs-lookup"><span data-stu-id="4904e-104">Update plannerUser</span></span>

> <span data-ttu-id="4904e-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4904e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4904e-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4904e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4904e-107">Atualize as propriedades de um objeto [plannerUser](../resources/planneruser.md) .</span><span class="sxs-lookup"><span data-stu-id="4904e-107">Update the properties of a [plannerUser](../resources/planneruser.md) object.</span></span> <span data-ttu-id="4904e-108">Você pode usar essa operação para adicionar ou remover os planos da lista de planos de favoritos do usuário e indicar que o usuário estiver planejando acessou recentemente.</span><span class="sxs-lookup"><span data-stu-id="4904e-108">You can use this operation to add or remove plans from a user's favorite plans list, and to indicate which plans the user has recently viewed.</span></span>

## <a name="permissions"></a><span data-ttu-id="4904e-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="4904e-109">Permissions</span></span>
<span data-ttu-id="4904e-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4904e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4904e-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4904e-112">Permission type</span></span>      | <span data-ttu-id="4904e-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4904e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4904e-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4904e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="4904e-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4904e-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4904e-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4904e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4904e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4904e-117">Not supported.</span></span>    |
|<span data-ttu-id="4904e-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4904e-118">Application</span></span> | <span data-ttu-id="4904e-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4904e-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4904e-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4904e-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/planner
```
## <a name="optional-request-headers"></a><span data-ttu-id="4904e-121">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="4904e-121">Optional request headers</span></span>
| <span data-ttu-id="4904e-122">Nome</span><span class="sxs-lookup"><span data-stu-id="4904e-122">Name</span></span>       | <span data-ttu-id="4904e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="4904e-123">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4904e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="4904e-124">Authorization</span></span>  | <span data-ttu-id="4904e-p105">Portador {código}. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4904e-p105">Bearer {code}. Required.</span></span>|
| <span data-ttu-id="4904e-127">If-Match</span><span class="sxs-lookup"><span data-stu-id="4904e-127">If-Match</span></span>  | <span data-ttu-id="4904e-128">Último valor conhecido do ETag para o **plannerUser** a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="4904e-128">Last known ETag value for the **plannerUser** to be updated.</span></span> <span data-ttu-id="4904e-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4904e-129">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4904e-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4904e-130">Request body</span></span>
<span data-ttu-id="4904e-131">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="4904e-131">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="4904e-132">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações em outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="4904e-132">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="4904e-133">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="4904e-133">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4904e-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4904e-134">Property</span></span>     | <span data-ttu-id="4904e-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="4904e-135">Type</span></span>   |<span data-ttu-id="4904e-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="4904e-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4904e-137">favoritePlanReferences</span><span class="sxs-lookup"><span data-stu-id="4904e-137">favoritePlanReferences</span></span>|[<span data-ttu-id="4904e-138">plannerFavoritePlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="4904e-138">plannerFavoritePlanReferenceCollection</span></span>](../resources/plannerfavoriteplanreferencecollection.md)|<span data-ttu-id="4904e-139">Alterações à coleção que contém as referências para os planos de que o usuário tenha marcado como um favorito.</span><span class="sxs-lookup"><span data-stu-id="4904e-139">Changes to the collection containing the references to the plans that the user has marked as a favorite.</span></span>|
|<span data-ttu-id="4904e-140">recentPlanReferences</span><span class="sxs-lookup"><span data-stu-id="4904e-140">recentPlanReferences</span></span>|[<span data-ttu-id="4904e-141">plannerRecentPlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="4904e-141">plannerRecentPlanReferenceCollection</span></span>](../resources/plannerrecentplanreferencecollection.md)|<span data-ttu-id="4904e-142">Alterações à coleção que contém as referências para os planos de que o usuário acessou recentemente.</span><span class="sxs-lookup"><span data-stu-id="4904e-142">Changes to the collection containing the references to the plans that the user has recently viewed.</span></span>|

## <a name="response"></a><span data-ttu-id="4904e-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="4904e-143">Response</span></span>
<span data-ttu-id="4904e-144">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [plannerUser](../resources/planneruser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4904e-144">If successful, this method returns a `200 OK` response code and an updated [plannerUser](../resources/planneruser.md) object in the response body.</span></span>

<span data-ttu-id="4904e-p108">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="4904e-p108">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="4904e-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4904e-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4904e-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4904e-149">Request</span></span>
<span data-ttu-id="4904e-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4904e-150">The following is an example of the request.</span></span> <span data-ttu-id="4904e-151">Essa solicitação adiciona o plano de "Próximo lançamento discussão" com o ID "jd8S5gOaFk2S8aWCIAJz42QAAxtD" como um favorito para o usuário e remove plano com ID "7oTB5aMIAE2rVo-1N-L7RmQAGX2q" da lista de planos favorito.</span><span class="sxs-lookup"><span data-stu-id="4904e-151">This request adds the plan "Next Release Discussion" with ID "jd8S5gOaFk2S8aWCIAJz42QAAxtD" as a favorite for the user, and removes plan with ID "7oTB5aMIAE2rVo-1N-L7RmQAGX2q" from the favorite plans list.</span></span>
<span data-ttu-id="4904e-152">Ele também atualiza a última vez em modo de exibição do plano de "jd8S5gOaFk2S8aWCIAJz42QAAxtD".</span><span class="sxs-lookup"><span data-stu-id="4904e-152">It also updates the last view time of the plan "jd8S5gOaFk2S8aWCIAJz42QAAxtD".</span></span>
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
##### <a name="response"></a><span data-ttu-id="4904e-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="4904e-153">Response</span></span>
<span data-ttu-id="4904e-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4904e-154">The following is an example of the response.</span></span> 

><span data-ttu-id="4904e-p110">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4904e-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Update planneruser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
