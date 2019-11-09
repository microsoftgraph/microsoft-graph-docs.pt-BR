---
title: ação refreshDeviceComplianceReportSummarization
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f2e2b39afbfd80148a730995e654aed67f4fb136
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38086176"
---
# <a name="refreshdevicecompliancereportsummarization-action"></a><span data-ttu-id="ff574-103">ação refreshDeviceComplianceReportSummarization</span><span class="sxs-lookup"><span data-stu-id="ff574-103">refreshDeviceComplianceReportSummarization action</span></span>

> <span data-ttu-id="ff574-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ff574-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff574-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ff574-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff574-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ff574-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff574-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ff574-107">Prerequisites</span></span>
<span data-ttu-id="ff574-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff574-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff574-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ff574-110">Permission type</span></span>|<span data-ttu-id="ff574-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ff574-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff574-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ff574-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ff574-113">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="ff574-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="ff574-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ff574-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ff574-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ff574-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff574-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff574-116">Not supported.</span></span>|
|<span data-ttu-id="ff574-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ff574-117">Application</span></span>||
| <span data-ttu-id="ff574-118">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="ff574-118">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="ff574-119">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ff574-119">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff574-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ff574-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/refreshDeviceComplianceReportSummarization
```

## <a name="request-headers"></a><span data-ttu-id="ff574-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ff574-121">Request headers</span></span>
|<span data-ttu-id="ff574-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ff574-122">Header</span></span>|<span data-ttu-id="ff574-123">Valor</span><span class="sxs-lookup"><span data-stu-id="ff574-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff574-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ff574-124">Authorization</span></span>|<span data-ttu-id="ff574-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff574-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff574-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ff574-126">Accept</span></span>|<span data-ttu-id="ff574-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ff574-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff574-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ff574-128">Request body</span></span>
<span data-ttu-id="ff574-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ff574-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff574-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff574-130">Response</span></span>
<span data-ttu-id="ff574-131">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ff574-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ff574-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ff574-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff574-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff574-133">Request</span></span>
<span data-ttu-id="ff574-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ff574-134">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/refreshDeviceComplianceReportSummarization
```

### <a name="response"></a><span data-ttu-id="ff574-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff574-135">Response</span></span>
<span data-ttu-id="ff574-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ff574-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









