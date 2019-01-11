---
title: ação de revokeDeviceLicense
description: REVOKE atribuído iOS VPP dispositivo licença para fornecido app.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5a8dca4ea62e08e9d34727dd2142a156ba2d8dee
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864971"
---
# <a name="revokedevicelicense-action"></a><span data-ttu-id="feab1-103">ação de revokeDeviceLicense</span><span class="sxs-lookup"><span data-stu-id="feab1-103">revokeDeviceLicense action</span></span>

> <span data-ttu-id="feab1-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="feab1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="feab1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="feab1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="feab1-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="feab1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="feab1-107">REVOKE atribuído iOS VPP dispositivo licença para fornecido app.</span><span class="sxs-lookup"><span data-stu-id="feab1-107">Revoke assigned iOS VPP device license for given app.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="feab1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="feab1-108">Prerequisites</span></span>
<span data-ttu-id="feab1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="feab1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="feab1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="feab1-111">Permission type</span></span>|<span data-ttu-id="feab1-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="feab1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="feab1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="feab1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="feab1-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="feab1-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="feab1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="feab1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="feab1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="feab1-116">Not supported.</span></span>|
|<span data-ttu-id="feab1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="feab1-117">Application</span></span>|<span data-ttu-id="feab1-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="feab1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="feab1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="feab1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/revokeDeviceLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/revokeDeviceLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/revokeDeviceLicense
```

## <a name="request-headers"></a><span data-ttu-id="feab1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="feab1-120">Request headers</span></span>
|<span data-ttu-id="feab1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="feab1-121">Header</span></span>|<span data-ttu-id="feab1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="feab1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="feab1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="feab1-123">Authorization</span></span>|<span data-ttu-id="feab1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="feab1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="feab1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="feab1-125">Accept</span></span>|<span data-ttu-id="feab1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="feab1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="feab1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="feab1-127">Request body</span></span>
<span data-ttu-id="feab1-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="feab1-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="feab1-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="feab1-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="feab1-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="feab1-130">Property</span></span>|<span data-ttu-id="feab1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="feab1-131">Type</span></span>|<span data-ttu-id="feab1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="feab1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="feab1-133">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="feab1-133">managedDeviceId</span></span>|<span data-ttu-id="feab1-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="feab1-134">String</span></span>|<span data-ttu-id="feab1-135">DeviceId para quem a licença de aplicativo atribuídas é a ser revogado</span><span class="sxs-lookup"><span data-stu-id="feab1-135">DeviceId for whom assigned app license is to be revoked</span></span>|
|<span data-ttu-id="feab1-136">notifyManagedDevices</span><span class="sxs-lookup"><span data-stu-id="feab1-136">notifyManagedDevices</span></span>|<span data-ttu-id="feab1-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="feab1-137">Boolean</span></span>|<span data-ttu-id="feab1-138">Boolean que indica se revoke notificação deve ser enviada ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="feab1-138">Boolean that indicates if revoke notification should be sent to device</span></span>|



## <a name="response"></a><span data-ttu-id="feab1-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="feab1-139">Response</span></span>
<span data-ttu-id="feab1-140">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="feab1-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="feab1-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="feab1-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="feab1-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="feab1-142">Request</span></span>
<span data-ttu-id="feab1-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="feab1-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/revokeDeviceLicense

Content-type: application/json
Content-length: 85

{
  "managedDeviceId": "Managed Device Id value",
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="feab1-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="feab1-144">Response</span></span>
<span data-ttu-id="feab1-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="feab1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





