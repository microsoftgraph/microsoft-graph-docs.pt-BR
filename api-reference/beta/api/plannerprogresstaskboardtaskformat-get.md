---
title: Get plannerProgressTaskBoardTaskFormat
description: Recupere as propriedades e os relacionamentos do objeto **plannerProgressTaskBoardTaskFormat**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 4100d7d5e2f5f12f22508c87433738737aa8d054
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510068"
---
# <a name="get-plannerprogresstaskboardtaskformat"></a><span data-ttu-id="e76ec-103">Get plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="e76ec-103">Get plannerProgressTaskBoardTaskFormat</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e76ec-104">Recupere as propriedades e os relacionamentos do objeto **plannerProgressTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="e76ec-104">Retrieve the properties and relationships of **plannerProgressTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e76ec-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e76ec-105">Permissions</span></span>
<span data-ttu-id="e76ec-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e76ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e76ec-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e76ec-108">Permission type</span></span>      | <span data-ttu-id="e76ec-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e76ec-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e76ec-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e76ec-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e76ec-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e76ec-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e76ec-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e76ec-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e76ec-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e76ec-113">Not supported.</span></span>    |
|<span data-ttu-id="e76ec-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e76ec-114">Application</span></span> | <span data-ttu-id="e76ec-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e76ec-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e76ec-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e76ec-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/<id>/progressTaskBoardFormat
```

## <a name="request-headers"></a><span data-ttu-id="e76ec-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e76ec-117">Request headers</span></span>
| <span data-ttu-id="e76ec-118">Nome</span><span class="sxs-lookup"><span data-stu-id="e76ec-118">Name</span></span>      |<span data-ttu-id="e76ec-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="e76ec-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e76ec-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="e76ec-120">Authorization</span></span>  | <span data-ttu-id="e76ec-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e76ec-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e76ec-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e76ec-123">Request body</span></span>
<span data-ttu-id="e76ec-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e76ec-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e76ec-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="e76ec-125">Response</span></span>

<span data-ttu-id="e76ec-126">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e76ec-126">If successful, this method returns a `200 OK` response code and [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="e76ec-p103">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="e76ec-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="e76ec-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e76ec-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e76ec-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e76ec-131">Request</span></span>
<span data-ttu-id="e76ec-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e76ec-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannerprogresstaskboardtaskformat"
}-->
```http
GET https://graph.microsoft.com/beta/planner/tasks/<id>/progressTaskBoardFormat
```
##### <a name="response"></a><span data-ttu-id="e76ec-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e76ec-133">Response</span></span>
<span data-ttu-id="e76ec-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e76ec-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerProgressTaskBoardTaskFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 76

{
  "id": "01gzSlKkIUSUl6DF_EilrmQAKDhh",
  "orderHint": "85752723360752+"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get plannerProgressTaskBoardTaskFormat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/plannerprogresstaskboardtaskformat-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
