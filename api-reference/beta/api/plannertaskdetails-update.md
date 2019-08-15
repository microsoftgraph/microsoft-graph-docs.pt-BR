---
title: Atualizar plannertaskdetails
description: Atualize as propriedades do objeto **plannertaskdetails** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 44e54574b5a332c61219c05c53337d53c03eba0e
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36413059"
---
# <a name="update-plannertaskdetails"></a><span data-ttu-id="2f6e0-103">Atualizar plannertaskdetails</span><span class="sxs-lookup"><span data-stu-id="2f6e0-103">Update plannertaskdetails</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f6e0-104">Atualize as propriedades do objeto **plannertaskdetails** .</span><span class="sxs-lookup"><span data-stu-id="2f6e0-104">Update the properties of **plannertaskdetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2f6e0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2f6e0-105">Permissions</span></span>
<span data-ttu-id="2f6e0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f6e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f6e0-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f6e0-108">Permission type</span></span>      | <span data-ttu-id="2f6e0-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2f6e0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f6e0-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f6e0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2f6e0-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f6e0-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2f6e0-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f6e0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f6e0-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f6e0-113">Not supported.</span></span>    |
|<span data-ttu-id="2f6e0-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f6e0-114">Application</span></span> | <span data-ttu-id="2f6e0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f6e0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2f6e0-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f6e0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}/details
```
## <a name="optional-request-headers"></a><span data-ttu-id="2f6e0-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="2f6e0-117">Optional request headers</span></span>
| <span data-ttu-id="2f6e0-118">Nome</span><span class="sxs-lookup"><span data-stu-id="2f6e0-118">Name</span></span>       | <span data-ttu-id="2f6e0-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f6e0-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="2f6e0-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f6e0-120">Authorization</span></span>  | <span data-ttu-id="2f6e0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f6e0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2f6e0-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="2f6e0-123">If-Match</span></span>  | <span data-ttu-id="2f6e0-124">Último valor de ETag conhecido para o **plannerTaskDetails** a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="2f6e0-124">Last known ETag value for the **plannerTaskDetails** to be updated.</span></span> <span data-ttu-id="2f6e0-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f6e0-125">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f6e0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f6e0-126">Request body</span></span>
<span data-ttu-id="2f6e0-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="2f6e0-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2f6e0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2f6e0-130">Property</span></span>     | <span data-ttu-id="2f6e0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f6e0-131">Type</span></span>   |<span data-ttu-id="2f6e0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f6e0-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2f6e0-133">verificação</span><span class="sxs-lookup"><span data-stu-id="2f6e0-133">checklist</span></span>|[<span data-ttu-id="2f6e0-134">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="2f6e0-134">plannerChecklistItems</span></span>](../resources/plannerchecklistitems.md)|<span data-ttu-id="2f6e0-135">A coleção de itens de lista de verificação na tarefa.</span><span class="sxs-lookup"><span data-stu-id="2f6e0-135">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="2f6e0-136">descrição</span><span class="sxs-lookup"><span data-stu-id="2f6e0-136">description</span></span>|<span data-ttu-id="2f6e0-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f6e0-137">String</span></span>|<span data-ttu-id="2f6e0-138">Descrição da tarefa</span><span class="sxs-lookup"><span data-stu-id="2f6e0-138">Description of the task</span></span>|
|<span data-ttu-id="2f6e0-139">previewType</span><span class="sxs-lookup"><span data-stu-id="2f6e0-139">previewType</span></span>|<span data-ttu-id="2f6e0-140">string</span><span class="sxs-lookup"><span data-stu-id="2f6e0-140">string</span></span>|<span data-ttu-id="2f6e0-141">Isso define o tipo de visualização que aparece na tarefa.</span><span class="sxs-lookup"><span data-stu-id="2f6e0-141">This sets the type of preview that shows up on the task.</span></span> <span data-ttu-id="2f6e0-142">Os valores possíveis são: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span><span class="sxs-lookup"><span data-stu-id="2f6e0-142">Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span></span> <span data-ttu-id="2f6e0-143">Quando definido para `automatic` a visualização exibida é escolhido pelo aplicativo que está exibindo a tarefa.</span><span class="sxs-lookup"><span data-stu-id="2f6e0-143">When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="2f6e0-144">Referencie</span><span class="sxs-lookup"><span data-stu-id="2f6e0-144">references</span></span>|[<span data-ttu-id="2f6e0-145">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="2f6e0-145">plannerExternalReferences</span></span>](../resources/plannerexternalreferences.md)|<span data-ttu-id="2f6e0-146">A coleção de referências na tarefa.</span><span class="sxs-lookup"><span data-stu-id="2f6e0-146">The collection of references on the task.</span></span>|

## <a name="response"></a><span data-ttu-id="2f6e0-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f6e0-147">Response</span></span>

<span data-ttu-id="2f6e0-148">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [plannerTaskDetails](../resources/plannertaskdetails.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f6e0-148">If successful, this method returns a `200 OK` response code and updated [plannerTaskDetails](../resources/plannertaskdetails.md) object in the response body.</span></span>

<span data-ttu-id="2f6e0-p106">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="2f6e0-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="2f6e0-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f6e0-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2f6e0-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f6e0-153">Request</span></span>
<span data-ttu-id="2f6e0-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f6e0-154">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2f6e0-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f6e0-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannertaskdetails"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/tasks/gcrYAaAkgU2EQUvpkNNXLGQAGTtu/details
Content-type: application/json
Content-length: 857
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "previewType": "noPreview",
  "references": {
    "http%3A//developer%2Emicrosoft%2Ecom":{
      "@odata.type": "microsoft.graph.plannerExternalReference",
      "alias": "Documentation",
      "previewPriority": " !",
      "type": "Other"
    },
    "https%3A//developer%2Emicrosoft%2Ecom/en-us/graph/graph-explorer":{
      "@odata.type": "microsoft.graph.plannerExternalReference",
      "previewPriority": "  !!",
    },
    "http%3A//www%2Ebing%2Ecom": null
  },
  "checklist": {
    "95e27074-6c4a-447a-aa24-9d718a0b86fa":{
      "@odata.type": "microsoft.graph.plannerChecklistItem",
      "title": "Update task details",
      "isChecked": true
    },
    "d280ed1a-9f6b-4f9c-a962-fb4d00dc50ff":{
      "@odata.type": "microsoft.graph.plannerChecklistItem",
      "isChecked": true,
    },
    "a93c93c5-10a6-4167-9551-8bafa09967a7": null
  }
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2f6e0-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2f6e0-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannertaskdetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2f6e0-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f6e0-157">Response</span></span>
<span data-ttu-id="2f6e0-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f6e0-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTaskDetails"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1793

{
  "description": "Task details properties:\nchecklist:Sub items\nreferences:Related links",
  "previewType": "automatic",
  "references": {
    "https%3A//developer%2Emicrosoft%2Ecom/en-us/graph/graph-explorer": {
      "@odata.type": "#microsoft.graph.plannerExternalReference",
      "alias": "Graph Explorer",
      "type": "Other",
      "previewPriority": "8599273",
      "lastModifiedBy": {
        "user": {
          "id": "fbab97d0-4932-4511-b675-204639209557"
        }
      },
      "lastModifiedDateTime": "2017-04-24T22:52:29.814Z"
    },
    "http%3A//developer%2Emicrosoft%2Ecom": {
      "@odata.type": "#microsoft.graph.plannerExternalReference",
      "alias": "Documentation",
      "type": "Other",
      "previewPriority": "90727736",
      "lastModifiedBy": {
        "user": {
          "id": "fbab97d0-4932-4511-b675-204639209557"
        }
      },
      "lastModifiedDateTime": "2017-04-24T22:52:29.814Z"
    }
  },
  "checklist": {
    "d280ed1a-9f6b-4f9c-a962-fb4d00dc50ff": {
      "@odata.type": "#microsoft.graph.plannerChecklistItem",
      "isChecked": true,
      "title": "Try reading task details",
      "orderHint": "a93c93c5^",
      "lastModifiedBy": {
        "user": {
          "id": "fbab97d0-4932-4511-b675-204639209557"
        }
      },
      "lastModifiedDateTime": "2017-04-24T22:52:29.814Z"
    },
    "95e27074-6c4a-447a-aa24-9d718a0b86f": {
      "@odata.type": "#microsoft.graph.plannerChecklistItem",
      "isChecked": true,
      "title": "Update task details",
      "orderHint": "8587094707721254251P]",
      "lastModifiedBy": {
        "user": {
          "id": "fbab97d0-4932-4511-b675-204639209557"
        }
      },
      "lastModifiedDateTime": "2017-04-24T22:52:29.814Z"
    }
  },
  "id": "gcrYAaAkgU2EQUvpkNNXLGQAGTtu"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update plannertaskdetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
