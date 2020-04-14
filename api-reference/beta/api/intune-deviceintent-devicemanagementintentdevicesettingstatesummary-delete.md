---
title: Excluir deviceManagementIntentDeviceSettingStateSummary
description: Exclui deviceManagementIntentDeviceSettingStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0bfa33ab7b6996b21ae0a717a1b1f7d02949e4b9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43326864"
---
# <a name="delete-devicemanagementintentdevicesettingstatesummary"></a><span data-ttu-id="d1570-103">Excluir deviceManagementIntentDeviceSettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="d1570-103">Delete deviceManagementIntentDeviceSettingStateSummary</span></span>

<span data-ttu-id="d1570-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1570-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d1570-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d1570-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1570-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d1570-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1570-107">Exclui [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="d1570-107">Deletes a [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d1570-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d1570-108">Prerequisites</span></span>
<span data-ttu-id="d1570-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1570-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1570-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d1570-111">Permission type</span></span>|<span data-ttu-id="d1570-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d1570-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1570-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d1570-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d1570-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1570-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d1570-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d1570-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1570-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1570-116">Not supported.</span></span>|
|<span data-ttu-id="d1570-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d1570-117">Application</span></span>|<span data-ttu-id="d1570-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1570-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1570-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d1570-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries/{deviceManagementIntentDeviceSettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="d1570-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d1570-120">Request headers</span></span>
|<span data-ttu-id="d1570-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d1570-121">Header</span></span>|<span data-ttu-id="d1570-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d1570-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1570-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d1570-123">Authorization</span></span>|<span data-ttu-id="d1570-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d1570-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1570-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d1570-125">Accept</span></span>|<span data-ttu-id="d1570-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d1570-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1570-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d1570-127">Request body</span></span>
<span data-ttu-id="d1570-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d1570-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1570-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1570-129">Response</span></span>
<span data-ttu-id="d1570-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d1570-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d1570-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d1570-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d1570-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d1570-132">Request</span></span>
<span data-ttu-id="d1570-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d1570-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries/{deviceManagementIntentDeviceSettingStateSummaryId}
```

### <a name="response"></a><span data-ttu-id="d1570-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1570-134">Response</span></span>
<span data-ttu-id="d1570-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d1570-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



