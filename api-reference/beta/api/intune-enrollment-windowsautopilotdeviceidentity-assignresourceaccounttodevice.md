---
title: Ação assignResourceAccountToDevice
description: Atribui a conta de recurso aos dispositivos do AutoPilot.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b9b8c51e15785088d9f9d8e388168690f8f7fcc4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48011155"
---
# <a name="assignresourceaccounttodevice-action"></a><span data-ttu-id="f0bc4-103">Ação assignResourceAccountToDevice</span><span class="sxs-lookup"><span data-stu-id="f0bc4-103">assignResourceAccountToDevice action</span></span>

<span data-ttu-id="f0bc4-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f0bc4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f0bc4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f0bc4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0bc4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f0bc4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0bc4-107">Atribui a conta de recurso aos dispositivos do AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="f0bc4-107">Assigns resource account to Autopilot devices.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f0bc4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f0bc4-108">Prerequisites</span></span>
<span data-ttu-id="f0bc4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0bc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0bc4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f0bc4-111">Permission type</span></span>|<span data-ttu-id="f0bc4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f0bc4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0bc4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f0bc4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f0bc4-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0bc4-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f0bc4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f0bc4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0bc4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0bc4-116">Not supported.</span></span>|
|<span data-ttu-id="f0bc4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0bc4-117">Application</span></span>|<span data-ttu-id="f0bc4-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0bc4-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0bc4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f0bc4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignResourceAccountToDevice
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}/assignResourceAccountToDevice
```

## <a name="request-headers"></a><span data-ttu-id="f0bc4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f0bc4-120">Request headers</span></span>
|<span data-ttu-id="f0bc4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f0bc4-121">Header</span></span>|<span data-ttu-id="f0bc4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f0bc4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0bc4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f0bc4-123">Authorization</span></span>|<span data-ttu-id="f0bc4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f0bc4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0bc4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f0bc4-125">Accept</span></span>|<span data-ttu-id="f0bc4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f0bc4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0bc4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f0bc4-127">Request body</span></span>
<span data-ttu-id="f0bc4-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="f0bc4-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f0bc4-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="f0bc4-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f0bc4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f0bc4-130">Property</span></span>|<span data-ttu-id="f0bc4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0bc4-131">Type</span></span>|<span data-ttu-id="f0bc4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0bc4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0bc4-133">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f0bc4-133">userPrincipalName</span></span>|<span data-ttu-id="f0bc4-134">String</span><span class="sxs-lookup"><span data-stu-id="f0bc4-134">String</span></span>|<span data-ttu-id="f0bc4-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f0bc4-135">Not yet documented</span></span>|
|<span data-ttu-id="f0bc4-136">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="f0bc4-136">addressableUserName</span></span>|<span data-ttu-id="f0bc4-137">String</span><span class="sxs-lookup"><span data-stu-id="f0bc4-137">String</span></span>|<span data-ttu-id="f0bc4-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f0bc4-138">Not yet documented</span></span>|
|<span data-ttu-id="f0bc4-139">resourceAccountName</span><span class="sxs-lookup"><span data-stu-id="f0bc4-139">resourceAccountName</span></span>|<span data-ttu-id="f0bc4-140">String</span><span class="sxs-lookup"><span data-stu-id="f0bc4-140">String</span></span>|<span data-ttu-id="f0bc4-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f0bc4-141">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f0bc4-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0bc4-142">Response</span></span>
<span data-ttu-id="f0bc4-143">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f0bc4-143">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f0bc4-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f0bc4-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="f0bc4-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0bc4-145">Request</span></span>
<span data-ttu-id="f0bc4-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f0bc4-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignResourceAccountToDevice

Content-type: application/json
Content-length: 170

{
  "userPrincipalName": "User Principal Name value",
  "addressableUserName": "Addressable User Name value",
  "resourceAccountName": "Resource Account Name value"
}
```

### <a name="response"></a><span data-ttu-id="f0bc4-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0bc4-147">Response</span></span>
<span data-ttu-id="f0bc4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f0bc4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






