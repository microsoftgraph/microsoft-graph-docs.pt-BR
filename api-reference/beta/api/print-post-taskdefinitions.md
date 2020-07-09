---
title: Criar taskDefinition
description: Criar uma nova definição de tarefa.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 147e1271ee0f5bcd7c04e167e172c48939a4da98
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091552"
---
# <a name="create-taskdefinition"></a><span data-ttu-id="b369c-103">Criar taskDefinition</span><span class="sxs-lookup"><span data-stu-id="b369c-103">Create taskDefinition</span></span>

<span data-ttu-id="b369c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b369c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b369c-105">Criar uma nova definição de tarefa.</span><span class="sxs-lookup"><span data-stu-id="b369c-105">Create a new task definition.</span></span>

<span data-ttu-id="b369c-106">Para obter detalhes sobre como usar essa API para adicionar suporte à impressão pull à impressão universal, consulte [Estendeing universal print to support pull Printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="b369c-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="b369c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b369c-107">Permissions</span></span>
<span data-ttu-id="b369c-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="b369c-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="b369c-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b369c-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="b369c-110">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="b369c-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="b369c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b369c-111">Permission type</span></span> | <span data-ttu-id="b369c-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b369c-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="b369c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b369c-113">Delegated (work or school account)</span></span>| <span data-ttu-id="b369c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b369c-114">Not supported.</span></span> |
|<span data-ttu-id="b369c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b369c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b369c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b369c-116">Not Supported.</span></span>|
|<span data-ttu-id="b369c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b369c-117">Application</span></span>| <span data-ttu-id="b369c-118">PrintTaskDefinition. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b369c-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b369c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b369c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/taskDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="b369c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b369c-120">Request headers</span></span>
| <span data-ttu-id="b369c-121">Nome</span><span class="sxs-lookup"><span data-stu-id="b369c-121">Name</span></span>      |<span data-ttu-id="b369c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b369c-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b369c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b369c-123">Authorization</span></span> | <span data-ttu-id="b369c-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="b369c-124">Bearer {token}.</span></span> <span data-ttu-id="b369c-125">Required.</span><span class="sxs-lookup"><span data-stu-id="b369c-125">Required.</span></span> |
| <span data-ttu-id="b369c-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="b369c-126">Content-type</span></span>  | <span data-ttu-id="b369c-127">application/json.</span><span class="sxs-lookup"><span data-stu-id="b369c-127">application/json.</span></span> <span data-ttu-id="b369c-128">Required.</span><span class="sxs-lookup"><span data-stu-id="b369c-128">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b369c-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b369c-129">Request body</span></span>
<span data-ttu-id="b369c-130">No corpo da solicitação, forneça uma representação JSON do objeto [printTaskDefinition](../resources/printtaskdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="b369c-130">In the request body, supply a JSON representation of [printTaskDefinition](../resources/printtaskdefinition.md) object.</span></span>

<span data-ttu-id="b369c-131">As propriedades **ID** e **createdBy. AppID** do [printTaskDefinition](../resources/printtaskdefinition.md)são definidas automaticamente na criação de recurso.</span><span class="sxs-lookup"><span data-stu-id="b369c-131">The [printTaskDefinition](../resources/printtaskdefinition.md)'s **id** and **createdBy.appId** properties are set automatically upon resource creation.</span></span>

## <a name="response"></a><span data-ttu-id="b369c-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="b369c-132">Response</span></span>
<span data-ttu-id="b369c-133">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [printTaskDefinition](../resources/printtaskdefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b369c-133">If successful, this method returns a `201 Created` response code and a [printTaskDefinition](../resources/printtaskdefinition.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b369c-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b369c-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="b369c-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b369c-135">Request</span></span>
<span data-ttu-id="b369c-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b369c-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "print_create_taskdefinition"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/beta/print/taskDefinitions
Content-type: application/json
Content-length: 122

{
  "displayName": "Test TaskDefinitionName",
  "createdBy": {
    "displayName": "Requesting App Display Name"
  }
}
```

---

### <a name="response"></a><span data-ttu-id="b369c-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="b369c-137">Response</span></span>
<span data-ttu-id="b369c-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b369c-138">The following is an example of the response.</span></span>
><span data-ttu-id="b369c-139">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="b369c-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b369c-140">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="b369c-140">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskDefinition"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 322

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/taskDefinitions/$entity",
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
  "description": "Create taskDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
