# <a name="update-plannertaskdetails"></a><span data-ttu-id="94030-101">Atualizar plannertaskdetails</span><span class="sxs-lookup"><span data-stu-id="94030-101">Update plannertaskdetails</span></span>

<span data-ttu-id="94030-102">Atualize as propriedades do objeto **plannertaskdetails**.</span><span class="sxs-lookup"><span data-stu-id="94030-102">Update the properties of **plannertaskdetails** object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="94030-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="94030-103">Prerequisites</span></span>
<span data-ttu-id="94030-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="94030-104">The following **scopes** are required to execute this API:</span></span> 

<span data-ttu-id="94030-105">*Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="94030-105">*Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="94030-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94030-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/<id>/details
```
## <a name="optional-request-headers"></a><span data-ttu-id="94030-107">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="94030-107">Optional request headers</span></span>
| <span data-ttu-id="94030-108">Nome</span><span class="sxs-lookup"><span data-stu-id="94030-108">Name</span></span>       | <span data-ttu-id="94030-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="94030-109">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="94030-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="94030-110">Authorization</span></span>  | <span data-ttu-id="94030-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94030-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="94030-113">If-Match</span><span class="sxs-lookup"><span data-stu-id="94030-113">If-Match</span></span>  | <span data-ttu-id="94030-p102">O último valor ETag conhecido do objeto **plannerTaskDetails** a ser atualizado. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94030-p102">Last known ETag value for the **plannerTaskDetails** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="94030-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94030-116">Request body</span></span>
<span data-ttu-id="94030-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="94030-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="94030-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="94030-120">Property</span></span>     | <span data-ttu-id="94030-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="94030-121">Type</span></span>   |<span data-ttu-id="94030-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="94030-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94030-123">lista de verificação</span><span class="sxs-lookup"><span data-stu-id="94030-123">checklist</span></span>|[<span data-ttu-id="94030-124">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="94030-124">plannerChecklistItems</span></span>](../resources/plannerchecklistitems.md)|<span data-ttu-id="94030-125">A coleção de itens da lista de verificação na tarefa.</span><span class="sxs-lookup"><span data-stu-id="94030-125">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="94030-126">description</span><span class="sxs-lookup"><span data-stu-id="94030-126">description</span></span>|<span data-ttu-id="94030-127">String</span><span class="sxs-lookup"><span data-stu-id="94030-127">String</span></span>|<span data-ttu-id="94030-128">Descrição da tarefa</span><span class="sxs-lookup"><span data-stu-id="94030-128">Description of the task</span></span>|
|<span data-ttu-id="94030-129">previewType</span><span class="sxs-lookup"><span data-stu-id="94030-129">previewType</span></span>|<span data-ttu-id="94030-130">string</span><span class="sxs-lookup"><span data-stu-id="94030-130">string</span></span>|<span data-ttu-id="94030-p104">Isso define o tipo de visualização que aparece na tarefa. Os valores possíveis são: `automatic`, `noPreview`, `checklist`, `description` e `reference`. Quando definido como `automatic`, a visualização exibida é escolhida pelo aplicativo que exibe a tarefa.</span><span class="sxs-lookup"><span data-stu-id="94030-p104">This sets the type of preview that shows up on the task. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`. When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="94030-134">referências</span><span class="sxs-lookup"><span data-stu-id="94030-134">references</span></span>|[<span data-ttu-id="94030-135">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="94030-135">plannerExternalReferences</span></span>](../resources/plannerexternalreferences.md)|<span data-ttu-id="94030-136">A coleção de referências na tarefa.</span><span class="sxs-lookup"><span data-stu-id="94030-136">The collection of references on the task.</span></span>|

## <a name="response"></a><span data-ttu-id="94030-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="94030-137">Response</span></span>

<span data-ttu-id="94030-138">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [plannerTaskDetails](../resources/plannertaskdetails.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94030-138">If successful, this method returns a `200 OK` response code and updated [plannerTaskDetails](../resources/plannertaskdetails.md) object in the response body.</span></span>

<span data-ttu-id="94030-p105">Este método pode retornar qualquer um dos [códigos de status de HTTP](../../../concepts/errors.md). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner_overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="94030-p105">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="94030-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="94030-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="94030-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94030-143">Request</span></span>
<span data-ttu-id="94030-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="94030-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannertaskdetails"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/tasks/gcrYAaAkgU2EQUvpkNNXLGQAGTtu/details
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
##### <a name="response"></a><span data-ttu-id="94030-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="94030-145">Response</span></span>
<span data-ttu-id="94030-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="94030-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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