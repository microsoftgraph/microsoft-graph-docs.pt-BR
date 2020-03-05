---
title: Atualizar mobileAppInstallSummary
description: Atualiza as propriedades de um objeto mobileAppInstallSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 55e9c0388990bd333931e6f07bed16913b7b1ee9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42450682"
---
# <a name="update-mobileappinstallsummary"></a><span data-ttu-id="f457e-103">Atualizar mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="f457e-103">Update mobileAppInstallSummary</span></span>

<span data-ttu-id="f457e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f457e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f457e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f457e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f457e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f457e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f457e-107">Atualiza as propriedades de um objeto [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="f457e-107">Update the properties of a [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f457e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f457e-108">Prerequisites</span></span>
<span data-ttu-id="f457e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f457e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f457e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f457e-111">Permission type</span></span>|<span data-ttu-id="f457e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f457e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f457e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f457e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f457e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f457e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f457e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f457e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f457e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f457e-116">Not supported.</span></span>|
|<span data-ttu-id="f457e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f457e-117">Application</span></span>|<span data-ttu-id="f457e-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f457e-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f457e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f457e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="f457e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f457e-120">Request headers</span></span>
|<span data-ttu-id="f457e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f457e-121">Header</span></span>|<span data-ttu-id="f457e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f457e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f457e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f457e-123">Authorization</span></span>|<span data-ttu-id="f457e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f457e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f457e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f457e-125">Accept</span></span>|<span data-ttu-id="f457e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f457e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f457e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f457e-127">Request body</span></span>
<span data-ttu-id="f457e-128">No corpo da solicitação, forneça uma representação JSON do objeto [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="f457e-128">In the request body, supply a JSON representation for the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>

<span data-ttu-id="f457e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="f457e-129">The following table shows the properties that are required when you create the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md).</span></span>

|<span data-ttu-id="f457e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f457e-130">Property</span></span>|<span data-ttu-id="f457e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f457e-131">Type</span></span>|<span data-ttu-id="f457e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f457e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f457e-133">id</span><span class="sxs-lookup"><span data-stu-id="f457e-133">id</span></span>|<span data-ttu-id="f457e-134">String</span><span class="sxs-lookup"><span data-stu-id="f457e-134">String</span></span>|<span data-ttu-id="f457e-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f457e-135">Key of the entity.</span></span>|
|<span data-ttu-id="f457e-136">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f457e-136">installedDeviceCount</span></span>|<span data-ttu-id="f457e-137">Int32</span><span class="sxs-lookup"><span data-stu-id="f457e-137">Int32</span></span>|<span data-ttu-id="f457e-138">Número de dispositivos que instalaram com êxito este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f457e-138">Number of Devices that have successfully installed this app.</span></span>|
|<span data-ttu-id="f457e-139">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f457e-139">failedDeviceCount</span></span>|<span data-ttu-id="f457e-140">Int32</span><span class="sxs-lookup"><span data-stu-id="f457e-140">Int32</span></span>|<span data-ttu-id="f457e-141">Número de dispositivos que falharam ao instalar este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f457e-141">Number of Devices that have failed to install this app.</span></span>|
|<span data-ttu-id="f457e-142">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f457e-142">notApplicableDeviceCount</span></span>|<span data-ttu-id="f457e-143">Int32</span><span class="sxs-lookup"><span data-stu-id="f457e-143">Int32</span></span>|<span data-ttu-id="f457e-144">Número de dispositivos que não se aplicam a este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f457e-144">Number of Devices that are not applicable for this app.</span></span>|
|<span data-ttu-id="f457e-145">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f457e-145">notInstalledDeviceCount</span></span>|<span data-ttu-id="f457e-146">Int32</span><span class="sxs-lookup"><span data-stu-id="f457e-146">Int32</span></span>|<span data-ttu-id="f457e-147">Número de dispositivos que não possuem este aplicativo instalado.</span><span class="sxs-lookup"><span data-stu-id="f457e-147">Number of Devices that does not have this app installed.</span></span>|
|<span data-ttu-id="f457e-148">pendingInstallDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f457e-148">pendingInstallDeviceCount</span></span>|<span data-ttu-id="f457e-149">Int32</span><span class="sxs-lookup"><span data-stu-id="f457e-149">Int32</span></span>|<span data-ttu-id="f457e-150">Número de dispositivos que foram notificados para instalar este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f457e-150">Number of Devices that have been notified to install this app.</span></span>|
|<span data-ttu-id="f457e-151">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="f457e-151">installedUserCount</span></span>|<span data-ttu-id="f457e-152">Int32</span><span class="sxs-lookup"><span data-stu-id="f457e-152">Int32</span></span>|<span data-ttu-id="f457e-153">Número de usuários cujos dispositivos foram todos bem-sucedidos para instalar este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f457e-153">Number of Users whose devices have all succeeded to install this app.</span></span>|
|<span data-ttu-id="f457e-154">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="f457e-154">failedUserCount</span></span>|<span data-ttu-id="f457e-155">Int32</span><span class="sxs-lookup"><span data-stu-id="f457e-155">Int32</span></span>|<span data-ttu-id="f457e-156">Número de usuários que têm um ou mais dispositivos que não instalaram este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f457e-156">Number of Users that have 1 or more device that failed to install this app.</span></span>|
|<span data-ttu-id="f457e-157">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="f457e-157">notApplicableUserCount</span></span>|<span data-ttu-id="f457e-158">Int32</span><span class="sxs-lookup"><span data-stu-id="f457e-158">Int32</span></span>|<span data-ttu-id="f457e-159">Número de usuários cujos dispositivos não são todos aplicáveis para este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f457e-159">Number of Users whose devices were all not applicable for this app.</span></span>|
|<span data-ttu-id="f457e-160">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="f457e-160">notInstalledUserCount</span></span>|<span data-ttu-id="f457e-161">Int32</span><span class="sxs-lookup"><span data-stu-id="f457e-161">Int32</span></span>|<span data-ttu-id="f457e-162">Número de usuários que têm um ou mais dispositivos que não instalaram este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f457e-162">Number of Users that have 1 or more devices that did not install this app.</span></span>|
|<span data-ttu-id="f457e-163">pendingInstallUserCount</span><span class="sxs-lookup"><span data-stu-id="f457e-163">pendingInstallUserCount</span></span>|<span data-ttu-id="f457e-164">Int32</span><span class="sxs-lookup"><span data-stu-id="f457e-164">Int32</span></span>|<span data-ttu-id="f457e-165">Número de usuários que têm um ou mais dispositivos que foram notificados para instalar este aplicativo e têm 0 dispositivos com falhas.</span><span class="sxs-lookup"><span data-stu-id="f457e-165">Number of Users that have 1 or more device that have been notified to install this app and have 0 devices with failures.</span></span>|



## <a name="response"></a><span data-ttu-id="f457e-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="f457e-166">Response</span></span>
<span data-ttu-id="f457e-167">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f457e-167">If successful, this method returns a `200 OK` response code and an updated [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f457e-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f457e-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="f457e-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f457e-169">Request</span></span>
<span data-ttu-id="f457e-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f457e-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/installSummary
Content-type: application/json
Content-length: 374

{
  "@odata.type": "#microsoft.graph.mobileAppInstallSummary",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notApplicableDeviceCount": 8,
  "notInstalledDeviceCount": 7,
  "pendingInstallDeviceCount": 9,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notApplicableUserCount": 6,
  "notInstalledUserCount": 5,
  "pendingInstallUserCount": 7
}
```

### <a name="response"></a><span data-ttu-id="f457e-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="f457e-171">Response</span></span>
<span data-ttu-id="f457e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f457e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 423

{
  "@odata.type": "#microsoft.graph.mobileAppInstallSummary",
  "id": "06a792e9-92e9-06a7-e992-a706e992a706",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notApplicableDeviceCount": 8,
  "notInstalledDeviceCount": 7,
  "pendingInstallDeviceCount": 9,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notApplicableUserCount": 6,
  "notInstalledUserCount": 5,
  "pendingInstallUserCount": 7
}
```





