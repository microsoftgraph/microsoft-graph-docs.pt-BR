---
title: ação updateDeviceProperties
description: Atualiza as propriedades nos dispositivos do AutoPilot.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 09598a47f945878ccd815f497e30df207db79040
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49212367"
---
# <a name="updatedeviceproperties-action"></a><span data-ttu-id="f4a48-103">ação updateDeviceProperties</span><span class="sxs-lookup"><span data-stu-id="f4a48-103">updateDeviceProperties action</span></span>

<span data-ttu-id="f4a48-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4a48-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f4a48-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f4a48-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4a48-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f4a48-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4a48-107">Atualiza as propriedades nos dispositivos do AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="f4a48-107">Updates properties on Autopilot devices.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4a48-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f4a48-108">Prerequisites</span></span>
<span data-ttu-id="f4a48-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4a48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4a48-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f4a48-111">Permission type</span></span>|<span data-ttu-id="f4a48-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f4a48-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4a48-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f4a48-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f4a48-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4a48-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f4a48-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f4a48-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4a48-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f4a48-116">Not supported.</span></span>|
|<span data-ttu-id="f4a48-117">Application</span><span class="sxs-lookup"><span data-stu-id="f4a48-117">Application</span></span>|<span data-ttu-id="f4a48-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4a48-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4a48-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f4a48-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/updateDeviceProperties
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}/updateDeviceProperties
```

## <a name="request-headers"></a><span data-ttu-id="f4a48-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f4a48-120">Request headers</span></span>
|<span data-ttu-id="f4a48-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f4a48-121">Header</span></span>|<span data-ttu-id="f4a48-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f4a48-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4a48-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f4a48-123">Authorization</span></span>|<span data-ttu-id="f4a48-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f4a48-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4a48-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f4a48-125">Accept</span></span>|<span data-ttu-id="f4a48-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f4a48-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4a48-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f4a48-127">Request body</span></span>
<span data-ttu-id="f4a48-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="f4a48-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f4a48-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="f4a48-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f4a48-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f4a48-130">Property</span></span>|<span data-ttu-id="f4a48-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4a48-131">Type</span></span>|<span data-ttu-id="f4a48-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4a48-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4a48-133">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f4a48-133">userPrincipalName</span></span>|<span data-ttu-id="f4a48-134">String</span><span class="sxs-lookup"><span data-stu-id="f4a48-134">String</span></span>|<span data-ttu-id="f4a48-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f4a48-135">Not yet documented</span></span>|
|<span data-ttu-id="f4a48-136">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="f4a48-136">addressableUserName</span></span>|<span data-ttu-id="f4a48-137">String</span><span class="sxs-lookup"><span data-stu-id="f4a48-137">String</span></span>|<span data-ttu-id="f4a48-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f4a48-138">Not yet documented</span></span>|
|<span data-ttu-id="f4a48-139">groupTag</span><span class="sxs-lookup"><span data-stu-id="f4a48-139">groupTag</span></span>|<span data-ttu-id="f4a48-140">String</span><span class="sxs-lookup"><span data-stu-id="f4a48-140">String</span></span>|<span data-ttu-id="f4a48-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f4a48-141">Not yet documented</span></span>|
|<span data-ttu-id="f4a48-142">displayName</span><span class="sxs-lookup"><span data-stu-id="f4a48-142">displayName</span></span>|<span data-ttu-id="f4a48-143">String</span><span class="sxs-lookup"><span data-stu-id="f4a48-143">String</span></span>|<span data-ttu-id="f4a48-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f4a48-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f4a48-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4a48-145">Response</span></span>
<span data-ttu-id="f4a48-146">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f4a48-146">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f4a48-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f4a48-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4a48-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f4a48-148">Request</span></span>
<span data-ttu-id="f4a48-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f4a48-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/updateDeviceProperties

Content-type: application/json
Content-length: 187

{
  "userPrincipalName": "User Principal Name value",
  "addressableUserName": "Addressable User Name value",
  "groupTag": "Group Tag value",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="f4a48-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4a48-150">Response</span></span>
<span data-ttu-id="f4a48-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f4a48-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




