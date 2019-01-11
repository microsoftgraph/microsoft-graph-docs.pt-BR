---
title: Atualizar plannertaskdetails
description: Atualize as propriedades do objeto **plannertaskdetails**.
localization_priority: Normal
ms.openlocfilehash: b87688c91a3fe33439c15c403ff248b171a3241e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840191"
---
# <a name="update-plannertaskdetails"></a><span data-ttu-id="02f13-103">Atualizar plannertaskdetails</span><span class="sxs-lookup"><span data-stu-id="02f13-103">Update plannertaskdetails</span></span>

<span data-ttu-id="02f13-104">Atualize as propriedades do objeto **plannertaskdetails**.</span><span class="sxs-lookup"><span data-stu-id="02f13-104">Update the properties of **plannertaskdetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="02f13-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="02f13-105">Permissions</span></span>
<span data-ttu-id="02f13-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02f13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02f13-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02f13-108">Permission type</span></span>      | <span data-ttu-id="02f13-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="02f13-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02f13-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02f13-110">Delegated (work or school account)</span></span> | <span data-ttu-id="02f13-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02f13-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="02f13-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02f13-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02f13-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02f13-113">Not supported.</span></span>    |
|<span data-ttu-id="02f13-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02f13-114">Application</span></span> | <span data-ttu-id="02f13-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02f13-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="02f13-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02f13-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}/details
```
## <a name="optional-request-headers"></a><span data-ttu-id="02f13-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="02f13-117">Optional request headers</span></span>
| <span data-ttu-id="02f13-118">Nome</span><span class="sxs-lookup"><span data-stu-id="02f13-118">Name</span></span>       | <span data-ttu-id="02f13-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="02f13-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="02f13-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="02f13-120">Authorization</span></span>  | <span data-ttu-id="02f13-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02f13-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="02f13-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="02f13-123">If-Match</span></span>  | <span data-ttu-id="02f13-p103">O último valor ETag conhecido do objeto **plannerTaskDetails** a ser atualizado. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02f13-p103">Last known ETag value for the **plannerTaskDetails** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="02f13-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02f13-126">Request body</span></span>
<span data-ttu-id="02f13-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="02f13-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="02f13-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="02f13-130">Property</span></span>     | <span data-ttu-id="02f13-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="02f13-131">Type</span></span>   |<span data-ttu-id="02f13-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="02f13-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02f13-133">lista de verificação</span><span class="sxs-lookup"><span data-stu-id="02f13-133">checklist</span></span>|[<span data-ttu-id="02f13-134">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="02f13-134">plannerChecklistItems</span></span>](../resources/plannerchecklistitems.md)|<span data-ttu-id="02f13-135">A coleção de itens da lista de verificação na tarefa.</span><span class="sxs-lookup"><span data-stu-id="02f13-135">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="02f13-136">description</span><span class="sxs-lookup"><span data-stu-id="02f13-136">description</span></span>|<span data-ttu-id="02f13-137">String</span><span class="sxs-lookup"><span data-stu-id="02f13-137">String</span></span>|<span data-ttu-id="02f13-138">Descrição da tarefa</span><span class="sxs-lookup"><span data-stu-id="02f13-138">Description of the task</span></span>|
|<span data-ttu-id="02f13-139">previewType</span><span class="sxs-lookup"><span data-stu-id="02f13-139">previewType</span></span>|<span data-ttu-id="02f13-140">string</span><span class="sxs-lookup"><span data-stu-id="02f13-140">string</span></span>|<span data-ttu-id="02f13-141">Isto define o tipo de visualização que aparecerá na tarefa.</span><span class="sxs-lookup"><span data-stu-id="02f13-141">This sets the type of preview that shows up on the task.</span></span> <span data-ttu-id="02f13-142">Os valores possíveis são: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span><span class="sxs-lookup"><span data-stu-id="02f13-142">The possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span></span> <span data-ttu-id="02f13-143">Quando definido como `automatic` a visualização exibida for escolhida pelo app exibindo a tarefa.</span><span class="sxs-lookup"><span data-stu-id="02f13-143">When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="02f13-144">referências</span><span class="sxs-lookup"><span data-stu-id="02f13-144">references</span></span>|[<span data-ttu-id="02f13-145">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="02f13-145">plannerExternalReferences</span></span>](../resources/plannerexternalreferences.md)|<span data-ttu-id="02f13-146">A coleção de referências na tarefa.</span><span class="sxs-lookup"><span data-stu-id="02f13-146">The collection of references on the task.</span></span>|

## <a name="response"></a><span data-ttu-id="02f13-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="02f13-147">Response</span></span>

<span data-ttu-id="02f13-148">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [plannerTaskDetails](../resources/plannertaskdetails.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02f13-148">If successful, this method returns a `200 OK` response code and updated [plannerTaskDetails](../resources/plannertaskdetails.md) object in the response body.</span></span>

<span data-ttu-id="02f13-p106">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="02f13-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="02f13-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="02f13-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="02f13-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02f13-153">Request</span></span>
<span data-ttu-id="02f13-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="02f13-154">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannertaskdetails"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/tasks/{task-id}/details
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
      "ischecked": true
    },
    "d280ed1a-9f6b-4f9c-a962-fb4d00dc50ff":{
      "@odata.type": "microsoft.graph.plannerChecklistItem",
      "isChecked": true,
    },
    "a93c93c5-10a6-4167-9551-8bafa09967a7": null
  }
}
```
##### <a name="response"></a><span data-ttu-id="02f13-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="02f13-155">Response</span></span>
<span data-ttu-id="02f13-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="02f13-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update plannertaskdetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
