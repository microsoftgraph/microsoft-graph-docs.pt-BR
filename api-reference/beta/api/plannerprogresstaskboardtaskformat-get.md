---
title: Get plannerProgressTaskBoardTaskFormat
description: Recupere as propriedades e os relacionamentos do objeto **plannerProgressTaskBoardTaskFormat**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 9311ee5388c951b72da28d32eefa9b32b0426b95
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950166"
---
# <a name="get-plannerprogresstaskboardtaskformat"></a><span data-ttu-id="9239a-103">Get plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="9239a-103">Get plannerProgressTaskBoardTaskFormat</span></span>

> <span data-ttu-id="9239a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9239a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9239a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9239a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9239a-106">Recupere as propriedades e os relacionamentos do objeto **plannerProgressTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="9239a-106">Retrieve the properties and relationships of **plannerProgressTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9239a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="9239a-107">Permissions</span></span>
<span data-ttu-id="9239a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9239a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9239a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9239a-110">Permission type</span></span>      | <span data-ttu-id="9239a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9239a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9239a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9239a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9239a-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9239a-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9239a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9239a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9239a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9239a-115">Not supported.</span></span>    |
|<span data-ttu-id="9239a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9239a-116">Application</span></span> | <span data-ttu-id="9239a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9239a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9239a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9239a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/<id>/progressTaskBoardFormat
```

## <a name="request-headers"></a><span data-ttu-id="9239a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9239a-119">Request headers</span></span>
| <span data-ttu-id="9239a-120">Nome</span><span class="sxs-lookup"><span data-stu-id="9239a-120">Name</span></span>      |<span data-ttu-id="9239a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9239a-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9239a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9239a-122">Authorization</span></span>  | <span data-ttu-id="9239a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9239a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9239a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9239a-125">Request body</span></span>
<span data-ttu-id="9239a-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9239a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9239a-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="9239a-127">Response</span></span>

<span data-ttu-id="9239a-128">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9239a-128">If successful, this method returns a `200 OK` response code and [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="9239a-p104">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="9239a-p104">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="9239a-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9239a-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9239a-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9239a-133">Request</span></span>
<span data-ttu-id="9239a-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9239a-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannerprogresstaskboardtaskformat"
}-->
```http
GET https://graph.microsoft.com/beta/planner/tasks/<id>/progressTaskBoardFormat
```
##### <a name="response"></a><span data-ttu-id="9239a-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="9239a-135">Response</span></span>
<span data-ttu-id="9239a-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9239a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerProgressTaskBoardTaskFormat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
