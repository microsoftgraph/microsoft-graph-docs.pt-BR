---
title: Obter plannerTaskDetails
description: Recupere as propriedades e os relacionamentos do objeto **plannertaskdetails** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 77920e12c3c3563fc9af739be8c68fe83d558557
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32546864"
---
# <a name="get-plannertaskdetails"></a><span data-ttu-id="9b665-103">Obter plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="9b665-103">Get plannerTaskDetails</span></span>

<span data-ttu-id="9b665-104">Recupere as propriedades e os relacionamentos do objeto **plannertaskdetails** .</span><span class="sxs-lookup"><span data-stu-id="9b665-104">Retrieve the properties and relationships of **plannertaskdetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9b665-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9b665-105">Permissions</span></span>
<span data-ttu-id="9b665-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b665-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b665-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9b665-108">Permission type</span></span>      | <span data-ttu-id="9b665-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9b665-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9b665-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9b665-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9b665-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b665-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9b665-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9b665-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b665-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b665-113">Not supported.</span></span>    |
|<span data-ttu-id="9b665-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9b665-114">Application</span></span> | <span data-ttu-id="9b665-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b665-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9b665-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9b665-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/{id}/details
```

## <a name="request-headers"></a><span data-ttu-id="9b665-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9b665-117">Request headers</span></span>
| <span data-ttu-id="9b665-118">Nome</span><span class="sxs-lookup"><span data-stu-id="9b665-118">Name</span></span>      |<span data-ttu-id="9b665-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b665-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9b665-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="9b665-120">Authorization</span></span>  | <span data-ttu-id="9b665-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9b665-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9b665-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9b665-123">Request body</span></span>
<span data-ttu-id="9b665-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9b665-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b665-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b665-125">Response</span></span>

<span data-ttu-id="9b665-126">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [plannerTaskDetails](../resources/plannertaskdetails.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9b665-126">If successful, this method returns a `200 OK` response code and [plannerTaskDetails](../resources/plannertaskdetails.md) object in the response body.</span></span>

<span data-ttu-id="9b665-127">Este método pode retornar qualquer um dos [códigos de status http](/graph/errors).</span><span class="sxs-lookup"><span data-stu-id="9b665-127">This method can return any of the [HTTP status codes](/graph/errors).</span></span> <span data-ttu-id="9b665-128">Os erros mais comuns que os aplicativos devem lidar com esse método são as respostas 403 e 404.</span><span class="sxs-lookup"><span data-stu-id="9b665-128">The most common errors that apps should handle for this method are the 403 and 404 responses.</span></span> <span data-ttu-id="9b665-129">Para obter mais informações sobre esses erros, confira [condições de erro do planejador comum](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="9b665-129">For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="9b665-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9b665-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9b665-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9b665-131">Request</span></span>
<span data-ttu-id="9b665-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9b665-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannertaskdetails"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/tasks/{task-id}/details
```
##### <a name="response"></a><span data-ttu-id="9b665-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b665-133">Response</span></span>
<span data-ttu-id="9b665-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9b665-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTaskDetails"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1036

{
  "description": "Task details properties:\nchecklist:Sub items\nreferences:Related links",
  "previewType": "automatic",
  "references": {
    "https%3A//developer%2Emicrosoft%2Ecom/en-us/graph/graph-explorer": {
      "@odata.type": "#microsoft.graph.plannerExternalReference",
      "alias": "Graph Explorer",
      "type": "Other",
      "previewPriority": "0009005706180391122",
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
      "isChecked": false,
      "title": "Try reading task details",
      "orderHint": "8587094707721254251P]",
      "lastModifiedBy": {
        "user": {
          "id": "e396de0e-4812-4fcb-9f9e-0358744df343"
        }
      },
      "lastModifiedDateTime": "2017-04-14T02:16:14.866Z"
    }
  },
  "id": "gcrYAaAkgU2EQUvpkNNXLGQAGTtu"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerTaskDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
