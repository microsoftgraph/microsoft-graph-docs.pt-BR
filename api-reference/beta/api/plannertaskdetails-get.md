---
title: Obter plannerTaskDetails
description: Recupere as propriedades e os relacionamentos do objeto **plannertaskdetails** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 35108884c49fccc1af8cdd6fc8b2c55c66d0b69b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36361405"
---
# <a name="get-plannertaskdetails"></a><span data-ttu-id="6a16e-103">Obter plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="6a16e-103">Get plannerTaskDetails</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a16e-104">Recupere as propriedades e os relacionamentos do objeto **plannertaskdetails** .</span><span class="sxs-lookup"><span data-stu-id="6a16e-104">Retrieve the properties and relationships of **plannertaskdetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6a16e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6a16e-105">Permissions</span></span>
<span data-ttu-id="6a16e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a16e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a16e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a16e-108">Permission type</span></span>      | <span data-ttu-id="6a16e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6a16e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a16e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a16e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6a16e-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a16e-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6a16e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a16e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a16e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a16e-113">Not supported.</span></span>    |
|<span data-ttu-id="6a16e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6a16e-114">Application</span></span> | <span data-ttu-id="6a16e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a16e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6a16e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a16e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/<id>/details
```

## <a name="request-headers"></a><span data-ttu-id="6a16e-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6a16e-117">Request headers</span></span>
| <span data-ttu-id="6a16e-118">Nome</span><span class="sxs-lookup"><span data-stu-id="6a16e-118">Name</span></span>      |<span data-ttu-id="6a16e-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a16e-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6a16e-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="6a16e-120">Authorization</span></span>  | <span data-ttu-id="6a16e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a16e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6a16e-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6a16e-123">Request body</span></span>
<span data-ttu-id="6a16e-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6a16e-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a16e-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a16e-125">Response</span></span>

<span data-ttu-id="6a16e-126">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [plannerTaskDetails](../resources/plannertaskdetails.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6a16e-126">If successful, this method returns a `200 OK` response code and [plannerTaskDetails](../resources/plannertaskdetails.md) object in the response body.</span></span>

<span data-ttu-id="6a16e-127">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors).</span><span class="sxs-lookup"><span data-stu-id="6a16e-127">This method can return any of the [HTTP status codes](/graph/errors).</span></span> <span data-ttu-id="6a16e-128">Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404.</span><span class="sxs-lookup"><span data-stu-id="6a16e-128">The most common errors that apps should handle for this method are the 403 and 404 responses.</span></span> <span data-ttu-id="6a16e-129">Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="6a16e-129">For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="6a16e-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6a16e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6a16e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a16e-131">Request</span></span>
<span data-ttu-id="6a16e-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6a16e-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6a16e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="6a16e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plannertaskdetails"
}-->
```http
GET https://graph.microsoft.com/beta/planner/tasks/gcrYAaAkgU2EQUvpkNNXLGQAGTtu/details
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6a16e-134">C#</span><span class="sxs-lookup"><span data-stu-id="6a16e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plannertaskdetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6a16e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6a16e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plannertaskdetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6a16e-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="6a16e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plannertaskdetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6a16e-137">Java</span><span class="sxs-lookup"><span data-stu-id="6a16e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-plannertaskdetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6a16e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a16e-138">Response</span></span>
<span data-ttu-id="6a16e-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6a16e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get plannerTaskDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
