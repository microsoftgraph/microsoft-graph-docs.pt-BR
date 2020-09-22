---
title: Ação unassignResourceAccountFromDevice
description: Retira a atribuição da conta de recurso de um dispositivo de piloto automático.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 319408d8ebd962a1567ae53e4237676cf7444830
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48062593"
---
# <a name="unassignresourceaccountfromdevice-action"></a><span data-ttu-id="41261-103">Ação unassignResourceAccountFromDevice</span><span class="sxs-lookup"><span data-stu-id="41261-103">unassignResourceAccountFromDevice action</span></span>

<span data-ttu-id="41261-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41261-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="41261-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="41261-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="41261-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="41261-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41261-107">Retira a atribuição da conta de recurso de um dispositivo de piloto automático.</span><span class="sxs-lookup"><span data-stu-id="41261-107">Unassigns the resource account from an Autopilot device.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="41261-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="41261-108">Prerequisites</span></span>
<span data-ttu-id="41261-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41261-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41261-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="41261-111">Permission type</span></span>|<span data-ttu-id="41261-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="41261-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41261-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41261-113">Delegated (work or school account)</span></span>|<span data-ttu-id="41261-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41261-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="41261-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41261-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41261-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41261-116">Not supported.</span></span>|
|<span data-ttu-id="41261-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="41261-117">Application</span></span>|<span data-ttu-id="41261-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41261-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="41261-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="41261-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/unassignResourceAccountFromDevice
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}/unassignResourceAccountFromDevice
```

## <a name="request-headers"></a><span data-ttu-id="41261-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="41261-120">Request headers</span></span>
|<span data-ttu-id="41261-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="41261-121">Header</span></span>|<span data-ttu-id="41261-122">Valor</span><span class="sxs-lookup"><span data-stu-id="41261-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41261-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="41261-123">Authorization</span></span>|<span data-ttu-id="41261-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41261-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41261-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="41261-125">Accept</span></span>|<span data-ttu-id="41261-126">application/json</span><span class="sxs-lookup"><span data-stu-id="41261-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41261-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="41261-127">Request body</span></span>
<span data-ttu-id="41261-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="41261-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41261-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="41261-129">Response</span></span>
<span data-ttu-id="41261-130">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="41261-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="41261-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="41261-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="41261-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41261-132">Request</span></span>
<span data-ttu-id="41261-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="41261-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/unassignResourceAccountFromDevice
```

### <a name="response"></a><span data-ttu-id="41261-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="41261-134">Response</span></span>
<span data-ttu-id="41261-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="41261-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






