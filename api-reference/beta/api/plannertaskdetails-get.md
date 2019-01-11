---
title: Get plannerTaskDetails
description: Recupere as propriedades e os relacionamentos do objeto **plannertaskdetails**.
localization_priority: Normal
ms.openlocfilehash: 5edf56f2c201ed84ae3c8cb4cb25f9c5cc74b96e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860925"
---
# <a name="get-plannertaskdetails"></a><span data-ttu-id="06458-103">Get plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="06458-103">Get plannerTaskDetails</span></span>

> <span data-ttu-id="06458-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="06458-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06458-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="06458-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="06458-106">Recupere as propriedades e os relacionamentos do objeto **plannertaskdetails**.</span><span class="sxs-lookup"><span data-stu-id="06458-106">Retrieve the properties and relationships of **plannertaskdetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="06458-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="06458-107">Permissions</span></span>
<span data-ttu-id="06458-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06458-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06458-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="06458-110">Permission type</span></span>      | <span data-ttu-id="06458-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="06458-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06458-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="06458-112">Delegated (work or school account)</span></span> | <span data-ttu-id="06458-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06458-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="06458-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="06458-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06458-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06458-115">Not supported.</span></span>    |
|<span data-ttu-id="06458-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="06458-116">Application</span></span> | <span data-ttu-id="06458-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06458-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="06458-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="06458-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/<id>/details
```

## <a name="request-headers"></a><span data-ttu-id="06458-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="06458-119">Request headers</span></span>
| <span data-ttu-id="06458-120">Nome</span><span class="sxs-lookup"><span data-stu-id="06458-120">Name</span></span>      |<span data-ttu-id="06458-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="06458-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="06458-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="06458-122">Authorization</span></span>  | <span data-ttu-id="06458-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="06458-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="06458-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="06458-125">Request body</span></span>
<span data-ttu-id="06458-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="06458-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06458-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="06458-127">Response</span></span>

<span data-ttu-id="06458-128">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [plannerTaskDetails](../resources/plannertaskdetails.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="06458-128">If successful, this method returns a `200 OK` response code and [plannerTaskDetails](../resources/plannertaskdetails.md) object in the response body.</span></span>

<span data-ttu-id="06458-p104">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="06458-p104">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="06458-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="06458-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="06458-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="06458-133">Request</span></span>
<span data-ttu-id="06458-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="06458-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannertaskdetails"
}-->
```http
GET https://graph.microsoft.com/beta/planner/tasks/gcrYAaAkgU2EQUvpkNNXLGQAGTtu/details
```
##### <a name="response"></a><span data-ttu-id="06458-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="06458-135">Response</span></span>
<span data-ttu-id="06458-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="06458-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
