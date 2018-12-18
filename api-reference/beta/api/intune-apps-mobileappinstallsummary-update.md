---
title: Atualizar mobileAppInstallSummary
description: Atualize as propriedades de um objeto mobileAppInstallSummary.
author: tfitzmac
ms.openlocfilehash: 94dc7fa5023d26de91b4d64efda27332dd51de63
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315635"
---
# <a name="update-mobileappinstallsummary"></a><span data-ttu-id="3472f-103">Atualizar mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="3472f-103">Update mobileAppInstallSummary</span></span>

> <span data-ttu-id="3472f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3472f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3472f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3472f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3472f-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3472f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3472f-107">Atualize as propriedades de um objeto [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="3472f-107">Update the properties of a [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3472f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3472f-108">Prerequisites</span></span>
<span data-ttu-id="3472f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3472f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3472f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3472f-111">Permission type</span></span>|<span data-ttu-id="3472f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3472f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3472f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3472f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3472f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3472f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3472f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3472f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3472f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3472f-116">Not supported.</span></span>|
|<span data-ttu-id="3472f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3472f-117">Application</span></span>|<span data-ttu-id="3472f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3472f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3472f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3472f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="3472f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3472f-120">Request headers</span></span>
|<span data-ttu-id="3472f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3472f-121">Header</span></span>|<span data-ttu-id="3472f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3472f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3472f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3472f-123">Authorization</span></span>|<span data-ttu-id="3472f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3472f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3472f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3472f-125">Accept</span></span>|<span data-ttu-id="3472f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3472f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3472f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3472f-127">Request body</span></span>
<span data-ttu-id="3472f-128">No corpo da solicitação, fornece uma representação JSON para o objeto [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="3472f-128">In the request body, supply a JSON representation for the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>

<span data-ttu-id="3472f-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="3472f-129">The following table shows the properties that are required when you create the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md).</span></span>

|<span data-ttu-id="3472f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3472f-130">Property</span></span>|<span data-ttu-id="3472f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3472f-131">Type</span></span>|<span data-ttu-id="3472f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3472f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3472f-133">id</span><span class="sxs-lookup"><span data-stu-id="3472f-133">id</span></span>|<span data-ttu-id="3472f-134">String</span><span class="sxs-lookup"><span data-stu-id="3472f-134">String</span></span>|<span data-ttu-id="3472f-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3472f-135">Key of the entity.</span></span>|
|<span data-ttu-id="3472f-136">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3472f-136">installedDeviceCount</span></span>|<span data-ttu-id="3472f-137">Int32</span><span class="sxs-lookup"><span data-stu-id="3472f-137">Int32</span></span>|<span data-ttu-id="3472f-138">Número de dispositivos que instalou com sucesso deste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3472f-138">Number of Devices that have successfully installed this app.</span></span>|
|<span data-ttu-id="3472f-139">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3472f-139">failedDeviceCount</span></span>|<span data-ttu-id="3472f-140">Int32</span><span class="sxs-lookup"><span data-stu-id="3472f-140">Int32</span></span>|<span data-ttu-id="3472f-141">Número de dispositivos que não tenha conseguido instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3472f-141">Number of Devices that have failed to install this app.</span></span>|
|<span data-ttu-id="3472f-142">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3472f-142">notApplicableDeviceCount</span></span>|<span data-ttu-id="3472f-143">Int32</span><span class="sxs-lookup"><span data-stu-id="3472f-143">Int32</span></span>|<span data-ttu-id="3472f-144">Número de dispositivos que não são aplicáveis para esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3472f-144">Number of Devices that are not applicable for this app.</span></span>|
|<span data-ttu-id="3472f-145">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3472f-145">notInstalledDeviceCount</span></span>|<span data-ttu-id="3472f-146">Int32</span><span class="sxs-lookup"><span data-stu-id="3472f-146">Int32</span></span>|<span data-ttu-id="3472f-147">Número de dispositivos que não tem este aplicativo instalado.</span><span class="sxs-lookup"><span data-stu-id="3472f-147">Number of Devices that does not have this app installed.</span></span>|
|<span data-ttu-id="3472f-148">pendingInstallDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3472f-148">pendingInstallDeviceCount</span></span>|<span data-ttu-id="3472f-149">Int32</span><span class="sxs-lookup"><span data-stu-id="3472f-149">Int32</span></span>|<span data-ttu-id="3472f-150">Número de dispositivos que foram notificados para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3472f-150">Number of Devices that have been notified to install this app.</span></span>|
|<span data-ttu-id="3472f-151">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="3472f-151">installedUserCount</span></span>|<span data-ttu-id="3472f-152">Int32</span><span class="sxs-lookup"><span data-stu-id="3472f-152">Int32</span></span>|<span data-ttu-id="3472f-153">Número de usuários cujos dispositivos tiveram êxito para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3472f-153">Number of Users whose devices have all succeeded to install this app.</span></span>|
|<span data-ttu-id="3472f-154">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="3472f-154">failedUserCount</span></span>|<span data-ttu-id="3472f-155">Int32</span><span class="sxs-lookup"><span data-stu-id="3472f-155">Int32</span></span>|<span data-ttu-id="3472f-156">Número de usuários que têm 1 ou mais dispositivo com falha para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3472f-156">Number of Users that have 1 or more device that failed to install this app.</span></span>|
|<span data-ttu-id="3472f-157">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="3472f-157">notApplicableUserCount</span></span>|<span data-ttu-id="3472f-158">Int32</span><span class="sxs-lookup"><span data-stu-id="3472f-158">Int32</span></span>|<span data-ttu-id="3472f-159">Número de usuários cujos dispositivos tudo não eram aplicáveis para esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3472f-159">Number of Users whose devices were all not applicable for this app.</span></span>|
|<span data-ttu-id="3472f-160">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="3472f-160">notInstalledUserCount</span></span>|<span data-ttu-id="3472f-161">Int32</span><span class="sxs-lookup"><span data-stu-id="3472f-161">Int32</span></span>|<span data-ttu-id="3472f-162">Número de usuários que têm 1 ou mais dispositivos que não tiver instalado esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3472f-162">Number of Users that have 1 or more devices that did not install this app.</span></span>|
|<span data-ttu-id="3472f-163">pendingInstallUserCount</span><span class="sxs-lookup"><span data-stu-id="3472f-163">pendingInstallUserCount</span></span>|<span data-ttu-id="3472f-164">Int32</span><span class="sxs-lookup"><span data-stu-id="3472f-164">Int32</span></span>|<span data-ttu-id="3472f-165">Número de usuários que têm 1 ou mais dispositivo que foram notificados para instalar esse aplicativo e tiver 0 dispositivos com falhas.</span><span class="sxs-lookup"><span data-stu-id="3472f-165">Number of Users that have 1 or more device that have been notified to install this app and have 0 devices with failures.</span></span>|



## <a name="response"></a><span data-ttu-id="3472f-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="3472f-166">Response</span></span>
<span data-ttu-id="3472f-167">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3472f-167">If successful, this method returns a `200 OK` response code and an updated [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3472f-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3472f-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="3472f-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3472f-169">Request</span></span>
<span data-ttu-id="3472f-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3472f-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3472f-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="3472f-171">Response</span></span>
<span data-ttu-id="3472f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3472f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





