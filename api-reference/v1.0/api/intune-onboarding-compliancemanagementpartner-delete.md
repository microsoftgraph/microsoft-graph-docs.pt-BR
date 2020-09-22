---
title: Excluir complianceManagementPartner
description: Exclui complianceManagementPartner.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 17819fc253907b54ecddbda8f2d4324891b90e63
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015712"
---
# <a name="delete-compliancemanagementpartner"></a><span data-ttu-id="38873-103">Excluir complianceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="38873-103">Delete complianceManagementPartner</span></span>

<span data-ttu-id="38873-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38873-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="38873-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="38873-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38873-106">Exclui [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="38873-106">Deletes a [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="38873-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="38873-107">Prerequisites</span></span>
<span data-ttu-id="38873-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38873-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38873-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="38873-110">Permission type</span></span>|<span data-ttu-id="38873-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="38873-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38873-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="38873-112">Delegated (work or school account)</span></span>|<span data-ttu-id="38873-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38873-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="38873-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="38873-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38873-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38873-115">Not supported.</span></span>|
|<span data-ttu-id="38873-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="38873-116">Application</span></span>|<span data-ttu-id="38873-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38873-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="38873-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="38873-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="38873-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="38873-119">Request headers</span></span>
|<span data-ttu-id="38873-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="38873-120">Header</span></span>|<span data-ttu-id="38873-121">Valor</span><span class="sxs-lookup"><span data-stu-id="38873-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38873-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="38873-122">Authorization</span></span>|<span data-ttu-id="38873-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38873-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38873-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="38873-124">Accept</span></span>|<span data-ttu-id="38873-125">application/json</span><span class="sxs-lookup"><span data-stu-id="38873-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38873-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="38873-126">Request body</span></span>
<span data-ttu-id="38873-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="38873-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38873-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="38873-128">Response</span></span>
<span data-ttu-id="38873-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="38873-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="38873-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="38873-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="38873-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38873-131">Request</span></span>
<span data-ttu-id="38873-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="38873-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
```

### <a name="response"></a><span data-ttu-id="38873-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="38873-133">Response</span></span>
<span data-ttu-id="38873-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="38873-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






