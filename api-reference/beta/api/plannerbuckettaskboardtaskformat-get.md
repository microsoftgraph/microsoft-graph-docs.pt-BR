---
title: Get plannerBucketTaskBoardTaskFormat
description: Recupere as propriedades e os relacionamentos do objeto **plannerBucketTaskBoardTaskFormat**.
ms.openlocfilehash: 5a2f0ad97b031ef6e1c45b75b17c816329dfe0ed
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035934"
---
# <a name="get-plannerbuckettaskboardtaskformat"></a><span data-ttu-id="3000f-103">Get plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="3000f-103">Get plannerBucketTaskBoardTaskFormat</span></span>

> <span data-ttu-id="3000f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3000f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3000f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3000f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3000f-106">Recupere as propriedades e os relacionamentos do objeto **plannerBucketTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="3000f-106">Retrieve the properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3000f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="3000f-107">Permissions</span></span>
<span data-ttu-id="3000f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3000f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3000f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3000f-110">Permission type</span></span>      | <span data-ttu-id="3000f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3000f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3000f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3000f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3000f-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3000f-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3000f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3000f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3000f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3000f-115">Not supported.</span></span>    |
|<span data-ttu-id="3000f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3000f-116">Application</span></span> | <span data-ttu-id="3000f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3000f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3000f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3000f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/<id>/bucketTaskBoardFormat
```

## <a name="request-headers"></a><span data-ttu-id="3000f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3000f-119">Request headers</span></span>
| <span data-ttu-id="3000f-120">Nome</span><span class="sxs-lookup"><span data-stu-id="3000f-120">Name</span></span>      |<span data-ttu-id="3000f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="3000f-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3000f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3000f-122">Authorization</span></span>  | <span data-ttu-id="3000f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3000f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3000f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3000f-125">Request body</span></span>
<span data-ttu-id="3000f-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3000f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3000f-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="3000f-127">Response</span></span>

<span data-ttu-id="3000f-128">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3000f-128">If successful, this method returns a `200 OK` response code and [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="3000f-p104">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="3000f-p104">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="3000f-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3000f-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3000f-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3000f-133">Request</span></span>
<span data-ttu-id="3000f-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3000f-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannerbuckettaskboardtaskformat"
}-->
```http
GET https://graph.microsoft.com/beta/planner/tasks/01gzSlKkIUSUl6DF_EilrmQAKDhh/bucketTaskBoardFormat
```
##### <a name="response"></a><span data-ttu-id="3000f-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="3000f-135">Response</span></span>
<span data-ttu-id="3000f-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3000f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucketTaskBoardTaskFormat"
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
  "description": "Get plannerBucketTaskBoardTaskFormat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->