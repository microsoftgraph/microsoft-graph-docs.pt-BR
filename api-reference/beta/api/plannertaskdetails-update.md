---
title: Atualizar plannertaskdetails
description: Atualize as propriedades do objeto **plannertaskdetails**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 04adf9c53907962f0298541f5d8c28402bc2b613
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960550"
---
# <a name="update-plannertaskdetails"></a><span data-ttu-id="fbc02-103">Atualizar plannertaskdetails</span><span class="sxs-lookup"><span data-stu-id="fbc02-103">Update plannertaskdetails</span></span>

> <span data-ttu-id="fbc02-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fbc02-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fbc02-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fbc02-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fbc02-106">Atualize as propriedades do objeto **plannertaskdetails**.</span><span class="sxs-lookup"><span data-stu-id="fbc02-106">Update the properties of **plannertaskdetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="fbc02-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="fbc02-107">Permissions</span></span>
<span data-ttu-id="fbc02-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbc02-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbc02-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fbc02-110">Permission type</span></span>      | <span data-ttu-id="fbc02-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fbc02-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fbc02-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fbc02-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fbc02-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbc02-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="fbc02-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fbc02-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fbc02-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fbc02-115">Not supported.</span></span>    |
|<span data-ttu-id="fbc02-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fbc02-116">Application</span></span> | <span data-ttu-id="fbc02-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fbc02-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fbc02-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fbc02-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/<id>/details
```
## <a name="optional-request-headers"></a><span data-ttu-id="fbc02-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="fbc02-119">Optional request headers</span></span>
| <span data-ttu-id="fbc02-120">Nome</span><span class="sxs-lookup"><span data-stu-id="fbc02-120">Name</span></span>       | <span data-ttu-id="fbc02-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbc02-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="fbc02-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fbc02-122">Authorization</span></span>  | <span data-ttu-id="fbc02-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fbc02-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fbc02-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="fbc02-125">If-Match</span></span>  | <span data-ttu-id="fbc02-p104">O último valor ETag conhecido do objeto **plannerTaskDetails** a ser atualizado. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fbc02-p104">Last known ETag value for the **plannerTaskDetails** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fbc02-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fbc02-128">Request body</span></span>
<span data-ttu-id="fbc02-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="fbc02-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="fbc02-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fbc02-132">Property</span></span>     | <span data-ttu-id="fbc02-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="fbc02-133">Type</span></span>   |<span data-ttu-id="fbc02-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbc02-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fbc02-135">lista de verificação</span><span class="sxs-lookup"><span data-stu-id="fbc02-135">checklist</span></span>|[<span data-ttu-id="fbc02-136">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="fbc02-136">plannerChecklistItems</span></span>](../resources/plannerchecklistitems.md)|<span data-ttu-id="fbc02-137">A coleção de itens da lista de verificação na tarefa.</span><span class="sxs-lookup"><span data-stu-id="fbc02-137">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="fbc02-138">description</span><span class="sxs-lookup"><span data-stu-id="fbc02-138">description</span></span>|<span data-ttu-id="fbc02-139">String</span><span class="sxs-lookup"><span data-stu-id="fbc02-139">String</span></span>|<span data-ttu-id="fbc02-140">Descrição da tarefa</span><span class="sxs-lookup"><span data-stu-id="fbc02-140">Description of the task</span></span>|
|<span data-ttu-id="fbc02-141">previewType</span><span class="sxs-lookup"><span data-stu-id="fbc02-141">previewType</span></span>|<span data-ttu-id="fbc02-142">string</span><span class="sxs-lookup"><span data-stu-id="fbc02-142">string</span></span>|<span data-ttu-id="fbc02-p106">Isso define o tipo de visualização que aparece na tarefa. Os valores possíveis são: `automatic`, `noPreview`, `checklist`, `description` e `reference`. Quando definido como `automatic`, a visualização exibida é escolhida pelo aplicativo que exibe a tarefa.</span><span class="sxs-lookup"><span data-stu-id="fbc02-p106">This sets the type of preview that shows up on the task. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`. When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="fbc02-146">referências</span><span class="sxs-lookup"><span data-stu-id="fbc02-146">references</span></span>|[<span data-ttu-id="fbc02-147">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="fbc02-147">plannerExternalReferences</span></span>](../resources/plannerexternalreferences.md)|<span data-ttu-id="fbc02-148">A coleção de referências na tarefa.</span><span class="sxs-lookup"><span data-stu-id="fbc02-148">The collection of references on the task.</span></span>|

## <a name="response"></a><span data-ttu-id="fbc02-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbc02-149">Response</span></span>

<span data-ttu-id="fbc02-150">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [plannerTaskDetails](../resources/plannertaskdetails.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fbc02-150">If successful, this method returns a `200 OK` response code and updated [plannerTaskDetails](../resources/plannertaskdetails.md) object in the response body.</span></span>

<span data-ttu-id="fbc02-p107">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="fbc02-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="fbc02-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fbc02-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fbc02-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fbc02-155">Request</span></span>
<span data-ttu-id="fbc02-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fbc02-156">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="fbc02-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbc02-157">Response</span></span>
<span data-ttu-id="fbc02-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fbc02-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
