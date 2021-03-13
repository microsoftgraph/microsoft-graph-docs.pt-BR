---
title: Criar printTaskDefinition
description: Crie uma nova definição de tarefa.
author: nilakhan
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: ee7172c76863cb62a24c44ba73de2f02bb27e30c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772209"
---
# <a name="create-printtaskdefinition"></a><span data-ttu-id="b75b3-103">Criar printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="b75b3-103">Create printTaskDefinition</span></span>
<span data-ttu-id="b75b3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b75b3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="b75b3-105">Crie uma nova definição de tarefa.</span><span class="sxs-lookup"><span data-stu-id="b75b3-105">Create a new task definition.</span></span>

<span data-ttu-id="b75b3-106">Para obter detalhes sobre como usar essa API para adicionar suporte à impressão pull à Impressão Universal, consulte [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="b75b3-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="b75b3-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b75b3-107">Permissions</span></span>
<span data-ttu-id="b75b3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b75b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="b75b3-110">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa.</span><span class="sxs-lookup"><span data-stu-id="b75b3-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="b75b3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b75b3-111">Permission type</span></span> | <span data-ttu-id="b75b3-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b75b3-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="b75b3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b75b3-113">Delegated (work or school account)</span></span>| <span data-ttu-id="b75b3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b75b3-114">Not supported.</span></span> |
|<span data-ttu-id="b75b3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b75b3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b75b3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b75b3-116">Not Supported.</span></span>|
|<span data-ttu-id="b75b3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b75b3-117">Application</span></span>| <span data-ttu-id="b75b3-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b75b3-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b75b3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b75b3-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/taskDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="b75b3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b75b3-120">Request headers</span></span>
|<span data-ttu-id="b75b3-121">Nome</span><span class="sxs-lookup"><span data-stu-id="b75b3-121">Name</span></span>|<span data-ttu-id="b75b3-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b75b3-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b75b3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b75b3-123">Authorization</span></span>|<span data-ttu-id="b75b3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b75b3-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b75b3-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b75b3-126">Content-Type</span></span>|<span data-ttu-id="b75b3-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b75b3-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b75b3-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b75b3-129">Request body</span></span>
<span data-ttu-id="b75b3-130">No corpo da solicitação, fornece uma representação JSON do [objeto printTaskDefinition.](../resources/printtaskdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b75b3-130">In the request body, supply a JSON representation of [printTaskDefinition](../resources/printtaskdefinition.md) object.</span></span>

<span data-ttu-id="b75b3-131">As **propriedades id** e **createdBy.appId** do [objeto printTaskDefinition](../resources/printtaskdefinition.md) são definidas automaticamente após a criação do recurso.</span><span class="sxs-lookup"><span data-stu-id="b75b3-131">The **id** and **createdBy.appId** properties of the [printTaskDefinition](../resources/printtaskdefinition.md) object are set automatically upon resource creation.</span></span>

## <a name="response"></a><span data-ttu-id="b75b3-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="b75b3-132">Response</span></span>

<span data-ttu-id="b75b3-133">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto printTaskDefinition](../resources/printtaskdefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b75b3-133">If successful, this method returns a `201 Created` response code and a [printTaskDefinition](../resources/printtaskdefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b75b3-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b75b3-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b75b3-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b75b3-135">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b75b3-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="b75b3-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_printtaskdefinition_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/taskDefinitions
Content-Type: application/json
Content-length: 163

{
  "displayName": "Test TaskDefinitionName",
  "createdBy": {
    "displayName": "Requesting App Display Name"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="b75b3-137">C#</span><span class="sxs-lookup"><span data-stu-id="b75b3-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-printtaskdefinition-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b75b3-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b75b3-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-printtaskdefinition-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b75b3-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b75b3-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-printtaskdefinition-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b75b3-140">Java</span><span class="sxs-lookup"><span data-stu-id="b75b3-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-printtaskdefinition-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="b75b3-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="b75b3-141">Response</span></span>
<span data-ttu-id="b75b3-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b75b3-142">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskDefinition"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/taskDefinitions/$entity",
  "id": "fab143fd-ee61-4358-8558-2c7dee953982",
  "displayName": "Test TaskDefinitionName",
  "createdBy": {
    "appId": "815f204f-c791-4ee6-9098-614ecdb003f6",
    "displayName": "Requesting App Display Name"
  }
}
```

