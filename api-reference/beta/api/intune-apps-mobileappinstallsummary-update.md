---
title: Atualizar mobileAppInstallSummary
description: Atualiza as propriedades de um objeto mobileAppInstallSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 980f6b9c4712bea8fd4060f627603310ef8c6747
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30959660"
---
# <a name="update-mobileappinstallsummary"></a><span data-ttu-id="a50ac-103">Atualizar mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="a50ac-103">Update mobileAppInstallSummary</span></span>

> <span data-ttu-id="a50ac-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a50ac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a50ac-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a50ac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a50ac-106">Atualiza as propriedades de um objeto [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="a50ac-106">Update the properties of a [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a50ac-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a50ac-107">Prerequisites</span></span>
<span data-ttu-id="a50ac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a50ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a50ac-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a50ac-110">Permission type</span></span>|<span data-ttu-id="a50ac-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a50ac-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a50ac-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a50ac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a50ac-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a50ac-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a50ac-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a50ac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a50ac-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a50ac-115">Not supported.</span></span>|
|<span data-ttu-id="a50ac-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a50ac-116">Application</span></span>|<span data-ttu-id="a50ac-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a50ac-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a50ac-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a50ac-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="a50ac-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a50ac-119">Request headers</span></span>
|<span data-ttu-id="a50ac-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a50ac-120">Header</span></span>|<span data-ttu-id="a50ac-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a50ac-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a50ac-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a50ac-122">Authorization</span></span>|<span data-ttu-id="a50ac-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a50ac-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a50ac-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a50ac-124">Accept</span></span>|<span data-ttu-id="a50ac-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a50ac-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a50ac-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a50ac-126">Request body</span></span>
<span data-ttu-id="a50ac-127">No corpo da solicitação, forneça uma representação JSON do objeto [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="a50ac-127">In the request body, supply a JSON representation for the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>

<span data-ttu-id="a50ac-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="a50ac-128">The following table shows the properties that are required when you create the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md).</span></span>

|<span data-ttu-id="a50ac-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a50ac-129">Property</span></span>|<span data-ttu-id="a50ac-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a50ac-130">Type</span></span>|<span data-ttu-id="a50ac-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a50ac-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a50ac-132">id</span><span class="sxs-lookup"><span data-stu-id="a50ac-132">id</span></span>|<span data-ttu-id="a50ac-133">String</span><span class="sxs-lookup"><span data-stu-id="a50ac-133">String</span></span>|<span data-ttu-id="a50ac-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a50ac-134">Key of the entity.</span></span>|
|<span data-ttu-id="a50ac-135">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a50ac-135">installedDeviceCount</span></span>|<span data-ttu-id="a50ac-136">Int32</span><span class="sxs-lookup"><span data-stu-id="a50ac-136">Int32</span></span>|<span data-ttu-id="a50ac-137">Número de dispositivos que instalaram com êxito este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a50ac-137">Number of Devices that have successfully installed this app.</span></span>|
|<span data-ttu-id="a50ac-138">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a50ac-138">failedDeviceCount</span></span>|<span data-ttu-id="a50ac-139">Int32</span><span class="sxs-lookup"><span data-stu-id="a50ac-139">Int32</span></span>|<span data-ttu-id="a50ac-140">Número de dispositivos que falharam ao instalar este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a50ac-140">Number of Devices that have failed to install this app.</span></span>|
|<span data-ttu-id="a50ac-141">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a50ac-141">notApplicableDeviceCount</span></span>|<span data-ttu-id="a50ac-142">Int32</span><span class="sxs-lookup"><span data-stu-id="a50ac-142">Int32</span></span>|<span data-ttu-id="a50ac-143">Número de dispositivos que não se aplicam a este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a50ac-143">Number of Devices that are not applicable for this app.</span></span>|
|<span data-ttu-id="a50ac-144">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a50ac-144">notInstalledDeviceCount</span></span>|<span data-ttu-id="a50ac-145">Int32</span><span class="sxs-lookup"><span data-stu-id="a50ac-145">Int32</span></span>|<span data-ttu-id="a50ac-146">Número de dispositivos que não possuem este aplicativo instalado.</span><span class="sxs-lookup"><span data-stu-id="a50ac-146">Number of Devices that does not have this app installed.</span></span>|
|<span data-ttu-id="a50ac-147">pendingInstallDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a50ac-147">pendingInstallDeviceCount</span></span>|<span data-ttu-id="a50ac-148">Int32</span><span class="sxs-lookup"><span data-stu-id="a50ac-148">Int32</span></span>|<span data-ttu-id="a50ac-149">Número de dispositivos que foram notificados para instalar este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a50ac-149">Number of Devices that have been notified to install this app.</span></span>|
|<span data-ttu-id="a50ac-150">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="a50ac-150">installedUserCount</span></span>|<span data-ttu-id="a50ac-151">Int32</span><span class="sxs-lookup"><span data-stu-id="a50ac-151">Int32</span></span>|<span data-ttu-id="a50ac-152">Número de usuários cujos dispositivos foram todos bem-sucedidos para instalar este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a50ac-152">Number of Users whose devices have all succeeded to install this app.</span></span>|
|<span data-ttu-id="a50ac-153">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="a50ac-153">failedUserCount</span></span>|<span data-ttu-id="a50ac-154">Int32</span><span class="sxs-lookup"><span data-stu-id="a50ac-154">Int32</span></span>|<span data-ttu-id="a50ac-155">Número de usuários que têm um ou mais dispositivos que não instalaram este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a50ac-155">Number of Users that have 1 or more device that failed to install this app.</span></span>|
|<span data-ttu-id="a50ac-156">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="a50ac-156">notApplicableUserCount</span></span>|<span data-ttu-id="a50ac-157">Int32</span><span class="sxs-lookup"><span data-stu-id="a50ac-157">Int32</span></span>|<span data-ttu-id="a50ac-158">Número de usuários cujos dispositivos não são todos aplicáveis para este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a50ac-158">Number of Users whose devices were all not applicable for this app.</span></span>|
|<span data-ttu-id="a50ac-159">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="a50ac-159">notInstalledUserCount</span></span>|<span data-ttu-id="a50ac-160">Int32</span><span class="sxs-lookup"><span data-stu-id="a50ac-160">Int32</span></span>|<span data-ttu-id="a50ac-161">Número de usuários que têm um ou mais dispositivos que não instalaram este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a50ac-161">Number of Users that have 1 or more devices that did not install this app.</span></span>|
|<span data-ttu-id="a50ac-162">pendingInstallUserCount</span><span class="sxs-lookup"><span data-stu-id="a50ac-162">pendingInstallUserCount</span></span>|<span data-ttu-id="a50ac-163">Int32</span><span class="sxs-lookup"><span data-stu-id="a50ac-163">Int32</span></span>|<span data-ttu-id="a50ac-164">Número de usuários que têm um ou mais dispositivos que foram notificados para instalar este aplicativo e têm 0 dispositivos com falhas.</span><span class="sxs-lookup"><span data-stu-id="a50ac-164">Number of Users that have 1 or more device that have been notified to install this app and have 0 devices with failures.</span></span>|



## <a name="response"></a><span data-ttu-id="a50ac-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="a50ac-165">Response</span></span>
<span data-ttu-id="a50ac-166">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a50ac-166">If successful, this method returns a `200 OK` response code and an updated [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a50ac-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a50ac-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="a50ac-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a50ac-168">Request</span></span>
<span data-ttu-id="a50ac-169">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a50ac-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a50ac-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="a50ac-170">Response</span></span>
<span data-ttu-id="a50ac-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a50ac-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




