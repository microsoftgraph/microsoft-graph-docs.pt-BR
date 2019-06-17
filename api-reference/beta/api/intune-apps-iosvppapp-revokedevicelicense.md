---
title: ação revokeDeviceLicense
description: Revogar licença de dispositivo VPP do iOS atribuída para determinado aplicativo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5bc18f59a880eea7fe8e71f91cf018ae7925a066
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34965953"
---
# <a name="revokedevicelicense-action"></a><span data-ttu-id="658f0-103">ação revokeDeviceLicense</span><span class="sxs-lookup"><span data-stu-id="658f0-103">revokeDeviceLicense action</span></span>

> <span data-ttu-id="658f0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="658f0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="658f0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="658f0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="658f0-106">Revogar licença de dispositivo VPP do iOS atribuída para determinado aplicativo.</span><span class="sxs-lookup"><span data-stu-id="658f0-106">Revoke assigned iOS VPP device license for given app.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="658f0-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="658f0-107">Prerequisites</span></span>
<span data-ttu-id="658f0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="658f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="658f0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="658f0-110">Permission type</span></span>|<span data-ttu-id="658f0-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="658f0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="658f0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="658f0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="658f0-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="658f0-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="658f0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="658f0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="658f0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="658f0-115">Not supported.</span></span>|
|<span data-ttu-id="658f0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="658f0-116">Application</span></span>|<span data-ttu-id="658f0-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="658f0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="658f0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="658f0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/revokeDeviceLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/revokeDeviceLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/revokeDeviceLicense
```

## <a name="request-headers"></a><span data-ttu-id="658f0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="658f0-119">Request headers</span></span>
|<span data-ttu-id="658f0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="658f0-120">Header</span></span>|<span data-ttu-id="658f0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="658f0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="658f0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="658f0-122">Authorization</span></span>|<span data-ttu-id="658f0-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="658f0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="658f0-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="658f0-124">Accept</span></span>|<span data-ttu-id="658f0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="658f0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="658f0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="658f0-126">Request body</span></span>
<span data-ttu-id="658f0-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="658f0-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="658f0-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="658f0-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="658f0-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="658f0-129">Property</span></span>|<span data-ttu-id="658f0-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="658f0-130">Type</span></span>|<span data-ttu-id="658f0-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="658f0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="658f0-132">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="658f0-132">managedDeviceId</span></span>|<span data-ttu-id="658f0-133">String</span><span class="sxs-lookup"><span data-stu-id="658f0-133">String</span></span>|<span data-ttu-id="658f0-134">A DeviceID para a qual a licença de aplicativo atribuída deve ser revogada</span><span class="sxs-lookup"><span data-stu-id="658f0-134">DeviceId for whom assigned app license is to be revoked</span></span>|
|<span data-ttu-id="658f0-135">notifyManagedDevices</span><span class="sxs-lookup"><span data-stu-id="658f0-135">notifyManagedDevices</span></span>|<span data-ttu-id="658f0-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="658f0-136">Boolean</span></span>|<span data-ttu-id="658f0-137">Booliano que indica se a notificação de revogação deve ser enviada ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="658f0-137">Boolean that indicates if revoke notification should be sent to device</span></span>|



## <a name="response"></a><span data-ttu-id="658f0-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="658f0-138">Response</span></span>
<span data-ttu-id="658f0-139">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="658f0-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="658f0-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="658f0-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="658f0-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="658f0-141">Request</span></span>
<span data-ttu-id="658f0-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="658f0-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/revokeDeviceLicense

Content-type: application/json
Content-length: 85

{
  "managedDeviceId": "Managed Device Id value",
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="658f0-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="658f0-143">Response</span></span>
<span data-ttu-id="658f0-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="658f0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





