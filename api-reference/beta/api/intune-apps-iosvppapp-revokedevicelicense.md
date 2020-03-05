---
title: ação revokeDeviceLicense
description: Revogar licença de dispositivo VPP do iOS atribuída para determinado aplicativo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 66ff656304d7b67b5638d9d4844bf34b66eca2fd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42445579"
---
# <a name="revokedevicelicense-action"></a><span data-ttu-id="8cf8f-103">ação revokeDeviceLicense</span><span class="sxs-lookup"><span data-stu-id="8cf8f-103">revokeDeviceLicense action</span></span>

<span data-ttu-id="8cf8f-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8cf8f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8cf8f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8cf8f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8cf8f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8cf8f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8cf8f-107">Revogar licença de dispositivo VPP do iOS atribuída para determinado aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8cf8f-107">Revoke assigned iOS VPP device license for given app.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8cf8f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8cf8f-108">Prerequisites</span></span>
<span data-ttu-id="8cf8f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8cf8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cf8f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8cf8f-111">Permission type</span></span>|<span data-ttu-id="8cf8f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8cf8f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8cf8f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8cf8f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8cf8f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cf8f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8cf8f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8cf8f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8cf8f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8cf8f-116">Not supported.</span></span>|
|<span data-ttu-id="8cf8f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8cf8f-117">Application</span></span>|<span data-ttu-id="8cf8f-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cf8f-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8cf8f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8cf8f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/revokeDeviceLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/revokeDeviceLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/revokeDeviceLicense
```

## <a name="request-headers"></a><span data-ttu-id="8cf8f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8cf8f-120">Request headers</span></span>
|<span data-ttu-id="8cf8f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8cf8f-121">Header</span></span>|<span data-ttu-id="8cf8f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8cf8f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8cf8f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8cf8f-123">Authorization</span></span>|<span data-ttu-id="8cf8f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8cf8f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8cf8f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8cf8f-125">Accept</span></span>|<span data-ttu-id="8cf8f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8cf8f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8cf8f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8cf8f-127">Request body</span></span>
<span data-ttu-id="8cf8f-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="8cf8f-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="8cf8f-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="8cf8f-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="8cf8f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8cf8f-130">Property</span></span>|<span data-ttu-id="8cf8f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8cf8f-131">Type</span></span>|<span data-ttu-id="8cf8f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cf8f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cf8f-133">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="8cf8f-133">managedDeviceId</span></span>|<span data-ttu-id="8cf8f-134">String</span><span class="sxs-lookup"><span data-stu-id="8cf8f-134">String</span></span>|<span data-ttu-id="8cf8f-135">A DeviceID para a qual a licença de aplicativo atribuída deve ser revogada</span><span class="sxs-lookup"><span data-stu-id="8cf8f-135">DeviceId for whom assigned app license is to be revoked</span></span>|
|<span data-ttu-id="8cf8f-136">notifyManagedDevices</span><span class="sxs-lookup"><span data-stu-id="8cf8f-136">notifyManagedDevices</span></span>|<span data-ttu-id="8cf8f-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cf8f-137">Boolean</span></span>|<span data-ttu-id="8cf8f-138">Booliano que indica se a notificação de revogação deve ser enviada ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="8cf8f-138">Boolean that indicates if revoke notification should be sent to device</span></span>|



## <a name="response"></a><span data-ttu-id="8cf8f-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cf8f-139">Response</span></span>
<span data-ttu-id="8cf8f-140">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8cf8f-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8cf8f-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8cf8f-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="8cf8f-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8cf8f-142">Request</span></span>
<span data-ttu-id="8cf8f-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8cf8f-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/revokeDeviceLicense

Content-type: application/json
Content-length: 85

{
  "managedDeviceId": "Managed Device Id value",
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="8cf8f-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cf8f-144">Response</span></span>
<span data-ttu-id="8cf8f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8cf8f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





