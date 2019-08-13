---
title: ação sendCustomNotificationToCompanyPortal
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 51b776f3ff2633d5b671377e7ef79b4e580fbaae
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350428"
---
# <a name="sendcustomnotificationtocompanyportal-action"></a><span data-ttu-id="b0043-103">ação sendCustomNotificationToCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="b0043-103">sendCustomNotificationToCompanyPortal action</span></span>

> <span data-ttu-id="b0043-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b0043-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0043-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b0043-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0043-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b0043-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b0043-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b0043-107">Prerequisites</span></span>
<span data-ttu-id="b0043-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0043-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0043-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b0043-110">Permission type</span></span>|<span data-ttu-id="b0043-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b0043-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0043-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b0043-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b0043-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0043-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b0043-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b0043-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0043-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0043-115">Not supported.</span></span>|
|<span data-ttu-id="b0043-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b0043-116">Application</span></span>|<span data-ttu-id="b0043-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0043-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0043-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b0043-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/sendCustomNotificationToCompanyPortal
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/sendCustomNotificationToCompanyPortal
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/sendCustomNotificationToCompanyPortal
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/sendCustomNotificationToCompanyPortal
```

## <a name="request-headers"></a><span data-ttu-id="b0043-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b0043-119">Request headers</span></span>
|<span data-ttu-id="b0043-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b0043-120">Header</span></span>|<span data-ttu-id="b0043-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b0043-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0043-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b0043-122">Authorization</span></span>|<span data-ttu-id="b0043-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b0043-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0043-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b0043-124">Accept</span></span>|<span data-ttu-id="b0043-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b0043-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0043-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b0043-126">Request body</span></span>
<span data-ttu-id="b0043-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="b0043-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b0043-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="b0043-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b0043-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0043-129">Property</span></span>|<span data-ttu-id="b0043-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0043-130">Type</span></span>|<span data-ttu-id="b0043-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0043-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0043-132">notificationTitle</span><span class="sxs-lookup"><span data-stu-id="b0043-132">notificationTitle</span></span>|<span data-ttu-id="b0043-133">String</span><span class="sxs-lookup"><span data-stu-id="b0043-133">String</span></span>|<span data-ttu-id="b0043-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b0043-134">Not yet documented</span></span>|
|<span data-ttu-id="b0043-135">notificationBody</span><span class="sxs-lookup"><span data-stu-id="b0043-135">notificationBody</span></span>|<span data-ttu-id="b0043-136">String</span><span class="sxs-lookup"><span data-stu-id="b0043-136">String</span></span>|<span data-ttu-id="b0043-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b0043-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b0043-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0043-138">Response</span></span>
<span data-ttu-id="b0043-139">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b0043-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b0043-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b0043-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="b0043-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b0043-141">Request</span></span>
<span data-ttu-id="b0043-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b0043-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/sendCustomNotificationToCompanyPortal

Content-type: application/json
Content-length: 105

{
  "notificationTitle": "Notification Title value",
  "notificationBody": "Notification Body value"
}
```

### <a name="response"></a><span data-ttu-id="b0043-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0043-143">Response</span></span>
<span data-ttu-id="b0043-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b0043-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






