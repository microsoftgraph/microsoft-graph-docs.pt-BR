---
title: ação revokeDeviceLicense
description: Revogar licença de dispositivo VPP do iOS atribuída para determinado aplicativo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e064f84f994a34b8e5ddee34fd0adce4c205682f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35951537"
---
# <a name="revokedevicelicense-action"></a><span data-ttu-id="28c09-103">ação revokeDeviceLicense</span><span class="sxs-lookup"><span data-stu-id="28c09-103">revokeDeviceLicense action</span></span>

> <span data-ttu-id="28c09-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="28c09-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28c09-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="28c09-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28c09-106">Revogar licença de dispositivo VPP do iOS atribuída para determinado aplicativo.</span><span class="sxs-lookup"><span data-stu-id="28c09-106">Revoke assigned iOS VPP device license for given app.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28c09-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="28c09-107">Prerequisites</span></span>
<span data-ttu-id="28c09-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28c09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28c09-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="28c09-110">Permission type</span></span>|<span data-ttu-id="28c09-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="28c09-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28c09-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="28c09-112">Delegated (work or school account)</span></span>|<span data-ttu-id="28c09-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28c09-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="28c09-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="28c09-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28c09-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28c09-115">Not supported.</span></span>|
|<span data-ttu-id="28c09-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="28c09-116">Application</span></span>|<span data-ttu-id="28c09-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28c09-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="28c09-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="28c09-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/revokeDeviceLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/revokeDeviceLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/revokeDeviceLicense
```

## <a name="request-headers"></a><span data-ttu-id="28c09-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="28c09-119">Request headers</span></span>
|<span data-ttu-id="28c09-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="28c09-120">Header</span></span>|<span data-ttu-id="28c09-121">Valor</span><span class="sxs-lookup"><span data-stu-id="28c09-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28c09-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="28c09-122">Authorization</span></span>|<span data-ttu-id="28c09-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="28c09-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28c09-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="28c09-124">Accept</span></span>|<span data-ttu-id="28c09-125">application/json</span><span class="sxs-lookup"><span data-stu-id="28c09-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28c09-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="28c09-126">Request body</span></span>
<span data-ttu-id="28c09-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="28c09-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="28c09-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="28c09-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="28c09-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="28c09-129">Property</span></span>|<span data-ttu-id="28c09-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="28c09-130">Type</span></span>|<span data-ttu-id="28c09-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="28c09-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28c09-132">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="28c09-132">managedDeviceId</span></span>|<span data-ttu-id="28c09-133">String</span><span class="sxs-lookup"><span data-stu-id="28c09-133">String</span></span>|<span data-ttu-id="28c09-134">A DeviceID para a qual a licença de aplicativo atribuída deve ser revogada</span><span class="sxs-lookup"><span data-stu-id="28c09-134">DeviceId for whom assigned app license is to be revoked</span></span>|
|<span data-ttu-id="28c09-135">notifyManagedDevices</span><span class="sxs-lookup"><span data-stu-id="28c09-135">notifyManagedDevices</span></span>|<span data-ttu-id="28c09-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="28c09-136">Boolean</span></span>|<span data-ttu-id="28c09-137">Booliano que indica se a notificação de revogação deve ser enviada ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="28c09-137">Boolean that indicates if revoke notification should be sent to device</span></span>|



## <a name="response"></a><span data-ttu-id="28c09-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="28c09-138">Response</span></span>
<span data-ttu-id="28c09-139">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="28c09-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="28c09-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="28c09-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="28c09-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28c09-141">Request</span></span>
<span data-ttu-id="28c09-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="28c09-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/revokeDeviceLicense

Content-type: application/json
Content-length: 85

{
  "managedDeviceId": "Managed Device Id value",
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="28c09-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="28c09-143">Response</span></span>
<span data-ttu-id="28c09-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="28c09-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





