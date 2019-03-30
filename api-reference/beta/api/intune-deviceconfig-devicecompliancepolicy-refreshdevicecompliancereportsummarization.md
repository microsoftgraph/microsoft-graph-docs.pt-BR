---
title: ação refreshDeviceComplianceReportSummarization
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 68a52635930a8bcb77d33b26c68ce53a855d51c4
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30985981"
---
# <a name="refreshdevicecompliancereportsummarization-action"></a><span data-ttu-id="dc278-103">ação refreshDeviceComplianceReportSummarization</span><span class="sxs-lookup"><span data-stu-id="dc278-103">refreshDeviceComplianceReportSummarization action</span></span>

> <span data-ttu-id="dc278-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dc278-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc278-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dc278-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc278-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="dc278-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dc278-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dc278-107">Prerequisites</span></span>
<span data-ttu-id="dc278-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc278-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc278-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dc278-110">Permission type</span></span>|<span data-ttu-id="dc278-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dc278-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc278-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dc278-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dc278-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="dc278-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="dc278-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dc278-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc278-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc278-115">Not supported.</span></span>|
|<span data-ttu-id="dc278-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dc278-116">Application</span></span>|<span data-ttu-id="dc278-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc278-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc278-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dc278-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/refreshDeviceComplianceReportSummarization
```

## <a name="request-headers"></a><span data-ttu-id="dc278-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dc278-119">Request headers</span></span>
|<span data-ttu-id="dc278-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dc278-120">Header</span></span>|<span data-ttu-id="dc278-121">Valor</span><span class="sxs-lookup"><span data-stu-id="dc278-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc278-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="dc278-122">Authorization</span></span>|<span data-ttu-id="dc278-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dc278-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc278-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dc278-124">Accept</span></span>|<span data-ttu-id="dc278-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dc278-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc278-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dc278-126">Request body</span></span>
<span data-ttu-id="dc278-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dc278-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc278-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc278-128">Response</span></span>
<span data-ttu-id="dc278-129">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="dc278-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="dc278-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dc278-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="dc278-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dc278-131">Request</span></span>
<span data-ttu-id="dc278-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dc278-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/refreshDeviceComplianceReportSummarization
```

### <a name="response"></a><span data-ttu-id="dc278-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc278-133">Response</span></span>
<span data-ttu-id="dc278-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dc278-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




