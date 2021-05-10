---
title: 'unifiedRoleEligibilityScheduleRequest: cancel'
description: Cancele um unifiedRoleEligibilityScheduleRequest.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 94e3fd5c5f42b5fc35a27724e77d47b07a7876ec
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299099"
---
# <a name="unifiedroleeligibilityschedulerequest-cancel"></a><span data-ttu-id="994ca-103">unifiedRoleEligibilityScheduleRequest: cancel</span><span class="sxs-lookup"><span data-stu-id="994ca-103">unifiedRoleEligibilityScheduleRequest: cancel</span></span>
<span data-ttu-id="994ca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="994ca-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="994ca-105">Cancele imediatamente [um unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) e o sistema exclua automaticamente a solicitação cancelada após 30 dias.</span><span class="sxs-lookup"><span data-stu-id="994ca-105">Immediately cancel a [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) and have the system automatically delete the cancelled request after 30 days.</span></span>

## <a name="permissions"></a><span data-ttu-id="994ca-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="994ca-106">Permissions</span></span>
<span data-ttu-id="994ca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="994ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="994ca-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="994ca-109">Permission type</span></span>|<span data-ttu-id="994ca-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="994ca-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="994ca-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="994ca-111">Delegated (work or school account)</span></span>|<span data-ttu-id="994ca-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="994ca-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="994ca-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="994ca-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="994ca-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="994ca-114">Not supported</span></span>|
|<span data-ttu-id="994ca-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="994ca-115">Application</span></span>|<span data-ttu-id="994ca-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="994ca-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="994ca-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="994ca-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /roleManagement/directory/roleEligibilityScheduleRequests/{unifiedRoleEligibilityScheduleRequestsId}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="994ca-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="994ca-118">Request headers</span></span>
|<span data-ttu-id="994ca-119">Nome</span><span class="sxs-lookup"><span data-stu-id="994ca-119">Name</span></span>|<span data-ttu-id="994ca-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="994ca-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="994ca-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="994ca-121">Authorization</span></span>|<span data-ttu-id="994ca-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="994ca-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="994ca-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="994ca-124">Request body</span></span>
<span data-ttu-id="994ca-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="994ca-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="994ca-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="994ca-126">Response</span></span>

<span data-ttu-id="994ca-127">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="994ca-127">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="994ca-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="994ca-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="994ca-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="994ca-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "unifiedroleeligibilityschedulerequest_cancel"
}
-->
``` http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilityScheduleRequests/{unifiedRoleEligibilityScheduleRequestsId}/cancel
```


### <a name="response"></a><span data-ttu-id="994ca-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="994ca-130">Response</span></span>
<span data-ttu-id="994ca-131">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="994ca-131">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

