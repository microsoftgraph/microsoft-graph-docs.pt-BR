---
title: Atualizar printTaskDefinition
description: Atualize uma definição de tarefa.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 98f075e89828a1e07fe3ee04bbed0b95b511b0d5
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516875"
---
# <a name="update-printtaskdefinition"></a><span data-ttu-id="16742-103">Atualizar printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="16742-103">Update printTaskDefinition</span></span>

<span data-ttu-id="16742-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16742-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="16742-105">Atualize uma definição de tarefa.</span><span class="sxs-lookup"><span data-stu-id="16742-105">Update a task definition.</span></span>

<span data-ttu-id="16742-106">Para obter detalhes sobre como usar essa API para adicionar suporte à impressão pull à Impressão Universal, consulte [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="16742-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="16742-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="16742-107">Permissions</span></span>
<span data-ttu-id="16742-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16742-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="16742-110">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa.</span><span class="sxs-lookup"><span data-stu-id="16742-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="16742-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="16742-111">Permission type</span></span> | <span data-ttu-id="16742-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="16742-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="16742-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="16742-113">Delegated (work or school account)</span></span>| <span data-ttu-id="16742-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16742-114">Not supported.</span></span> |
|<span data-ttu-id="16742-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="16742-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16742-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16742-116">Not Supported.</span></span>|
|<span data-ttu-id="16742-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="16742-117">Application</span></span>| <span data-ttu-id="16742-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16742-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="16742-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="16742-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /print/taskDefinitions/{printTaskDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="16742-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="16742-120">Request headers</span></span>
|<span data-ttu-id="16742-121">Nome</span><span class="sxs-lookup"><span data-stu-id="16742-121">Name</span></span>|<span data-ttu-id="16742-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="16742-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="16742-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="16742-123">Authorization</span></span>|<span data-ttu-id="16742-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="16742-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="16742-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="16742-126">Content-Type</span></span>|<span data-ttu-id="16742-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="16742-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="16742-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="16742-129">Request body</span></span>
<span data-ttu-id="16742-130">No corpo da solicitação, fornece os valores para os campos [printTaskDefinition](../resources/printtaskdefinition.md) relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="16742-130">In the request body, supply the values for the relevant [printTaskDefinition](../resources/printtaskdefinition.md) fields that should be updated.</span></span> <span data-ttu-id="16742-131">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="16742-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="16742-132">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="16742-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="16742-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="16742-133">Property</span></span>     | <span data-ttu-id="16742-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="16742-134">Type</span></span>        | <span data-ttu-id="16742-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="16742-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="16742-136">displayName</span><span class="sxs-lookup"><span data-stu-id="16742-136">displayName</span></span>|<span data-ttu-id="16742-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16742-137">String</span></span>|<span data-ttu-id="16742-138">O nome da **printTaskDefinition**.</span><span class="sxs-lookup"><span data-stu-id="16742-138">The name of the **printTaskDefinition**.</span></span>|
|<span data-ttu-id="16742-139">createdBy</span><span class="sxs-lookup"><span data-stu-id="16742-139">createdBy</span></span>|<span data-ttu-id="16742-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16742-140">String</span></span>|<span data-ttu-id="16742-141">Informações sobre o aplicativo que criou a definição de tarefa.</span><span class="sxs-lookup"><span data-stu-id="16742-141">Information about the app that created the task definition.</span></span> <span data-ttu-id="16742-142">Somente a `createdBy.displayName` propriedade pode ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="16742-142">Only the `createdBy.displayName` property can be updated.</span></span>|

## <a name="response"></a><span data-ttu-id="16742-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="16742-143">Response</span></span>

<span data-ttu-id="16742-144">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto printTaskDefinition](../resources/printtaskdefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="16742-144">If successful, this method returns a `200 OK` response code and an updated [printTaskDefinition](../resources/printtaskdefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="16742-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="16742-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="16742-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="16742-146">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_printtaskdefinition"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/print/taskDefinitions/{printTaskDefinitionId}
Content-Type: application/json
Content-length: 163

{
  "displayName": "Test TaskDefinitionName",
  "createdBy": {
    "displayName": "Requesting App Display Name"
  }
}
```

### <a name="response"></a><span data-ttu-id="16742-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="16742-147">Response</span></span>
<span data-ttu-id="16742-148">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="16742-148">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskDefinition"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/taskDefinitions/$entity",
  "id": "fab143fd-ee61-4358-8558-2c7dee953982",
  "displayName": "Test TaskDefinitionName",
  "createdBy": {
    "appId" : "479688a0-cc3a-4993-ab24-54c7c80b047e",
    "displayName": "Requesting App Display Name"
  }
}
```

