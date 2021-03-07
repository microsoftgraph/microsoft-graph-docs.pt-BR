---
title: Excluir taskDefinition
description: Excluir uma definição de tarefa.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 457ebc3ba3f2e125b5d252c138ed08b28d3e0798
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516837"
---
# <a name="delete-printtaskdefinition"></a><span data-ttu-id="069cf-103">Excluir printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="069cf-103">Delete printTaskDefinition</span></span>
<span data-ttu-id="069cf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="069cf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="069cf-105">Excluir uma **tarefaDefinition**.</span><span class="sxs-lookup"><span data-stu-id="069cf-105">Delete a **taskDefinition**.</span></span>

<span data-ttu-id="069cf-106">Para obter detalhes sobre como usar essa API para adicionar suporte à impressão pull à Impressão Universal, consulte [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="069cf-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="069cf-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="069cf-107">Permissions</span></span>
<span data-ttu-id="069cf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="069cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="069cf-110">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa.</span><span class="sxs-lookup"><span data-stu-id="069cf-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="069cf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="069cf-111">Permission type</span></span> | <span data-ttu-id="069cf-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="069cf-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="069cf-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="069cf-113">Delegated (work or school account)</span></span>| <span data-ttu-id="069cf-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="069cf-114">Not supported.</span></span> |
|<span data-ttu-id="069cf-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="069cf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="069cf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="069cf-116">Not Supported.</span></span>|
|<span data-ttu-id="069cf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="069cf-117">Application</span></span>| <span data-ttu-id="069cf-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="069cf-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="069cf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="069cf-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /print/taskDefinitions/{printTaskDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="069cf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="069cf-120">Request headers</span></span>
|<span data-ttu-id="069cf-121">Nome</span><span class="sxs-lookup"><span data-stu-id="069cf-121">Name</span></span>|<span data-ttu-id="069cf-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="069cf-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="069cf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="069cf-123">Authorization</span></span>|<span data-ttu-id="069cf-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="069cf-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="069cf-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="069cf-126">Request body</span></span>
<span data-ttu-id="069cf-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="069cf-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="069cf-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="069cf-128">Response</span></span>
<span data-ttu-id="069cf-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="069cf-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="069cf-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="069cf-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="069cf-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="069cf-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_printtaskdefinition"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/print/taskDefinitions/{printTaskDefinitionId}
```


### <a name="response"></a><span data-ttu-id="069cf-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="069cf-133">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

