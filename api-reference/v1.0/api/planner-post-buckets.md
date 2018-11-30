---
title: Criar plannerBucket
description: Use essa API para criar um novo **plannerBucket**.
ms.openlocfilehash: 4e766c33e26fdbca15f957bad66781a90a3a0c8d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004159"
---
# <a name="create-plannerbucket"></a><span data-ttu-id="7683e-103">Criar plannerBucket</span><span class="sxs-lookup"><span data-stu-id="7683e-103">Create plannerBucket</span></span>

<span data-ttu-id="7683e-104">Use essa API para criar um novo **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="7683e-104">Use this API to create a new **plannerBucket**.</span></span>

## <a name="permissions"></a><span data-ttu-id="7683e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7683e-105">Permissions</span></span>
<span data-ttu-id="7683e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7683e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7683e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7683e-108">Permission type</span></span>      | <span data-ttu-id="7683e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7683e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7683e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7683e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7683e-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7683e-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7683e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7683e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7683e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7683e-113">Not supported.</span></span>    |
|<span data-ttu-id="7683e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7683e-114">Application</span></span> | <span data-ttu-id="7683e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7683e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7683e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7683e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /planner/buckets

```
## <a name="request-headers"></a><span data-ttu-id="7683e-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7683e-117">Request headers</span></span>
| <span data-ttu-id="7683e-118">Nome</span><span class="sxs-lookup"><span data-stu-id="7683e-118">Name</span></span>       | <span data-ttu-id="7683e-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="7683e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7683e-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="7683e-120">Authorization</span></span>  | <span data-ttu-id="7683e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7683e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7683e-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7683e-123">Request body</span></span>
<span data-ttu-id="7683e-124">No corpo da solicitação, forneça uma representação JSON do objeto [plannerBucket](../resources/plannerbucket.md).</span><span class="sxs-lookup"><span data-stu-id="7683e-124">In the request body, supply a JSON representation of [plannerBucket](../resources/plannerbucket.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7683e-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="7683e-125">Response</span></span>

<span data-ttu-id="7683e-126">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [plannerBucket](../resources/plannerbucket.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7683e-126">If successful, this method returns `201 Created` response code and [plannerBucket](../resources/plannerbucket.md) object in the response body.</span></span>

<span data-ttu-id="7683e-p103">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403 e 404. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="7683e-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="7683e-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7683e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7683e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7683e-131">Request</span></span>
<span data-ttu-id="7683e-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7683e-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_plannerbucket_from_planner"
}-->
```http
POST https://graph.microsoft.com/v1.0/planner/buckets
Content-type: application/json
Content-length: 92

{
  "name": "Advertising",
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "orderHint": " !"
}
```
<span data-ttu-id="7683e-133">No corpo da solicitação, forneça uma representação JSON do objeto [plannerBucket](../resources/plannerbucket.md).</span><span class="sxs-lookup"><span data-stu-id="7683e-133">In the request body, supply a JSON representation of [plannerBucket](../resources/plannerbucket.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="7683e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="7683e-134">Response</span></span>
<span data-ttu-id="7683e-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7683e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create plannerBucket",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->