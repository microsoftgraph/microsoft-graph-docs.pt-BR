---
title: ação sendCustomNotificationToCompanyPortal
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fb5628331c11f4cad9543fe4c95989603655fb02
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49219213"
---
# <a name="sendcustomnotificationtocompanyportal-action"></a><span data-ttu-id="dac14-103">ação sendCustomNotificationToCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="dac14-103">sendCustomNotificationToCompanyPortal action</span></span>

<span data-ttu-id="dac14-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dac14-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dac14-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dac14-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dac14-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dac14-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dac14-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="dac14-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dac14-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dac14-108">Prerequisites</span></span>
<span data-ttu-id="dac14-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dac14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dac14-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dac14-111">Permission type</span></span>|<span data-ttu-id="dac14-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dac14-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dac14-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dac14-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dac14-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dac14-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="dac14-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dac14-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dac14-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dac14-116">Not supported.</span></span>|
|<span data-ttu-id="dac14-117">Application</span><span class="sxs-lookup"><span data-stu-id="dac14-117">Application</span></span>|<span data-ttu-id="dac14-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dac14-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dac14-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dac14-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/sendCustomNotificationToCompanyPortal
POST /deviceManagement/comanagedDevices/{managedDeviceId}/sendCustomNotificationToCompanyPortal
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/sendCustomNotificationToCompanyPortal
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/sendCustomNotificationToCompanyPortal
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/sendCustomNotificationToCompanyPortal
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/sendCustomNotificationToCompanyPortal
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/sendCustomNotificationToCompanyPortal
```

## <a name="request-headers"></a><span data-ttu-id="dac14-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dac14-120">Request headers</span></span>
|<span data-ttu-id="dac14-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dac14-121">Header</span></span>|<span data-ttu-id="dac14-122">Valor</span><span class="sxs-lookup"><span data-stu-id="dac14-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dac14-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="dac14-123">Authorization</span></span>|<span data-ttu-id="dac14-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dac14-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dac14-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dac14-125">Accept</span></span>|<span data-ttu-id="dac14-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dac14-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dac14-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dac14-127">Request body</span></span>
<span data-ttu-id="dac14-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="dac14-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="dac14-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="dac14-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="dac14-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dac14-130">Property</span></span>|<span data-ttu-id="dac14-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="dac14-131">Type</span></span>|<span data-ttu-id="dac14-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="dac14-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dac14-133">notificationTitle</span><span class="sxs-lookup"><span data-stu-id="dac14-133">notificationTitle</span></span>|<span data-ttu-id="dac14-134">String</span><span class="sxs-lookup"><span data-stu-id="dac14-134">String</span></span>|<span data-ttu-id="dac14-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="dac14-135">Not yet documented</span></span>|
|<span data-ttu-id="dac14-136">notificationBody</span><span class="sxs-lookup"><span data-stu-id="dac14-136">notificationBody</span></span>|<span data-ttu-id="dac14-137">String</span><span class="sxs-lookup"><span data-stu-id="dac14-137">String</span></span>|<span data-ttu-id="dac14-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="dac14-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="dac14-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="dac14-139">Response</span></span>
<span data-ttu-id="dac14-140">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="dac14-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="dac14-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dac14-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="dac14-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dac14-142">Request</span></span>
<span data-ttu-id="dac14-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dac14-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/sendCustomNotificationToCompanyPortal

Content-type: application/json
Content-length: 105

{
  "notificationTitle": "Notification Title value",
  "notificationBody": "Notification Body value"
}
```

### <a name="response"></a><span data-ttu-id="dac14-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="dac14-144">Response</span></span>
<span data-ttu-id="dac14-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dac14-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




