---
title: Atualizar plannerPlan
description: Atualize as propriedades do objeto **plannerPlan** .
localization_priority: Normal
ms.openlocfilehash: 6e15ff81f48a7e98a53cefea0bee5c33be24b34f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876444"
---
# <a name="update-plannerplan"></a><span data-ttu-id="6dd32-103">Atualizar plannerPlan</span><span class="sxs-lookup"><span data-stu-id="6dd32-103">Update plannerPlan</span></span>

> <span data-ttu-id="6dd32-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6dd32-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6dd32-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6dd32-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6dd32-106">Atualize as propriedades do objeto **plannerPlan** .</span><span class="sxs-lookup"><span data-stu-id="6dd32-106">Update the properties of **plannerPlan** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6dd32-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="6dd32-107">Permissions</span></span>
<span data-ttu-id="6dd32-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6dd32-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6dd32-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6dd32-110">Permission type</span></span>      | <span data-ttu-id="6dd32-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6dd32-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6dd32-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6dd32-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6dd32-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6dd32-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6dd32-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6dd32-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6dd32-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6dd32-115">Not supported.</span></span>    |
|<span data-ttu-id="6dd32-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6dd32-116">Application</span></span> | <span data-ttu-id="6dd32-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6dd32-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6dd32-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6dd32-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/plans/<id>
```

## <a name="request-headers"></a><span data-ttu-id="6dd32-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6dd32-119">Request headers</span></span>

| <span data-ttu-id="6dd32-120">Nome</span><span class="sxs-lookup"><span data-stu-id="6dd32-120">Name</span></span>       | <span data-ttu-id="6dd32-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="6dd32-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="6dd32-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6dd32-122">Authorization</span></span>  | <span data-ttu-id="6dd32-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6dd32-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6dd32-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="6dd32-125">If-Match</span></span>  | <span data-ttu-id="6dd32-p104">O último valor ETag conhecido do objeto plannerPlan a ser atualizado. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6dd32-p104">Last known ETag value for the plannerPlan to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6dd32-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6dd32-128">Request body</span></span>
<span data-ttu-id="6dd32-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="6dd32-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6dd32-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6dd32-132">Property</span></span>     | <span data-ttu-id="6dd32-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="6dd32-133">Type</span></span>   |<span data-ttu-id="6dd32-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="6dd32-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6dd32-135">owner</span><span class="sxs-lookup"><span data-stu-id="6dd32-135">owner</span></span>|<span data-ttu-id="6dd32-136">String</span><span class="sxs-lookup"><span data-stu-id="6dd32-136">String</span></span>|<span data-ttu-id="6dd32-p106">[Grupo](../resources/group.md) `id` ao qual o plano pertence. Deve haver um grupo válido para que esse campo possa ser definido. Após definido, ele só poderá ser atualizado pelo proprietário.</span><span class="sxs-lookup"><span data-stu-id="6dd32-p106">[Group](../resources/group.md) `id` by which the plan is owned. A valid group must exist before this field can be set. Once set, this can only be updated by the owner.</span></span>|
|<span data-ttu-id="6dd32-140">title</span><span class="sxs-lookup"><span data-stu-id="6dd32-140">title</span></span>|<span data-ttu-id="6dd32-141">String</span><span class="sxs-lookup"><span data-stu-id="6dd32-141">String</span></span>|<span data-ttu-id="6dd32-142">Título do plano.</span><span class="sxs-lookup"><span data-stu-id="6dd32-142">Title of the plan.</span></span>|

## <a name="response"></a><span data-ttu-id="6dd32-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="6dd32-143">Response</span></span>

<span data-ttu-id="6dd32-144">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [plannerPlan](../resources/plannerplan.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6dd32-144">If successful, this method returns a `200 OK` response code and updated [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="6dd32-p107">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="6dd32-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="6dd32-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6dd32-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6dd32-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6dd32-149">Request</span></span>
<span data-ttu-id="6dd32-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6dd32-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerplan"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/plans/<id>
Content-type: application/json
Content-length: 29
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "title": "title-value"
}
```
##### <a name="response"></a><span data-ttu-id="6dd32-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="6dd32-151">Response</span></span>
<span data-ttu-id="6dd32-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6dd32-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update plannerplan",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
