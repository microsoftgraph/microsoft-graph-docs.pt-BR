---
title: Atualizar plannertaskdetails
description: Atualize as propriedades do **objeto plannertaskdetails.**
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: f7b610f2ba142346de4bbcdf65acc80409b1045f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049965"
---
# <a name="update-plannertaskdetails"></a><span data-ttu-id="81883-103">Atualizar plannertaskdetails</span><span class="sxs-lookup"><span data-stu-id="81883-103">Update plannertaskdetails</span></span>

<span data-ttu-id="81883-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81883-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81883-105">Atualize as propriedades do **objeto plannertaskdetails.**</span><span class="sxs-lookup"><span data-stu-id="81883-105">Update the properties of **plannertaskdetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="81883-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="81883-106">Permissions</span></span>
<span data-ttu-id="81883-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81883-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81883-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81883-109">Permission type</span></span>      | <span data-ttu-id="81883-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="81883-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81883-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81883-111">Delegated (work or school account)</span></span> | <span data-ttu-id="81883-112">Tasks.ReadWrite, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81883-112">Tasks.ReadWrite, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="81883-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81883-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81883-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81883-114">Not supported.</span></span>    |
|<span data-ttu-id="81883-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="81883-115">Application</span></span> | <span data-ttu-id="81883-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81883-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="81883-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81883-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}/details
```
## <a name="optional-request-headers"></a><span data-ttu-id="81883-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="81883-118">Optional request headers</span></span>
| <span data-ttu-id="81883-119">Nome</span><span class="sxs-lookup"><span data-stu-id="81883-119">Name</span></span>       | <span data-ttu-id="81883-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="81883-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="81883-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="81883-121">Authorization</span></span>  | <span data-ttu-id="81883-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81883-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="81883-124">If-Match</span><span class="sxs-lookup"><span data-stu-id="81883-124">If-Match</span></span>  | <span data-ttu-id="81883-125">Último valor ETag conhecido para o **plannerTaskDetails** a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="81883-125">Last known ETag value for the **plannerTaskDetails** to be updated.</span></span> <span data-ttu-id="81883-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81883-126">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="81883-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81883-127">Request body</span></span>
<span data-ttu-id="81883-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="81883-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="81883-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81883-131">Property</span></span>     | <span data-ttu-id="81883-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="81883-132">Type</span></span>   |<span data-ttu-id="81883-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="81883-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81883-134">checklist</span><span class="sxs-lookup"><span data-stu-id="81883-134">checklist</span></span>|[<span data-ttu-id="81883-135">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="81883-135">plannerChecklistItems</span></span>](../resources/plannerchecklistitems.md)|<span data-ttu-id="81883-136">A coleção de itens de lista de verificação na tarefa.</span><span class="sxs-lookup"><span data-stu-id="81883-136">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="81883-137">description</span><span class="sxs-lookup"><span data-stu-id="81883-137">description</span></span>|<span data-ttu-id="81883-138">String</span><span class="sxs-lookup"><span data-stu-id="81883-138">String</span></span>|<span data-ttu-id="81883-139">Descrição da tarefa</span><span class="sxs-lookup"><span data-stu-id="81883-139">Description of the task</span></span>|
|<span data-ttu-id="81883-140">previewType</span><span class="sxs-lookup"><span data-stu-id="81883-140">previewType</span></span>|<span data-ttu-id="81883-141">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="81883-141">string</span></span>|<span data-ttu-id="81883-142">Isso define o tipo de visualização que aparece na tarefa.</span><span class="sxs-lookup"><span data-stu-id="81883-142">This sets the type of preview that shows up on the task.</span></span> <span data-ttu-id="81883-143">Os valores possíveis são: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span><span class="sxs-lookup"><span data-stu-id="81883-143">Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span></span> <span data-ttu-id="81883-144">Quando definido para `automatic` a visualização exibida, é escolhido pelo aplicativo exibindo a tarefa.</span><span class="sxs-lookup"><span data-stu-id="81883-144">When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="81883-145">referências</span><span class="sxs-lookup"><span data-stu-id="81883-145">references</span></span>|[<span data-ttu-id="81883-146">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="81883-146">plannerExternalReferences</span></span>](../resources/plannerexternalreferences.md)|<span data-ttu-id="81883-147">A coleção de referências na tarefa.</span><span class="sxs-lookup"><span data-stu-id="81883-147">The collection of references on the task.</span></span>|

## <a name="response"></a><span data-ttu-id="81883-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="81883-148">Response</span></span>

<span data-ttu-id="81883-149">Se tiver êxito, este método retornará `204 No Content` resposta e conteúdo vazio.</span><span class="sxs-lookup"><span data-stu-id="81883-149">If successful, this method returns `204 No Content` response and empty content.</span></span> <span data-ttu-id="81883-150">Se a solicitação especificar o header com preferência, este método retornará um código de resposta e o objeto `Prefer` `return=representation` `200 OK` [plannerTaskDetails](../resources/plannertaskdetails.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81883-150">If the request specifies `Prefer` header with `return=representation` preference, then this method returns a `200 OK` response code and updated [plannerTaskDetails](../resources/plannertaskdetails.md) object in the response body.</span></span>

<span data-ttu-id="81883-p107">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="81883-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="81883-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="81883-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="81883-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81883-155">Request</span></span>
<span data-ttu-id="81883-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="81883-156">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="81883-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="81883-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannertaskdetails"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/tasks/gcrYAaAkgU2EQUvpkNNXLGQAGTtu/details
Content-type: application/json
Content-length: 857
Prefer: return=representation
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
# <a name="javascript"></a>[<span data-ttu-id="81883-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="81883-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannertaskdetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="81883-159">C#</span><span class="sxs-lookup"><span data-stu-id="81883-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannertaskdetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="81883-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="81883-160">Response</span></span>
<span data-ttu-id="81883-161">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81883-161">Here is an example of the response.</span></span> <span data-ttu-id="81883-162">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="81883-162">Note: The response object shown here might be shortened for readability.</span></span>
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


