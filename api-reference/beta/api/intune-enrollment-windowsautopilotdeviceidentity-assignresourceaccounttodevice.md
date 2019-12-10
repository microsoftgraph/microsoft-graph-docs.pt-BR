---
title: Ação assignResourceAccountToDevice
description: Atribui a conta de recurso aos dispositivos do AutoPilot.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4cdf4a176e18b6f68328e6eba286e3298e2a9be1
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39943716"
---
# <a name="assignresourceaccounttodevice-action"></a><span data-ttu-id="0ff8e-103">Ação assignResourceAccountToDevice</span><span class="sxs-lookup"><span data-stu-id="0ff8e-103">assignResourceAccountToDevice action</span></span>

> <span data-ttu-id="0ff8e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0ff8e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ff8e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0ff8e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ff8e-106">Atribui a conta de recurso aos dispositivos do AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="0ff8e-106">Assigns resource account to Autopilot devices.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0ff8e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0ff8e-107">Prerequisites</span></span>
<span data-ttu-id="0ff8e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ff8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ff8e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0ff8e-110">Permission type</span></span>|<span data-ttu-id="0ff8e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0ff8e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ff8e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0ff8e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0ff8e-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ff8e-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0ff8e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0ff8e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ff8e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ff8e-115">Not supported.</span></span>|
|<span data-ttu-id="0ff8e-116">Application</span><span class="sxs-lookup"><span data-stu-id="0ff8e-116">Application</span></span>|<span data-ttu-id="0ff8e-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ff8e-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ff8e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0ff8e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignResourceAccountToDevice
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}/assignResourceAccountToDevice
```

## <a name="request-headers"></a><span data-ttu-id="0ff8e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0ff8e-119">Request headers</span></span>
|<span data-ttu-id="0ff8e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0ff8e-120">Header</span></span>|<span data-ttu-id="0ff8e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0ff8e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ff8e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0ff8e-122">Authorization</span></span>|<span data-ttu-id="0ff8e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0ff8e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ff8e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0ff8e-124">Accept</span></span>|<span data-ttu-id="0ff8e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0ff8e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ff8e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0ff8e-126">Request body</span></span>
<span data-ttu-id="0ff8e-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="0ff8e-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="0ff8e-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="0ff8e-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="0ff8e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0ff8e-129">Property</span></span>|<span data-ttu-id="0ff8e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ff8e-130">Type</span></span>|<span data-ttu-id="0ff8e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ff8e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ff8e-132">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0ff8e-132">userPrincipalName</span></span>|<span data-ttu-id="0ff8e-133">String</span><span class="sxs-lookup"><span data-stu-id="0ff8e-133">String</span></span>|<span data-ttu-id="0ff8e-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0ff8e-134">Not yet documented</span></span>|
|<span data-ttu-id="0ff8e-135">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="0ff8e-135">addressableUserName</span></span>|<span data-ttu-id="0ff8e-136">String</span><span class="sxs-lookup"><span data-stu-id="0ff8e-136">String</span></span>|<span data-ttu-id="0ff8e-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0ff8e-137">Not yet documented</span></span>|
|<span data-ttu-id="0ff8e-138">resourceAccountName</span><span class="sxs-lookup"><span data-stu-id="0ff8e-138">resourceAccountName</span></span>|<span data-ttu-id="0ff8e-139">String</span><span class="sxs-lookup"><span data-stu-id="0ff8e-139">String</span></span>|<span data-ttu-id="0ff8e-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0ff8e-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0ff8e-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ff8e-141">Response</span></span>
<span data-ttu-id="0ff8e-142">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0ff8e-142">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0ff8e-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0ff8e-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ff8e-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0ff8e-144">Request</span></span>
<span data-ttu-id="0ff8e-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0ff8e-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0ff8e-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ff8e-146">Response</span></span>
<span data-ttu-id="0ff8e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0ff8e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





