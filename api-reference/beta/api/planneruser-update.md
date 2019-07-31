---
title: Atualizar plannerUser
description: Atualiza as propriedades de um objeto plannerUser. Você pode usar essa operação para adicionar ou remover planos da lista de planos favoritos de um usuário e para indicar quais planos o usuário exibiu recentemente.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 269741aff4f17a0855bda4681ae49799c03cd4f6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35992168"
---
# <a name="update-planneruser"></a><span data-ttu-id="0978b-104">Atualizar plannerUser</span><span class="sxs-lookup"><span data-stu-id="0978b-104">Update plannerUser</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0978b-105">Atualiza as propriedades de um objeto [plannerUser](../resources/planneruser.md) .</span><span class="sxs-lookup"><span data-stu-id="0978b-105">Update the properties of a [plannerUser](../resources/planneruser.md) object.</span></span> <span data-ttu-id="0978b-106">Você pode usar essa operação para adicionar ou remover planos da lista de planos favoritos de um usuário e para indicar quais planos o usuário exibiu recentemente.</span><span class="sxs-lookup"><span data-stu-id="0978b-106">You can use this operation to add or remove plans from a user's favorite plans list, and to indicate which plans the user has recently viewed.</span></span>

## <a name="permissions"></a><span data-ttu-id="0978b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="0978b-107">Permissions</span></span>
<span data-ttu-id="0978b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0978b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0978b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0978b-110">Permission type</span></span>      | <span data-ttu-id="0978b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0978b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0978b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0978b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0978b-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0978b-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0978b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0978b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0978b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0978b-115">Not supported.</span></span>    |
|<span data-ttu-id="0978b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0978b-116">Application</span></span> | <span data-ttu-id="0978b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0978b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0978b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0978b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/planner
```
## <a name="optional-request-headers"></a><span data-ttu-id="0978b-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="0978b-119">Optional request headers</span></span>
| <span data-ttu-id="0978b-120">Nome</span><span class="sxs-lookup"><span data-stu-id="0978b-120">Name</span></span>       | <span data-ttu-id="0978b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="0978b-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0978b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0978b-122">Authorization</span></span>  | <span data-ttu-id="0978b-123">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="0978b-123">Bearer {code}.</span></span> <span data-ttu-id="0978b-124">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0978b-124">Required.</span></span>|
| <span data-ttu-id="0978b-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="0978b-125">If-Match</span></span>  | <span data-ttu-id="0978b-126">Último valor de ETag conhecido para o **plannerUser** a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="0978b-126">Last known ETag value for the **plannerUser** to be updated.</span></span> <span data-ttu-id="0978b-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0978b-127">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0978b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0978b-128">Request body</span></span>
<span data-ttu-id="0978b-129">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="0978b-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="0978b-130">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="0978b-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="0978b-131">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="0978b-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0978b-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0978b-132">Property</span></span>     | <span data-ttu-id="0978b-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="0978b-133">Type</span></span>   |<span data-ttu-id="0978b-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="0978b-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0978b-135">favoritePlanReferences</span><span class="sxs-lookup"><span data-stu-id="0978b-135">favoritePlanReferences</span></span>|[<span data-ttu-id="0978b-136">plannerFavoritePlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="0978b-136">plannerFavoritePlanReferenceCollection</span></span>](../resources/plannerfavoriteplanreferencecollection.md)|<span data-ttu-id="0978b-137">Alterações à coleção que contém as referências para os planos que o usuário marcou como favorito.</span><span class="sxs-lookup"><span data-stu-id="0978b-137">Changes to the collection containing the references to the plans that the user has marked as a favorite.</span></span>|
|<span data-ttu-id="0978b-138">recentPlanReferences</span><span class="sxs-lookup"><span data-stu-id="0978b-138">recentPlanReferences</span></span>|[<span data-ttu-id="0978b-139">plannerRecentPlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="0978b-139">plannerRecentPlanReferenceCollection</span></span>](../resources/plannerrecentplanreferencecollection.md)|<span data-ttu-id="0978b-140">Alterações à coleção que contém as referências para os planos que o usuário exibiu recentemente.</span><span class="sxs-lookup"><span data-stu-id="0978b-140">Changes to the collection containing the references to the plans that the user has recently viewed.</span></span>|

## <a name="response"></a><span data-ttu-id="0978b-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="0978b-141">Response</span></span>
<span data-ttu-id="0978b-142">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [plannerUser](../resources/planneruser.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0978b-142">If successful, this method returns a `200 OK` response code and an updated [plannerUser](../resources/planneruser.md) object in the response body.</span></span>

<span data-ttu-id="0978b-p107">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="0978b-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="0978b-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0978b-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0978b-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0978b-147">Request</span></span>
<span data-ttu-id="0978b-148">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0978b-148">The following is an example of the request.</span></span> <span data-ttu-id="0978b-149">Essa solicitação adiciona o plano "próxima discussão de lançamento" com ID "jd8S5gOaFk2S8aWCIAJz42QAAxtD" como um favorito para o usuário e remove o plano com ID "7oTB5aMIAE2rVo-1N-L7RmQAGX2q" da lista de planos favoritos.</span><span class="sxs-lookup"><span data-stu-id="0978b-149">This request adds the plan "Next Release Discussion" with ID "jd8S5gOaFk2S8aWCIAJz42QAAxtD" as a favorite for the user, and removes plan with ID "7oTB5aMIAE2rVo-1N-L7RmQAGX2q" from the favorite plans list.</span></span>
<span data-ttu-id="0978b-150">Ele também atualiza a hora da última exibição do plano "jd8S5gOaFk2S8aWCIAJz42QAAxtD".</span><span class="sxs-lookup"><span data-stu-id="0978b-150">It also updates the last view time of the plan "jd8S5gOaFk2S8aWCIAJz42QAAxtD".</span></span>
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
##### <a name="response"></a><span data-ttu-id="0978b-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="0978b-151">Response</span></span>
<span data-ttu-id="0978b-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0978b-152">The following is an example of the response.</span></span> 

><span data-ttu-id="0978b-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0978b-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "suppressions": []
}
-->
