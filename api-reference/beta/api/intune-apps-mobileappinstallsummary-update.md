---
title: Atualizar mobileAppInstallSummary
description: Atualize as propriedades de um objeto mobileAppInstallSummary.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 19bd1e61359c5d2bdaff6ee87e807bae7dba0f05
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864796"
---
# <a name="update-mobileappinstallsummary"></a><span data-ttu-id="9b19b-103">Atualizar mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="9b19b-103">Update mobileAppInstallSummary</span></span>

> <span data-ttu-id="9b19b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9b19b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9b19b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9b19b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9b19b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9b19b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9b19b-107">Atualize as propriedades de um objeto [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="9b19b-107">Update the properties of a [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9b19b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9b19b-108">Prerequisites</span></span>
<span data-ttu-id="9b19b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b19b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b19b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9b19b-111">Permission type</span></span>|<span data-ttu-id="9b19b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9b19b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b19b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9b19b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9b19b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b19b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9b19b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9b19b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b19b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b19b-116">Not supported.</span></span>|
|<span data-ttu-id="9b19b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9b19b-117">Application</span></span>|<span data-ttu-id="9b19b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b19b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b19b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9b19b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="9b19b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9b19b-120">Request headers</span></span>
|<span data-ttu-id="9b19b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9b19b-121">Header</span></span>|<span data-ttu-id="9b19b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9b19b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b19b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9b19b-123">Authorization</span></span>|<span data-ttu-id="9b19b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9b19b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b19b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9b19b-125">Accept</span></span>|<span data-ttu-id="9b19b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9b19b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b19b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9b19b-127">Request body</span></span>
<span data-ttu-id="9b19b-128">No corpo da solicitação, fornece uma representação JSON para o objeto [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="9b19b-128">In the request body, supply a JSON representation for the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>

<span data-ttu-id="9b19b-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="9b19b-129">The following table shows the properties that are required when you create the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md).</span></span>

|<span data-ttu-id="9b19b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9b19b-130">Property</span></span>|<span data-ttu-id="9b19b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9b19b-131">Type</span></span>|<span data-ttu-id="9b19b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b19b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b19b-133">id</span><span class="sxs-lookup"><span data-stu-id="9b19b-133">id</span></span>|<span data-ttu-id="9b19b-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9b19b-134">String</span></span>|<span data-ttu-id="9b19b-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9b19b-135">Key of the entity.</span></span>|
|<span data-ttu-id="9b19b-136">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9b19b-136">installedDeviceCount</span></span>|<span data-ttu-id="9b19b-137">Int32</span><span class="sxs-lookup"><span data-stu-id="9b19b-137">Int32</span></span>|<span data-ttu-id="9b19b-138">Número de dispositivos que instalou com sucesso deste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9b19b-138">Number of Devices that have successfully installed this app.</span></span>|
|<span data-ttu-id="9b19b-139">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9b19b-139">failedDeviceCount</span></span>|<span data-ttu-id="9b19b-140">Int32</span><span class="sxs-lookup"><span data-stu-id="9b19b-140">Int32</span></span>|<span data-ttu-id="9b19b-141">Número de dispositivos que não tenha conseguido instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9b19b-141">Number of Devices that have failed to install this app.</span></span>|
|<span data-ttu-id="9b19b-142">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9b19b-142">notApplicableDeviceCount</span></span>|<span data-ttu-id="9b19b-143">Int32</span><span class="sxs-lookup"><span data-stu-id="9b19b-143">Int32</span></span>|<span data-ttu-id="9b19b-144">Número de dispositivos que não são aplicáveis para esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9b19b-144">Number of Devices that are not applicable for this app.</span></span>|
|<span data-ttu-id="9b19b-145">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9b19b-145">notInstalledDeviceCount</span></span>|<span data-ttu-id="9b19b-146">Int32</span><span class="sxs-lookup"><span data-stu-id="9b19b-146">Int32</span></span>|<span data-ttu-id="9b19b-147">Número de dispositivos que não tem este aplicativo instalado.</span><span class="sxs-lookup"><span data-stu-id="9b19b-147">Number of Devices that does not have this app installed.</span></span>|
|<span data-ttu-id="9b19b-148">pendingInstallDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9b19b-148">pendingInstallDeviceCount</span></span>|<span data-ttu-id="9b19b-149">Int32</span><span class="sxs-lookup"><span data-stu-id="9b19b-149">Int32</span></span>|<span data-ttu-id="9b19b-150">Número de dispositivos que foram notificados para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9b19b-150">Number of Devices that have been notified to install this app.</span></span>|
|<span data-ttu-id="9b19b-151">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="9b19b-151">installedUserCount</span></span>|<span data-ttu-id="9b19b-152">Int32</span><span class="sxs-lookup"><span data-stu-id="9b19b-152">Int32</span></span>|<span data-ttu-id="9b19b-153">Número de usuários cujos dispositivos tiveram êxito para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9b19b-153">Number of Users whose devices have all succeeded to install this app.</span></span>|
|<span data-ttu-id="9b19b-154">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="9b19b-154">failedUserCount</span></span>|<span data-ttu-id="9b19b-155">Int32</span><span class="sxs-lookup"><span data-stu-id="9b19b-155">Int32</span></span>|<span data-ttu-id="9b19b-156">Número de usuários que têm 1 ou mais dispositivo com falha para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9b19b-156">Number of Users that have 1 or more device that failed to install this app.</span></span>|
|<span data-ttu-id="9b19b-157">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="9b19b-157">notApplicableUserCount</span></span>|<span data-ttu-id="9b19b-158">Int32</span><span class="sxs-lookup"><span data-stu-id="9b19b-158">Int32</span></span>|<span data-ttu-id="9b19b-159">Número de usuários cujos dispositivos tudo não eram aplicáveis para esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9b19b-159">Number of Users whose devices were all not applicable for this app.</span></span>|
|<span data-ttu-id="9b19b-160">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="9b19b-160">notInstalledUserCount</span></span>|<span data-ttu-id="9b19b-161">Int32</span><span class="sxs-lookup"><span data-stu-id="9b19b-161">Int32</span></span>|<span data-ttu-id="9b19b-162">Número de usuários que têm 1 ou mais dispositivos que não tiver instalado esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9b19b-162">Number of Users that have 1 or more devices that did not install this app.</span></span>|
|<span data-ttu-id="9b19b-163">pendingInstallUserCount</span><span class="sxs-lookup"><span data-stu-id="9b19b-163">pendingInstallUserCount</span></span>|<span data-ttu-id="9b19b-164">Int32</span><span class="sxs-lookup"><span data-stu-id="9b19b-164">Int32</span></span>|<span data-ttu-id="9b19b-165">Número de usuários que têm 1 ou mais dispositivo que foram notificados para instalar esse aplicativo e tiver 0 dispositivos com falhas.</span><span class="sxs-lookup"><span data-stu-id="9b19b-165">Number of Users that have 1 or more device that have been notified to install this app and have 0 devices with failures.</span></span>|



## <a name="response"></a><span data-ttu-id="9b19b-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b19b-166">Response</span></span>
<span data-ttu-id="9b19b-167">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9b19b-167">If successful, this method returns a `200 OK` response code and an updated [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b19b-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9b19b-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="9b19b-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9b19b-169">Request</span></span>
<span data-ttu-id="9b19b-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9b19b-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/installSummary
Content-type: application/json
Content-length: 312

{
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

### <a name="response"></a><span data-ttu-id="9b19b-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b19b-171">Response</span></span>
<span data-ttu-id="9b19b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9b19b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





