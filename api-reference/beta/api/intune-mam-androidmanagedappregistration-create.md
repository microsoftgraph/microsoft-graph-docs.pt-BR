---
title: Criar androidManagedAppRegistration
description: Cria um novo objeto androidManagedAppRegistration.
author: tfitzmac
ms.openlocfilehash: 074d8d01a086956af1f88e0d0315ccc84b84c9cf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326758"
---
# <a name="create-androidmanagedappregistration"></a><span data-ttu-id="652f2-103">Criar androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="652f2-103">Create androidManagedAppRegistration</span></span>

> <span data-ttu-id="652f2-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="652f2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="652f2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="652f2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="652f2-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="652f2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="652f2-107">Cria um novo objeto [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="652f2-107">Create a new [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="652f2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="652f2-108">Prerequisites</span></span>
<span data-ttu-id="652f2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="652f2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="652f2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="652f2-111">Permission type</span></span>|<span data-ttu-id="652f2-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="652f2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="652f2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="652f2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="652f2-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="652f2-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="652f2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="652f2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="652f2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="652f2-116">Not supported.</span></span>|
|<span data-ttu-id="652f2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="652f2-117">Application</span></span>|<span data-ttu-id="652f2-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="652f2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="652f2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="652f2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="652f2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="652f2-120">Request headers</span></span>
|<span data-ttu-id="652f2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="652f2-121">Header</span></span>|<span data-ttu-id="652f2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="652f2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="652f2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="652f2-123">Authorization</span></span>|<span data-ttu-id="652f2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="652f2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="652f2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="652f2-125">Accept</span></span>|<span data-ttu-id="652f2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="652f2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="652f2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="652f2-127">Request body</span></span>
<span data-ttu-id="652f2-128">No corpo da solicitação, forneça uma representação JSON do objeto androidManagedAppRegistration.</span><span class="sxs-lookup"><span data-stu-id="652f2-128">In the request body, supply a JSON representation for the androidManagedAppRegistration object.</span></span>

<span data-ttu-id="652f2-129">A tabela a seguir mostra as propriedades que são necessárias ao criar androidManagedAppRegistration.</span><span class="sxs-lookup"><span data-stu-id="652f2-129">The following table shows the properties that are required when you create the androidManagedAppRegistration.</span></span>

|<span data-ttu-id="652f2-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="652f2-130">Property</span></span>|<span data-ttu-id="652f2-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="652f2-131">Type</span></span>|<span data-ttu-id="652f2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="652f2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="652f2-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="652f2-133">createdDateTime</span></span>|<span data-ttu-id="652f2-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="652f2-134">DateTimeOffset</span></span>|<span data-ttu-id="652f2-135">Data e hora de criação. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="652f2-135">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="652f2-136">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="652f2-136">lastSyncDateTime</span></span>|<span data-ttu-id="652f2-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="652f2-137">DateTimeOffset</span></span>|<span data-ttu-id="652f2-138">Data e hora em que o último aplicativo foi sincronizado com o serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="652f2-138">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="652f2-139">Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="652f2-139">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="652f2-140">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="652f2-140">applicationVersion</span></span>|<span data-ttu-id="652f2-141">String</span><span class="sxs-lookup"><span data-stu-id="652f2-141">String</span></span>|<span data-ttu-id="652f2-142">Versão do aplicativo. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="652f2-142">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="652f2-143">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="652f2-143">managementSdkVersion</span></span>|<span data-ttu-id="652f2-144">String</span><span class="sxs-lookup"><span data-stu-id="652f2-144">String</span></span>|<span data-ttu-id="652f2-145">Versão do SDK do gerenciamento de aplicativos. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="652f2-145">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="652f2-146">platformVersion</span><span class="sxs-lookup"><span data-stu-id="652f2-146">platformVersion</span></span>|<span data-ttu-id="652f2-147">String</span><span class="sxs-lookup"><span data-stu-id="652f2-147">String</span></span>|<span data-ttu-id="652f2-148">Versão do sistema operacional. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="652f2-148">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="652f2-149">deviceType</span><span class="sxs-lookup"><span data-stu-id="652f2-149">deviceType</span></span>|<span data-ttu-id="652f2-150">String</span><span class="sxs-lookup"><span data-stu-id="652f2-150">String</span></span>|<span data-ttu-id="652f2-151">Tipo de dispositivo do host. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="652f2-151">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="652f2-152">deviceTag</span><span class="sxs-lookup"><span data-stu-id="652f2-152">deviceTag</span></span>|<span data-ttu-id="652f2-153">String</span><span class="sxs-lookup"><span data-stu-id="652f2-153">String</span></span>|<span data-ttu-id="652f2-154">Uma tag gerada pelo SDK de gerenciamento, que ajuda a relacionar aplicativos hospedados no mesmo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="652f2-154">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="652f2-155">Sem garantia de indicar aplicativos em todas as condições.</span><span class="sxs-lookup"><span data-stu-id="652f2-155">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="652f2-156">Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="652f2-156">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="652f2-157">deviceName</span><span class="sxs-lookup"><span data-stu-id="652f2-157">deviceName</span></span>|<span data-ttu-id="652f2-158">String</span><span class="sxs-lookup"><span data-stu-id="652f2-158">String</span></span>|<span data-ttu-id="652f2-159">Nome de dispositivo do host. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="652f2-159">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="652f2-160">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="652f2-160">managedDeviceId</span></span>|<span data-ttu-id="652f2-161">String</span><span class="sxs-lookup"><span data-stu-id="652f2-161">String</span></span>|<span data-ttu-id="652f2-162">O identificador de dispositivo gerenciado do dispositivo de host.</span><span class="sxs-lookup"><span data-stu-id="652f2-162">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="652f2-163">Valor poderia ser vazia, mesmo quando o dispositivo do host é gerenciado.</span><span class="sxs-lookup"><span data-stu-id="652f2-163">Value could be empty even when the host device is managed.</span></span> <span data-ttu-id="652f2-164">Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="652f2-164">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="652f2-165">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="652f2-165">azureADDeviceId</span></span>|<span data-ttu-id="652f2-166">String</span><span class="sxs-lookup"><span data-stu-id="652f2-166">String</span></span>|<span data-ttu-id="652f2-167">O identificador de dispositivo do Azure Active Directory do dispositivo de host.</span><span class="sxs-lookup"><span data-stu-id="652f2-167">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="652f2-168">Valor poderia ser vazia, mesmo quando o dispositivo do host é o Azure Active Directory registrada.</span><span class="sxs-lookup"><span data-stu-id="652f2-168">Value could be empty even when the host device is Azure Active Directory registered.</span></span> <span data-ttu-id="652f2-169">Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="652f2-169">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="652f2-170">deviceModel</span><span class="sxs-lookup"><span data-stu-id="652f2-170">deviceModel</span></span>|<span data-ttu-id="652f2-171">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="652f2-171">String</span></span>|<span data-ttu-id="652f2-172">O modelo de dispositivo para que o registro atual do aplicativo Inherited de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="652f2-172">The device model for the current app registration  Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="652f2-173">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="652f2-173">deviceManufacturer</span></span>|<span data-ttu-id="652f2-174">String</span><span class="sxs-lookup"><span data-stu-id="652f2-174">String</span></span>|<span data-ttu-id="652f2-175">O fabricante do dispositivo para que o registro atual do aplicativo Inherited de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="652f2-175">The device manufacturer for the current app registration  Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="652f2-176">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="652f2-176">flaggedReasons</span></span>|<span data-ttu-id="652f2-177">coleção [managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)</span><span class="sxs-lookup"><span data-stu-id="652f2-177">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="652f2-178">Zero ou mais motivos para a sinalização de um registro de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="652f2-178">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="652f2-179">E.g.</span><span class="sxs-lookup"><span data-stu-id="652f2-179">E.g.</span></span> <span data-ttu-id="652f2-180">aplicativo em execução no dispositivo com raiz Inherited de [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="652f2-180">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span></span> <span data-ttu-id="652f2-181">Os valores possíveis são: `none` e `rootedDevice`.</span><span class="sxs-lookup"><span data-stu-id="652f2-181">Possible values are: `none`, `rootedDevice`.</span></span>|
|<span data-ttu-id="652f2-182">userId</span><span class="sxs-lookup"><span data-stu-id="652f2-182">userId</span></span>|<span data-ttu-id="652f2-183">String</span><span class="sxs-lookup"><span data-stu-id="652f2-183">String</span></span>|<span data-ttu-id="652f2-184">A ID de usuário à qual este registro de aplicativo pertence.</span><span class="sxs-lookup"><span data-stu-id="652f2-184">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="652f2-185">Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="652f2-185">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="652f2-186">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="652f2-186">appIdentifier</span></span>|[<span data-ttu-id="652f2-187">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="652f2-187">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="652f2-188">O Identificador de pacote do aplicativo. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="652f2-188">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="652f2-189">id</span><span class="sxs-lookup"><span data-stu-id="652f2-189">id</span></span>|<span data-ttu-id="652f2-190">String</span><span class="sxs-lookup"><span data-stu-id="652f2-190">String</span></span>|<span data-ttu-id="652f2-191">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="652f2-191">Key of the entity.</span></span> <span data-ttu-id="652f2-192">Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="652f2-192">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="652f2-193">version</span><span class="sxs-lookup"><span data-stu-id="652f2-193">version</span></span>|<span data-ttu-id="652f2-194">String</span><span class="sxs-lookup"><span data-stu-id="652f2-194">String</span></span>|<span data-ttu-id="652f2-195">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="652f2-195">Version of the entity.</span></span> <span data-ttu-id="652f2-196">Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="652f2-196">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="652f2-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="652f2-197">Response</span></span>
<span data-ttu-id="652f2-198">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="652f2-198">If successful, this method returns a `201 Created` response code and a [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="652f2-199">Exemplo</span><span class="sxs-lookup"><span data-stu-id="652f2-199">Example</span></span>
### <a name="request"></a><span data-ttu-id="652f2-200">Solicitação</span><span class="sxs-lookup"><span data-stu-id="652f2-200">Request</span></span>
<span data-ttu-id="652f2-201">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="652f2-201">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations
Content-type: application/json
Content-length: 837

{
  "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "applicationVersion": "Application Version value",
  "managementSdkVersion": "Management Sdk Version value",
  "platformVersion": "Platform Version value",
  "deviceType": "Device Type value",
  "deviceTag": "Device Tag value",
  "deviceName": "Device Name value",
  "managedDeviceId": "Managed Device Id value",
  "azureADDeviceId": "Azure ADDevice Id value",
  "deviceModel": "Device Model value",
  "deviceManufacturer": "Device Manufacturer value",
  "flaggedReasons": [
    "rootedDevice"
  ],
  "userId": "User Id value",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="652f2-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="652f2-202">Response</span></span>
<span data-ttu-id="652f2-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="652f2-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 945

{
  "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "applicationVersion": "Application Version value",
  "managementSdkVersion": "Management Sdk Version value",
  "platformVersion": "Platform Version value",
  "deviceType": "Device Type value",
  "deviceTag": "Device Tag value",
  "deviceName": "Device Name value",
  "managedDeviceId": "Managed Device Id value",
  "azureADDeviceId": "Azure ADDevice Id value",
  "deviceModel": "Device Model value",
  "deviceManufacturer": "Device Manufacturer value",
  "flaggedReasons": [
    "rootedDevice"
  ],
  "userId": "User Id value",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "id": "0e064997-4997-0e06-9749-060e9749060e",
  "version": "Version value"
}
```





