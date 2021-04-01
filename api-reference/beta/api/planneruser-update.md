---
title: Atualizar plannerUser
description: Atualize as propriedades de um objeto plannerUser. Você pode usar essa operação para adicionar ou remover planos da lista de planos favoritos de um usuário e para indicar quais planos o usuário exibiu recentemente.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 0555d7ccfd843fbfac3cf51fe43c61e16930421a
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473924"
---
# <a name="update-planneruser"></a><span data-ttu-id="c4da9-104">Atualizar plannerUser</span><span class="sxs-lookup"><span data-stu-id="c4da9-104">Update plannerUser</span></span>

<span data-ttu-id="c4da9-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4da9-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4da9-106">Atualize as propriedades de um [objeto plannerUser.](../resources/planneruser.md)</span><span class="sxs-lookup"><span data-stu-id="c4da9-106">Update the properties of a [plannerUser](../resources/planneruser.md) object.</span></span> <span data-ttu-id="c4da9-107">Você pode usar essa operação para adicionar ou remover planos da lista de planos favoritos de um usuário e para indicar quais planos o usuário exibiu recentemente.</span><span class="sxs-lookup"><span data-stu-id="c4da9-107">You can use this operation to add or remove plans from a user's favorite plans list, and to indicate which plans the user has recently viewed.</span></span>

## <a name="permissions"></a><span data-ttu-id="c4da9-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="c4da9-108">Permissions</span></span>
<span data-ttu-id="c4da9-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4da9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4da9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c4da9-111">Permission type</span></span>      | <span data-ttu-id="c4da9-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c4da9-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4da9-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c4da9-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c4da9-114">Tasks.ReadWrite, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4da9-114">Tasks.ReadWrite, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c4da9-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c4da9-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4da9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4da9-116">Not supported.</span></span>    |
|<span data-ttu-id="c4da9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c4da9-117">Application</span></span> | <span data-ttu-id="c4da9-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4da9-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4da9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c4da9-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/planner
```
## <a name="optional-request-headers"></a><span data-ttu-id="c4da9-120">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="c4da9-120">Optional request headers</span></span>
| <span data-ttu-id="c4da9-121">Nome</span><span class="sxs-lookup"><span data-stu-id="c4da9-121">Name</span></span>       | <span data-ttu-id="c4da9-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4da9-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c4da9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c4da9-123">Authorization</span></span>  | <span data-ttu-id="c4da9-124">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="c4da9-124">Bearer {code}.</span></span> <span data-ttu-id="c4da9-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4da9-125">Required.</span></span>|
| <span data-ttu-id="c4da9-126">If-Match</span><span class="sxs-lookup"><span data-stu-id="c4da9-126">If-Match</span></span>  | <span data-ttu-id="c4da9-127">Último valor ETag conhecido para o **plannerUser** ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="c4da9-127">Last known ETag value for the **plannerUser** to be updated.</span></span> <span data-ttu-id="c4da9-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4da9-128">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4da9-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c4da9-129">Request body</span></span>
<span data-ttu-id="c4da9-130">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="c4da9-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="c4da9-131">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="c4da9-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="c4da9-132">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="c4da9-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c4da9-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c4da9-133">Property</span></span>     | <span data-ttu-id="c4da9-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="c4da9-134">Type</span></span>   |<span data-ttu-id="c4da9-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4da9-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c4da9-136">favoritePlanReferences</span><span class="sxs-lookup"><span data-stu-id="c4da9-136">favoritePlanReferences</span></span>|[<span data-ttu-id="c4da9-137">plannerFavoritePlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="c4da9-137">plannerFavoritePlanReferenceCollection</span></span>](../resources/plannerfavoriteplanreferencecollection.md)|<span data-ttu-id="c4da9-138">Alterações na coleção que contém as referências aos planos que o usuário marcou como favorito.</span><span class="sxs-lookup"><span data-stu-id="c4da9-138">Changes to the collection containing the references to the plans that the user has marked as a favorite.</span></span>|
|<span data-ttu-id="c4da9-139">recentPlanReferences</span><span class="sxs-lookup"><span data-stu-id="c4da9-139">recentPlanReferences</span></span>|[<span data-ttu-id="c4da9-140">plannerRecentPlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="c4da9-140">plannerRecentPlanReferenceCollection</span></span>](../resources/plannerrecentplanreferencecollection.md)|<span data-ttu-id="c4da9-141">Alterações na coleção que contém as referências aos planos que o usuário exibiu recentemente.</span><span class="sxs-lookup"><span data-stu-id="c4da9-141">Changes to the collection containing the references to the plans that the user has recently viewed.</span></span>|

## <a name="response"></a><span data-ttu-id="c4da9-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4da9-142">Response</span></span>
<span data-ttu-id="c4da9-143">Se tiver êxito, este método retornará `204 No Content` resposta e conteúdo vazio.</span><span class="sxs-lookup"><span data-stu-id="c4da9-143">If successful, this method returns `204 No Content` response and empty content.</span></span> <span data-ttu-id="c4da9-144">Se a solicitação especificar o header com preferência, este método retornará um código de resposta e um `Prefer` `return=representation` objeto `200 OK` [plannerUser](../resources/planneruser.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c4da9-144">If the request specifies `Prefer` header with `return=representation` preference, then this method returns a `200 OK` response code and an updated [plannerUser](../resources/planneruser.md) object in the response body.</span></span>

<span data-ttu-id="c4da9-p108">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="c4da9-p108">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="c4da9-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c4da9-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c4da9-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4da9-149">Request</span></span>
<span data-ttu-id="c4da9-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c4da9-150">The following is an example of the request.</span></span> <span data-ttu-id="c4da9-151">Esta solicitação adiciona o plano "Próxima Discussão de Lançamento" com a ID "jd8S5gOaFk2S8aWCIAJz42QAAxtD" como um favorito para o usuário e remove o plano com iD "7oTB5aMIAE2rVo-1N-L7RmQAGX2q" da lista de planos favoritos.</span><span class="sxs-lookup"><span data-stu-id="c4da9-151">This request adds the plan "Next Release Discussion" with ID "jd8S5gOaFk2S8aWCIAJz42QAAxtD" as a favorite for the user, and removes plan with ID "7oTB5aMIAE2rVo-1N-L7RmQAGX2q" from the favorite plans list.</span></span>
<span data-ttu-id="c4da9-152">Ele também atualiza o último tempo de exibição do plano "jd8S5gOaFk2S8aWCIAJz42QAAxtD".</span><span class="sxs-lookup"><span data-stu-id="c4da9-152">It also updates the last view time of the plan "jd8S5gOaFk2S8aWCIAJz42QAAxtD".</span></span>

# <a name="http"></a>[<span data-ttu-id="c4da9-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4da9-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_planneruser"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/planner
Content-type: application/json
Content-length: 504
Prefer: return=representation
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
# <a name="c"></a>[<span data-ttu-id="c4da9-154">C#</span><span class="sxs-lookup"><span data-stu-id="c4da9-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-planneruser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c4da9-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4da9-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-planneruser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c4da9-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4da9-156">Response</span></span>
<span data-ttu-id="c4da9-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c4da9-157">The following is an example of the response.</span></span> 

><span data-ttu-id="c4da9-p110">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c4da9-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
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


