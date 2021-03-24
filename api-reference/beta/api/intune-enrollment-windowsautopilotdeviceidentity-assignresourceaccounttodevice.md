---
title: Ação assignResourceAccountToDevice
description: Atribui conta de recurso a dispositivos autopilot.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6d27c66a6d378a82af6ba81f63b90906fb91f7ca
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51142146"
---
# <a name="assignresourceaccounttodevice-action"></a><span data-ttu-id="5043d-103">Ação assignResourceAccountToDevice</span><span class="sxs-lookup"><span data-stu-id="5043d-103">assignResourceAccountToDevice action</span></span>

<span data-ttu-id="5043d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5043d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5043d-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5043d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5043d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5043d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5043d-107">Atribui conta de recurso a dispositivos autopilot.</span><span class="sxs-lookup"><span data-stu-id="5043d-107">Assigns resource account to Autopilot devices.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5043d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5043d-108">Prerequisites</span></span>
<span data-ttu-id="5043d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5043d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5043d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5043d-111">Permission type</span></span>|<span data-ttu-id="5043d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5043d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5043d-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5043d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5043d-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5043d-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5043d-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5043d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5043d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5043d-116">Not supported.</span></span>|
|<span data-ttu-id="5043d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5043d-117">Application</span></span>|<span data-ttu-id="5043d-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5043d-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5043d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5043d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignResourceAccountToDevice
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}/assignResourceAccountToDevice
```

## <a name="request-headers"></a><span data-ttu-id="5043d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5043d-120">Request headers</span></span>
|<span data-ttu-id="5043d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5043d-121">Header</span></span>|<span data-ttu-id="5043d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5043d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5043d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5043d-123">Authorization</span></span>|<span data-ttu-id="5043d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5043d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5043d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5043d-125">Accept</span></span>|<span data-ttu-id="5043d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5043d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5043d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5043d-127">Request body</span></span>
<span data-ttu-id="5043d-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="5043d-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="5043d-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="5043d-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="5043d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5043d-130">Property</span></span>|<span data-ttu-id="5043d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5043d-131">Type</span></span>|<span data-ttu-id="5043d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5043d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5043d-133">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5043d-133">userPrincipalName</span></span>|<span data-ttu-id="5043d-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5043d-134">String</span></span>|<span data-ttu-id="5043d-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5043d-135">Not yet documented</span></span>|
|<span data-ttu-id="5043d-136">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="5043d-136">addressableUserName</span></span>|<span data-ttu-id="5043d-137">String</span><span class="sxs-lookup"><span data-stu-id="5043d-137">String</span></span>|<span data-ttu-id="5043d-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5043d-138">Not yet documented</span></span>|
|<span data-ttu-id="5043d-139">resourceAccountName</span><span class="sxs-lookup"><span data-stu-id="5043d-139">resourceAccountName</span></span>|<span data-ttu-id="5043d-140">String</span><span class="sxs-lookup"><span data-stu-id="5043d-140">String</span></span>|<span data-ttu-id="5043d-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5043d-141">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="5043d-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="5043d-142">Response</span></span>
<span data-ttu-id="5043d-143">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5043d-143">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5043d-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5043d-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="5043d-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5043d-145">Request</span></span>
<span data-ttu-id="5043d-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5043d-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5043d-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="5043d-147">Response</span></span>
<span data-ttu-id="5043d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5043d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




