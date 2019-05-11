---
title: Excluir deviceManagementIntentDeviceSettingStateSummary
description: Exclui deviceManagementIntentDeviceSettingStateSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 74720c39ac2dc2715bf84d00b7f14871df5c4feb
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33916109"
---
# <a name="delete-devicemanagementintentdevicesettingstatesummary"></a><span data-ttu-id="04285-103">Excluir deviceManagementIntentDeviceSettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="04285-103">Delete deviceManagementIntentDeviceSettingStateSummary</span></span>

> <span data-ttu-id="04285-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="04285-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04285-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="04285-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04285-106">Exclui [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="04285-106">Deletes a [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04285-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="04285-107">Prerequisites</span></span>
<span data-ttu-id="04285-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04285-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04285-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="04285-110">Permission type</span></span>|<span data-ttu-id="04285-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="04285-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04285-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="04285-112">Delegated (work or school account)</span></span>|<span data-ttu-id="04285-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04285-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="04285-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="04285-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04285-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="04285-115">Not supported.</span></span>|
|<span data-ttu-id="04285-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="04285-116">Application</span></span>|<span data-ttu-id="04285-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="04285-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04285-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="04285-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries/{deviceManagementIntentDeviceSettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="04285-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="04285-119">Request headers</span></span>
|<span data-ttu-id="04285-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="04285-120">Header</span></span>|<span data-ttu-id="04285-121">Valor</span><span class="sxs-lookup"><span data-stu-id="04285-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04285-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="04285-122">Authorization</span></span>|<span data-ttu-id="04285-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04285-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04285-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="04285-124">Accept</span></span>|<span data-ttu-id="04285-125">application/json</span><span class="sxs-lookup"><span data-stu-id="04285-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04285-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="04285-126">Request body</span></span>
<span data-ttu-id="04285-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="04285-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04285-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="04285-128">Response</span></span>
<span data-ttu-id="04285-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="04285-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="04285-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="04285-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="04285-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="04285-131">Request</span></span>
<span data-ttu-id="04285-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="04285-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries/{deviceManagementIntentDeviceSettingStateSummaryId}
```

### <a name="response"></a><span data-ttu-id="04285-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="04285-133">Response</span></span>
<span data-ttu-id="04285-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="04285-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




