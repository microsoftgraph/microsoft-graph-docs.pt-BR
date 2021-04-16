---
title: ação refreshDeviceComplianceReportSummarization
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 71ce192e9b749b57a7409112314e82d6b0ad4ca4
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51863356"
---
# <a name="refreshdevicecompliancereportsummarization-action"></a><span data-ttu-id="a38b1-103">ação refreshDeviceComplianceReportSummarization</span><span class="sxs-lookup"><span data-stu-id="a38b1-103">refreshDeviceComplianceReportSummarization action</span></span>

<span data-ttu-id="a38b1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a38b1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a38b1-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a38b1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a38b1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a38b1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a38b1-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a38b1-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a38b1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a38b1-108">Prerequisites</span></span>
<span data-ttu-id="a38b1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a38b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a38b1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a38b1-111">Permission type</span></span>|<span data-ttu-id="a38b1-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a38b1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a38b1-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a38b1-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="a38b1-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="a38b1-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="a38b1-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a38b1-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a38b1-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a38b1-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a38b1-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a38b1-117">Not supported.</span></span>|
|<span data-ttu-id="a38b1-118">Application</span><span class="sxs-lookup"><span data-stu-id="a38b1-118">Application</span></span>||
| <span data-ttu-id="a38b1-119">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="a38b1-119">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="a38b1-120">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a38b1-120">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a38b1-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a38b1-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/refreshDeviceComplianceReportSummarization
```

## <a name="request-headers"></a><span data-ttu-id="a38b1-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a38b1-122">Request headers</span></span>
|<span data-ttu-id="a38b1-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a38b1-123">Header</span></span>|<span data-ttu-id="a38b1-124">Valor</span><span class="sxs-lookup"><span data-stu-id="a38b1-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a38b1-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="a38b1-125">Authorization</span></span>|<span data-ttu-id="a38b1-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a38b1-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a38b1-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a38b1-127">Accept</span></span>|<span data-ttu-id="a38b1-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a38b1-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a38b1-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a38b1-129">Request body</span></span>
<span data-ttu-id="a38b1-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a38b1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a38b1-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="a38b1-131">Response</span></span>
<span data-ttu-id="a38b1-132">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a38b1-132">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a38b1-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a38b1-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="a38b1-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a38b1-134">Request</span></span>
<span data-ttu-id="a38b1-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a38b1-135">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/refreshDeviceComplianceReportSummarization
```

### <a name="response"></a><span data-ttu-id="a38b1-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a38b1-136">Response</span></span>
<span data-ttu-id="a38b1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a38b1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







