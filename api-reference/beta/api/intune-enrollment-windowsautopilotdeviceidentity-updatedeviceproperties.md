---
title: ação updateDeviceProperties
description: Atualiza as propriedades nos dispositivos do AutoPilot.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 29451664b2c6f9ba3bab146515c4a3e24fb99ac3
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804979"
---
# <a name="updatedeviceproperties-action"></a><span data-ttu-id="c217d-103">ação updateDeviceProperties</span><span class="sxs-lookup"><span data-stu-id="c217d-103">updateDeviceProperties action</span></span>

> <span data-ttu-id="c217d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c217d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c217d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c217d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c217d-106">Atualiza as propriedades nos dispositivos do AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="c217d-106">Updates properties on Autopilot devices.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c217d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c217d-107">Prerequisites</span></span>
<span data-ttu-id="c217d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c217d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c217d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c217d-110">Permission type</span></span>|<span data-ttu-id="c217d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c217d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c217d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c217d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c217d-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c217d-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c217d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c217d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c217d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c217d-115">Not supported.</span></span>|
|<span data-ttu-id="c217d-116">Application</span><span class="sxs-lookup"><span data-stu-id="c217d-116">Application</span></span>|<span data-ttu-id="c217d-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c217d-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c217d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c217d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/updateDeviceProperties
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}/updateDeviceProperties
```

## <a name="request-headers"></a><span data-ttu-id="c217d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c217d-119">Request headers</span></span>
|<span data-ttu-id="c217d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c217d-120">Header</span></span>|<span data-ttu-id="c217d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c217d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c217d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c217d-122">Authorization</span></span>|<span data-ttu-id="c217d-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c217d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c217d-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c217d-124">Accept</span></span>|<span data-ttu-id="c217d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c217d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c217d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c217d-126">Request body</span></span>
<span data-ttu-id="c217d-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="c217d-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c217d-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="c217d-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c217d-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c217d-129">Property</span></span>|<span data-ttu-id="c217d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c217d-130">Type</span></span>|<span data-ttu-id="c217d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c217d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c217d-132">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c217d-132">userPrincipalName</span></span>|<span data-ttu-id="c217d-133">String</span><span class="sxs-lookup"><span data-stu-id="c217d-133">String</span></span>|<span data-ttu-id="c217d-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c217d-134">Not yet documented</span></span>|
|<span data-ttu-id="c217d-135">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="c217d-135">addressableUserName</span></span>|<span data-ttu-id="c217d-136">String</span><span class="sxs-lookup"><span data-stu-id="c217d-136">String</span></span>|<span data-ttu-id="c217d-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c217d-137">Not yet documented</span></span>|
|<span data-ttu-id="c217d-138">groupTag</span><span class="sxs-lookup"><span data-stu-id="c217d-138">groupTag</span></span>|<span data-ttu-id="c217d-139">String</span><span class="sxs-lookup"><span data-stu-id="c217d-139">String</span></span>|<span data-ttu-id="c217d-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c217d-140">Not yet documented</span></span>|
|<span data-ttu-id="c217d-141">displayName</span><span class="sxs-lookup"><span data-stu-id="c217d-141">displayName</span></span>|<span data-ttu-id="c217d-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c217d-142">String</span></span>|<span data-ttu-id="c217d-143">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c217d-143">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c217d-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="c217d-144">Response</span></span>
<span data-ttu-id="c217d-145">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c217d-145">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c217d-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c217d-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="c217d-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c217d-147">Request</span></span>
<span data-ttu-id="c217d-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c217d-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c217d-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="c217d-149">Response</span></span>
<span data-ttu-id="c217d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c217d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




