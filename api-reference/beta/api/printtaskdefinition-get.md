---
title: Obter taskDefinition
description: Obter detalhes sobre uma definição de tarefa.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 8105fa16971ed468e024291f97b529f2938df96c
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091533"
---
# <a name="get-taskdefinition"></a><span data-ttu-id="e7768-103">Obter taskDefinition</span><span class="sxs-lookup"><span data-stu-id="e7768-103">Get taskDefinition</span></span>

<span data-ttu-id="e7768-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7768-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7768-105">Obter detalhes sobre uma definição de tarefa.</span><span class="sxs-lookup"><span data-stu-id="e7768-105">Get details about a task definition.</span></span>

<span data-ttu-id="e7768-106">Para obter detalhes sobre como usar essa API para adicionar suporte à impressão pull à impressão universal, consulte [Estendeing universal print to support pull Printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="e7768-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="e7768-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e7768-107">Permissions</span></span>
<span data-ttu-id="e7768-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="e7768-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="e7768-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7768-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="e7768-110">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="e7768-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="e7768-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e7768-111">Permission type</span></span> | <span data-ttu-id="e7768-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e7768-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="e7768-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e7768-113">Delegated (work or school account)</span></span>| <span data-ttu-id="e7768-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7768-114">Not supported.</span></span> |
|<span data-ttu-id="e7768-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e7768-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7768-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7768-116">Not Supported.</span></span>|
|<span data-ttu-id="e7768-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e7768-117">Application</span></span>| <span data-ttu-id="e7768-118">PrintTaskDefinition. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e7768-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e7768-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7768-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/taskDefinitions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e7768-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e7768-120">Request headers</span></span>
| <span data-ttu-id="e7768-121">Nome</span><span class="sxs-lookup"><span data-stu-id="e7768-121">Name</span></span>      |<span data-ttu-id="e7768-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7768-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e7768-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7768-123">Authorization</span></span> | <span data-ttu-id="e7768-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="e7768-124">Bearer {token}.</span></span> <span data-ttu-id="e7768-125">Required.</span><span class="sxs-lookup"><span data-stu-id="e7768-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e7768-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e7768-126">Request body</span></span>
<span data-ttu-id="e7768-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e7768-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e7768-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7768-128">Response</span></span>
<span data-ttu-id="e7768-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [printTaskDefinition](../resources/printtaskdefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7768-129">If successful, this method returns a `200 OK` response code and a [printTaskDefinition](../resources/printtaskdefinition.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e7768-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e7768-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="e7768-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7768-131">Request</span></span>
<span data-ttu-id="e7768-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7768-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_taskdefinition"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/taskDefinitions/fab143fd-ee61-4358-8558-2c7dee953982
```

---

### <a name="response"></a><span data-ttu-id="e7768-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7768-133">Response</span></span>
<span data-ttu-id="e7768-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e7768-134">The following is an example of the response.</span></span>
><span data-ttu-id="e7768-135">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="e7768-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e7768-136">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="e7768-136">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskDefinition"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 380

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/taskDefinitions/$entity",
  "@odata.type": "#microsoft.graph.printTaskDefinition",
  "id": "fab143fd-ee61-4358-8558-2c7dee953982",
  "displayName": "Test TaskDefinitionName",
  "createdBy": {
    "appId": "815f204f-c791-4ee6-9098-614ecdb003f6",
    "displayName": "Requesting App Display Name"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get taskDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
