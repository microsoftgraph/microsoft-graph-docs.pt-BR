---
title: Criar plannerBucket
description: Use essa API para criar um novo **plannerBucket**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 8baf98de9431c0627edfcf4adb8c04a16bc2a77f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525707"
---
# <a name="create-plannerbucket"></a><span data-ttu-id="ca8a0-103">Criar plannerBucket</span><span class="sxs-lookup"><span data-stu-id="ca8a0-103">Create plannerBucket</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca8a0-104">Use essa API para criar um novo **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="ca8a0-104">Use this API to create a new **plannerBucket**.</span></span>

## <a name="permissions"></a><span data-ttu-id="ca8a0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ca8a0-105">Permissions</span></span>
<span data-ttu-id="ca8a0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca8a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca8a0-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ca8a0-108">Permission type</span></span>      | <span data-ttu-id="ca8a0-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ca8a0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ca8a0-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ca8a0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ca8a0-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca8a0-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ca8a0-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ca8a0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca8a0-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca8a0-113">Not supported.</span></span>    |
|<span data-ttu-id="ca8a0-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ca8a0-114">Application</span></span> | <span data-ttu-id="ca8a0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca8a0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca8a0-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ca8a0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /planner/buckets

```
## <a name="request-headers"></a><span data-ttu-id="ca8a0-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ca8a0-117">Request headers</span></span>
| <span data-ttu-id="ca8a0-118">Nome</span><span class="sxs-lookup"><span data-stu-id="ca8a0-118">Name</span></span>       | <span data-ttu-id="ca8a0-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca8a0-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ca8a0-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="ca8a0-120">Authorization</span></span>  | <span data-ttu-id="ca8a0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ca8a0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ca8a0-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ca8a0-123">Request body</span></span>
<span data-ttu-id="ca8a0-124">No corpo da solicitação, forneça uma representação JSON do objeto [plannerBucket](../resources/plannerbucket.md).</span><span class="sxs-lookup"><span data-stu-id="ca8a0-124">In the request body, supply a JSON representation of [plannerBucket](../resources/plannerbucket.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ca8a0-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca8a0-125">Response</span></span>

<span data-ttu-id="ca8a0-126">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [plannerBucket](../resources/plannerbucket.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ca8a0-126">If successful, this method returns `201 Created` response code and [plannerBucket](../resources/plannerbucket.md) object in the response body.</span></span>

<span data-ttu-id="ca8a0-p103">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403 e 404. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="ca8a0-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="ca8a0-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ca8a0-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ca8a0-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca8a0-131">Request</span></span>
<span data-ttu-id="ca8a0-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ca8a0-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_plannerbucket_from_planner"
}-->
```http
POST https://graph.microsoft.com/beta/planner/buckets
Content-type: application/json
Content-length: 92

{
  "name": "Advertising",
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "orderHint": " !"
}
```
<span data-ttu-id="ca8a0-133">No corpo da solicitação, forneça uma representação JSON do objeto [plannerBucket](../resources/plannerbucket.md).</span><span class="sxs-lookup"><span data-stu-id="ca8a0-133">In the request body, supply a JSON representation of [plannerBucket](../resources/plannerbucket.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ca8a0-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca8a0-134">Response</span></span>
<span data-ttu-id="ca8a0-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ca8a0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucket"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 145

{
  "name": "Advertising",
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "orderHint": "85752723360752+",
  "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create plannerBucket",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/planner-post-buckets.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
