---
title: ação revokeDeviceLicense
description: Revogar licença de dispositivo VPP do iOS atribuída para determinado aplicativo.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e7436c6a98f5a3d2c2c73bc8ce1c5776b0545b94
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42761941"
---
# <a name="revokedevicelicense-action"></a><span data-ttu-id="937ba-103">ação revokeDeviceLicense</span><span class="sxs-lookup"><span data-stu-id="937ba-103">revokeDeviceLicense action</span></span>

> <span data-ttu-id="937ba-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="937ba-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="937ba-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="937ba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="937ba-106">Revogar licença de dispositivo VPP do iOS atribuída para determinado aplicativo.</span><span class="sxs-lookup"><span data-stu-id="937ba-106">Revoke assigned iOS VPP device license for given app.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="937ba-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="937ba-107">Prerequisites</span></span>
<span data-ttu-id="937ba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="937ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="937ba-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="937ba-110">Permission type</span></span>|<span data-ttu-id="937ba-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="937ba-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="937ba-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="937ba-112">Delegated (work or school account)</span></span>|<span data-ttu-id="937ba-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="937ba-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="937ba-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="937ba-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="937ba-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="937ba-115">Not supported.</span></span>|
|<span data-ttu-id="937ba-116">Application</span><span class="sxs-lookup"><span data-stu-id="937ba-116">Application</span></span>|<span data-ttu-id="937ba-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="937ba-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="937ba-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="937ba-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/revokeDeviceLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/revokeDeviceLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/revokeDeviceLicense
```

## <a name="request-headers"></a><span data-ttu-id="937ba-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="937ba-119">Request headers</span></span>
|<span data-ttu-id="937ba-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="937ba-120">Header</span></span>|<span data-ttu-id="937ba-121">Valor</span><span class="sxs-lookup"><span data-stu-id="937ba-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="937ba-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="937ba-122">Authorization</span></span>|<span data-ttu-id="937ba-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="937ba-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="937ba-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="937ba-124">Accept</span></span>|<span data-ttu-id="937ba-125">application/json</span><span class="sxs-lookup"><span data-stu-id="937ba-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="937ba-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="937ba-126">Request body</span></span>
<span data-ttu-id="937ba-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="937ba-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="937ba-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="937ba-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="937ba-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="937ba-129">Property</span></span>|<span data-ttu-id="937ba-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="937ba-130">Type</span></span>|<span data-ttu-id="937ba-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="937ba-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="937ba-132">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="937ba-132">managedDeviceId</span></span>|<span data-ttu-id="937ba-133">String</span><span class="sxs-lookup"><span data-stu-id="937ba-133">String</span></span>|<span data-ttu-id="937ba-134">A DeviceID para a qual a licença de aplicativo atribuída deve ser revogada</span><span class="sxs-lookup"><span data-stu-id="937ba-134">DeviceId for whom assigned app license is to be revoked</span></span>|
|<span data-ttu-id="937ba-135">notifyManagedDevices</span><span class="sxs-lookup"><span data-stu-id="937ba-135">notifyManagedDevices</span></span>|<span data-ttu-id="937ba-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="937ba-136">Boolean</span></span>|<span data-ttu-id="937ba-137">Booliano que indica se a notificação de revogação deve ser enviada ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="937ba-137">Boolean that indicates if revoke notification should be sent to device</span></span>|



## <a name="response"></a><span data-ttu-id="937ba-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="937ba-138">Response</span></span>
<span data-ttu-id="937ba-139">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="937ba-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="937ba-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="937ba-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="937ba-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="937ba-141">Request</span></span>
<span data-ttu-id="937ba-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="937ba-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/revokeDeviceLicense

Content-type: application/json
Content-length: 85

{
  "managedDeviceId": "Managed Device Id value",
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="937ba-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="937ba-143">Response</span></span>
<span data-ttu-id="937ba-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="937ba-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




