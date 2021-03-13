---
title: Excluir printConnector
description: Excluir (não registro) um printConnector.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 71edae5cf61e9e3ab7e9d8ec8b36ed679d0c04f6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772153"
---
# <a name="delete-printconnector"></a><span data-ttu-id="f8a91-103">Excluir printConnector</span><span class="sxs-lookup"><span data-stu-id="f8a91-103">Delete printConnector</span></span>
<span data-ttu-id="f8a91-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8a91-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="f8a91-105">Excluir (não registro) um **printConnector**.</span><span class="sxs-lookup"><span data-stu-id="f8a91-105">Delete (unregister) a **printConnector**.</span></span>

## <a name="permissions"></a><span data-ttu-id="f8a91-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="f8a91-106">Permissions</span></span>
<span data-ttu-id="f8a91-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8a91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="f8a91-109">Para usar o serviço Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="f8a91-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="f8a91-110">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="f8a91-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="f8a91-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f8a91-111">Permission type</span></span> | <span data-ttu-id="f8a91-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f8a91-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="f8a91-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f8a91-113">Delegated (work or school account)</span></span>| <span data-ttu-id="f8a91-114">PrintConnector.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8a91-114">PrintConnector.ReadWrite.All</span></span> |
|<span data-ttu-id="f8a91-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f8a91-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8a91-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8a91-116">Not Supported.</span></span>|
|<span data-ttu-id="f8a91-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f8a91-117">Application</span></span>|<span data-ttu-id="f8a91-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8a91-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8a91-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f8a91-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /print/connectors/{printConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="f8a91-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f8a91-120">Request headers</span></span>
|<span data-ttu-id="f8a91-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f8a91-121">Name</span></span>|<span data-ttu-id="f8a91-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8a91-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f8a91-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f8a91-123">Authorization</span></span>|<span data-ttu-id="f8a91-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f8a91-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8a91-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f8a91-126">Request body</span></span>
<span data-ttu-id="f8a91-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f8a91-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8a91-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8a91-128">Response</span></span>
<span data-ttu-id="f8a91-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f8a91-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

### <a name="error-conditions-and-messages"></a><span data-ttu-id="f8a91-131">Condições de erro e mensagens</span><span class="sxs-lookup"><span data-stu-id="f8a91-131">Error conditions and messages</span></span>

|<span data-ttu-id="f8a91-132">Cenário</span><span class="sxs-lookup"><span data-stu-id="f8a91-132">Scenario</span></span>|<span data-ttu-id="f8a91-133">Método</span><span class="sxs-lookup"><span data-stu-id="f8a91-133">Method</span></span>|<span data-ttu-id="f8a91-134">Código</span><span class="sxs-lookup"><span data-stu-id="f8a91-134">Code</span></span>|<span data-ttu-id="f8a91-135">Mensagem</span><span class="sxs-lookup"><span data-stu-id="f8a91-135">Message</span></span>|
|--------|------|----|-------|
|<span data-ttu-id="f8a91-136">O usuário tenta excluir um conector que tenha uma ou mais impressoras registradas</span><span class="sxs-lookup"><span data-stu-id="f8a91-136">User attempts to delete a connector that has one or more printers registered</span></span>|<span data-ttu-id="f8a91-137">DELETE</span><span class="sxs-lookup"><span data-stu-id="f8a91-137">DELETE</span></span>|<span data-ttu-id="f8a91-138">409</span><span class="sxs-lookup"><span data-stu-id="f8a91-138">409</span></span>|<span data-ttu-id="f8a91-139">Antes de excluir o conector, desassocie o registro das impressoras associadas.</span><span class="sxs-lookup"><span data-stu-id="f8a91-139">Before deleting the connector, please unregister the associated printers.</span></span>|

## <a name="examples"></a><span data-ttu-id="f8a91-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f8a91-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f8a91-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f8a91-141">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f8a91-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="f8a91-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_printconnector"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/print/connectors/{printConnectorId}
```
# <a name="c"></a>[<span data-ttu-id="f8a91-143">C#</span><span class="sxs-lookup"><span data-stu-id="f8a91-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-printconnector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f8a91-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f8a91-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-printconnector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f8a91-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f8a91-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-printconnector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f8a91-146">Java</span><span class="sxs-lookup"><span data-stu-id="f8a91-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-printconnector-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="f8a91-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8a91-147">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

