---
title: Excluir complianceManagementPartner
description: Exclui complianceManagementPartner.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5d2c9cdc6571339ca38bf4f575d658de1c9cf83c
ms.sourcegitcommit: 3c8a92d89ac60a48cb63449976b1c3c2c6302281
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/16/2020
ms.locfileid: "44744107"
---
# <a name="delete-compliancemanagementpartner"></a><span data-ttu-id="67b88-103">Excluir complianceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="67b88-103">Delete complianceManagementPartner</span></span>

<span data-ttu-id="67b88-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67b88-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="67b88-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="67b88-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67b88-106">Exclui [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="67b88-106">Deletes a [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="67b88-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="67b88-107">Prerequisites</span></span>
<span data-ttu-id="67b88-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="67b88-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="67b88-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67b88-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67b88-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="67b88-110">Permission type</span></span>|<span data-ttu-id="67b88-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="67b88-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67b88-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="67b88-112">Delegated (work or school account)</span></span>|<span data-ttu-id="67b88-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67b88-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="67b88-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="67b88-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67b88-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67b88-115">Not supported.</span></span>|
|<span data-ttu-id="67b88-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="67b88-116">Application</span></span>|<span data-ttu-id="67b88-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67b88-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="67b88-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="67b88-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="67b88-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="67b88-119">Request headers</span></span>
|<span data-ttu-id="67b88-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="67b88-120">Header</span></span>|<span data-ttu-id="67b88-121">Valor</span><span class="sxs-lookup"><span data-stu-id="67b88-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67b88-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="67b88-122">Authorization</span></span>|<span data-ttu-id="67b88-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="67b88-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67b88-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="67b88-124">Accept</span></span>|<span data-ttu-id="67b88-125">application/json</span><span class="sxs-lookup"><span data-stu-id="67b88-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67b88-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="67b88-126">Request body</span></span>
<span data-ttu-id="67b88-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="67b88-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="67b88-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="67b88-128">Response</span></span>
<span data-ttu-id="67b88-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="67b88-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="67b88-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="67b88-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="67b88-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67b88-131">Request</span></span>
<span data-ttu-id="67b88-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="67b88-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
```

### <a name="response"></a><span data-ttu-id="67b88-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="67b88-133">Response</span></span>
<span data-ttu-id="67b88-134">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="67b88-134">Here is an example of the response.</span></span> <span data-ttu-id="67b88-135">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="67b88-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="67b88-136">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="67b88-136">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



