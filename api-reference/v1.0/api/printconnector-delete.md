---
title: Excluir printConnector
description: Excluir (não registro) um printConnector.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 4366aa9f3ab674861c404a4ce0f9c329a06b23e9
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516868"
---
# <a name="delete-printconnector"></a><span data-ttu-id="c9577-103">Excluir printConnector</span><span class="sxs-lookup"><span data-stu-id="c9577-103">Delete printConnector</span></span>
<span data-ttu-id="c9577-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9577-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="c9577-105">Excluir (não registro) um **printConnector**.</span><span class="sxs-lookup"><span data-stu-id="c9577-105">Delete (unregister) a **printConnector**.</span></span>

## <a name="permissions"></a><span data-ttu-id="c9577-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c9577-106">Permissions</span></span>
<span data-ttu-id="c9577-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9577-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c9577-109">Para usar o serviço Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="c9577-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="c9577-110">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="c9577-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="c9577-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c9577-111">Permission type</span></span> | <span data-ttu-id="c9577-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c9577-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="c9577-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c9577-113">Delegated (work or school account)</span></span>| <span data-ttu-id="c9577-114">PrintConnector.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9577-114">PrintConnector.ReadWrite.All</span></span> |
|<span data-ttu-id="c9577-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c9577-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9577-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c9577-116">Not Supported.</span></span>|
|<span data-ttu-id="c9577-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c9577-117">Application</span></span>|<span data-ttu-id="c9577-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c9577-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9577-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c9577-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /print/connectors/{printConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="c9577-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c9577-120">Request headers</span></span>
|<span data-ttu-id="c9577-121">Nome</span><span class="sxs-lookup"><span data-stu-id="c9577-121">Name</span></span>|<span data-ttu-id="c9577-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9577-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c9577-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c9577-123">Authorization</span></span>|<span data-ttu-id="c9577-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c9577-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9577-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c9577-126">Request body</span></span>
<span data-ttu-id="c9577-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c9577-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9577-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9577-128">Response</span></span>
<span data-ttu-id="c9577-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c9577-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

### <a name="error-conditions-and-messages"></a><span data-ttu-id="c9577-131">Condições de erro e mensagens</span><span class="sxs-lookup"><span data-stu-id="c9577-131">Error conditions and messages</span></span>

|<span data-ttu-id="c9577-132">Cenário</span><span class="sxs-lookup"><span data-stu-id="c9577-132">Scenario</span></span>|<span data-ttu-id="c9577-133">Método</span><span class="sxs-lookup"><span data-stu-id="c9577-133">Method</span></span>|<span data-ttu-id="c9577-134">Código</span><span class="sxs-lookup"><span data-stu-id="c9577-134">Code</span></span>|<span data-ttu-id="c9577-135">Mensagem</span><span class="sxs-lookup"><span data-stu-id="c9577-135">Message</span></span>|
|--------|------|----|-------|
|<span data-ttu-id="c9577-136">O usuário tenta excluir um conector que tenha uma ou mais impressoras registradas</span><span class="sxs-lookup"><span data-stu-id="c9577-136">User attempts to delete a connector that has one or more printers registered</span></span>|<span data-ttu-id="c9577-137">DELETE</span><span class="sxs-lookup"><span data-stu-id="c9577-137">DELETE</span></span>|<span data-ttu-id="c9577-138">409</span><span class="sxs-lookup"><span data-stu-id="c9577-138">409</span></span>|<span data-ttu-id="c9577-139">Antes de excluir o conector, desassocie o registro das impressoras associadas.</span><span class="sxs-lookup"><span data-stu-id="c9577-139">Before deleting the connector, please unregister the associated printers.</span></span>|

## <a name="examples"></a><span data-ttu-id="c9577-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c9577-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c9577-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c9577-141">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_printconnector"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/print/connectors/{printConnectorId}
```


### <a name="response"></a><span data-ttu-id="c9577-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9577-142">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

