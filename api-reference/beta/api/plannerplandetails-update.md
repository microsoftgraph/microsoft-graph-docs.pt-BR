---
title: Atualizar plannerplandetails
description: Atualize as propriedades do objeto **plannerplandetails**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: fd42196238fb103021debf8a4fee2f658053a255
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950134"
---
# <a name="update-plannerplandetails"></a><span data-ttu-id="e4b13-103">Atualizar plannerplandetails</span><span class="sxs-lookup"><span data-stu-id="e4b13-103">Update plannerplandetails</span></span>

> <span data-ttu-id="e4b13-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e4b13-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e4b13-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e4b13-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e4b13-106">Atualize as propriedades do objeto **plannerplandetails**.</span><span class="sxs-lookup"><span data-stu-id="e4b13-106">Update the properties of **plannerplandetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e4b13-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e4b13-107">Permissions</span></span>
<span data-ttu-id="e4b13-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4b13-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4b13-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e4b13-110">Permission type</span></span>      | <span data-ttu-id="e4b13-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e4b13-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4b13-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e4b13-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e4b13-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4b13-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e4b13-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e4b13-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4b13-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4b13-115">Not supported.</span></span>    |
|<span data-ttu-id="e4b13-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e4b13-116">Application</span></span> | <span data-ttu-id="e4b13-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4b13-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e4b13-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e4b13-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/plans/<id>/details
```
## <a name="optional-request-headers"></a><span data-ttu-id="e4b13-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="e4b13-119">Optional request headers</span></span>
| <span data-ttu-id="e4b13-120">Nome</span><span class="sxs-lookup"><span data-stu-id="e4b13-120">Name</span></span>       | <span data-ttu-id="e4b13-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4b13-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e4b13-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e4b13-122">Authorization</span></span>  | <span data-ttu-id="e4b13-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e4b13-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e4b13-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="e4b13-125">If-Match</span></span>  | <span data-ttu-id="e4b13-p104">O último valor ETag conhecido do objeto plannerPlanDetails a ser atualizado. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e4b13-p104">Last known ETag value for the plannerPlanDetails to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4b13-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e4b13-128">Request body</span></span>
<span data-ttu-id="e4b13-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="e4b13-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e4b13-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e4b13-132">Property</span></span>     | <span data-ttu-id="e4b13-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="e4b13-133">Type</span></span>   |<span data-ttu-id="e4b13-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4b13-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e4b13-135">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="e4b13-135">categoryDescriptions</span></span>|[<span data-ttu-id="e4b13-136">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="e4b13-136">plannerCategoryDescriptions</span></span>](../resources/plannercategorydescriptions.md)|<span data-ttu-id="e4b13-137">Um objeto que especifica as descrições das seis categorias que podem ser associadas a tarefas no plano</span><span class="sxs-lookup"><span data-stu-id="e4b13-137">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="e4b13-138">sharedWith</span><span class="sxs-lookup"><span data-stu-id="e4b13-138">sharedWith</span></span>|[<span data-ttu-id="e4b13-139">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="e4b13-139">plannerUserIds</span></span>](../resources/planneruserids.md)|<span data-ttu-id="e4b13-p106">Conjunto de identificações de usuários com o qual esse plano é compartilhado. Se você estiver aproveitando os Grupos do Office 365, use a API de Grupos para gerenciar a associação a um grupo para compartilhar o plano [do grupo](../resources/group.md). Você também pode adicionar membros existentes do grupo a essa coleção, embora isso não seja necessário para que eles possam acessar o plano do grupo.</span><span class="sxs-lookup"><span data-stu-id="e4b13-p106">Set of user ids that this plan is shared with. If you are leveraging Office 365 Groups, use the Groups API to manage group membership to share the [group's](../resources/group.md) plan. You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span>|

## <a name="response"></a><span data-ttu-id="e4b13-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4b13-143">Response</span></span>

<span data-ttu-id="e4b13-144">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [plannerPlanDetails](../resources/plannerplandetails.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e4b13-144">If successful, this method returns a `200 OK` response code and updated [plannerPlanDetails](../resources/plannerplandetails.md) object in the response body.</span></span>

<span data-ttu-id="e4b13-p107">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="e4b13-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="e4b13-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e4b13-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e4b13-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4b13-149">Request</span></span>
<span data-ttu-id="e4b13-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e4b13-150">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="e4b13-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4b13-151">Response</span></span>
<span data-ttu-id="e4b13-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e4b13-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Update plannerplandetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
