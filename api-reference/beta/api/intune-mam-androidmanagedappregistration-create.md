---
title: Criar androidManagedAppRegistration
description: Cria um novo objeto androidManagedAppRegistration.
ms.openlocfilehash: c7e88b7cb6f12e7784c2e33523dd7b5da8c53c75
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037541"
---
# <a name="create-androidmanagedappregistration"></a><span data-ttu-id="c4a11-103">Criar androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="c4a11-103">Create androidManagedAppRegistration</span></span>

> <span data-ttu-id="c4a11-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c4a11-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c4a11-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c4a11-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c4a11-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c4a11-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c4a11-107">Cria um novo objeto [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="c4a11-107">Create a new [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c4a11-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c4a11-108">Prerequisites</span></span>
<span data-ttu-id="c4a11-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4a11-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4a11-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c4a11-111">Permission type</span></span>|<span data-ttu-id="c4a11-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c4a11-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4a11-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c4a11-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c4a11-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4a11-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c4a11-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c4a11-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4a11-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4a11-116">Not supported.</span></span>|
|<span data-ttu-id="c4a11-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c4a11-117">Application</span></span>|<span data-ttu-id="c4a11-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4a11-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4a11-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c4a11-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="c4a11-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c4a11-120">Request headers</span></span>
|<span data-ttu-id="c4a11-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c4a11-121">Header</span></span>|<span data-ttu-id="c4a11-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c4a11-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4a11-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c4a11-123">Authorization</span></span>|<span data-ttu-id="c4a11-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4a11-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4a11-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c4a11-125">Accept</span></span>|<span data-ttu-id="c4a11-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c4a11-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4a11-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c4a11-127">Request body</span></span>
<span data-ttu-id="c4a11-128">No corpo da solicitação, forneça uma representação JSON do objeto androidManagedAppRegistration.</span><span class="sxs-lookup"><span data-stu-id="c4a11-128">In the request body, supply a JSON representation for the androidManagedAppRegistration object.</span></span>

<span data-ttu-id="c4a11-129">A tabela a seguir mostra as propriedades que são necessárias ao criar androidManagedAppRegistration.</span><span class="sxs-lookup"><span data-stu-id="c4a11-129">The following table shows the properties that are required when you create the androidManagedAppRegistration.</span></span>

|<span data-ttu-id="c4a11-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c4a11-130">Property</span></span>|<span data-ttu-id="c4a11-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c4a11-131">Type</span></span>|<span data-ttu-id="c4a11-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4a11-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4a11-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c4a11-133">createdDateTime</span></span>|<span data-ttu-id="c4a11-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4a11-134">DateTimeOffset</span></span>|<span data-ttu-id="c4a11-135">Data e hora de criação. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="c4a11-135">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c4a11-136">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="c4a11-136">lastSyncDateTime</span></span>|<span data-ttu-id="c4a11-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4a11-137">DateTimeOffset</span></span>|<span data-ttu-id="c4a11-138">Data e hora em que o último aplicativo foi sincronizado com o serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="c4a11-138">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="c4a11-139">Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="c4a11-139">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c4a11-140">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="c4a11-140">applicationVersion</span></span>|<span data-ttu-id="c4a11-141">String</span><span class="sxs-lookup"><span data-stu-id="c4a11-141">String</span></span>|<span data-ttu-id="c4a11-142">Versão do aplicativo. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="c4a11-142">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c4a11-143">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="c4a11-143">managementSdkVersion</span></span>|<span data-ttu-id="c4a11-144">String</span><span class="sxs-lookup"><span data-stu-id="c4a11-144">String</span></span>|<span data-ttu-id="c4a11-145">Versão do SDK do gerenciamento de aplicativos. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="c4a11-145">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c4a11-146">platformVersion</span><span class="sxs-lookup"><span data-stu-id="c4a11-146">platformVersion</span></span>|<span data-ttu-id="c4a11-147">String</span><span class="sxs-lookup"><span data-stu-id="c4a11-147">String</span></span>|<span data-ttu-id="c4a11-148">Versão do sistema operacional. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="c4a11-148">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c4a11-149">deviceType</span><span class="sxs-lookup"><span data-stu-id="c4a11-149">deviceType</span></span>|<span data-ttu-id="c4a11-150">String</span><span class="sxs-lookup"><span data-stu-id="c4a11-150">String</span></span>|<span data-ttu-id="c4a11-151">Tipo de dispositivo do host. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="c4a11-151">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c4a11-152">deviceTag</span><span class="sxs-lookup"><span data-stu-id="c4a11-152">deviceTag</span></span>|<span data-ttu-id="c4a11-153">String</span><span class="sxs-lookup"><span data-stu-id="c4a11-153">String</span></span>|<span data-ttu-id="c4a11-154">Uma tag gerada pelo SDK de gerenciamento, que ajuda a relacionar aplicativos hospedados no mesmo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c4a11-154">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="c4a11-155">Sem garantia de indicar aplicativos em todas as condições.</span><span class="sxs-lookup"><span data-stu-id="c4a11-155">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="c4a11-156">Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="c4a11-156">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c4a11-157">deviceName</span><span class="sxs-lookup"><span data-stu-id="c4a11-157">deviceName</span></span>|<span data-ttu-id="c4a11-158">String</span><span class="sxs-lookup"><span data-stu-id="c4a11-158">String</span></span>|<span data-ttu-id="c4a11-159">Nome de dispositivo do host. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="c4a11-159">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c4a11-160">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="c4a11-160">managedDeviceId</span></span>|<span data-ttu-id="c4a11-161">String</span><span class="sxs-lookup"><span data-stu-id="c4a11-161">String</span></span>|<span data-ttu-id="c4a11-162">O identificador de dispositivo gerenciado do dispositivo de host.</span><span class="sxs-lookup"><span data-stu-id="c4a11-162">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="c4a11-163">Valor poderia ser vazia, mesmo quando o dispositivo do host é gerenciado.</span><span class="sxs-lookup"><span data-stu-id="c4a11-163">Value could be empty even when the host device is managed.</span></span> <span data-ttu-id="c4a11-164">Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="c4a11-164">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c4a11-165">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="c4a11-165">azureADDeviceId</span></span>|<span data-ttu-id="c4a11-166">String</span><span class="sxs-lookup"><span data-stu-id="c4a11-166">String</span></span>|<span data-ttu-id="c4a11-167">O identificador de dispositivo do Azure Active Directory do dispositivo de host.</span><span class="sxs-lookup"><span data-stu-id="c4a11-167">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="c4a11-168">Valor poderia ser vazia, mesmo quando o dispositivo do host é o Azure Active Directory registrada.</span><span class="sxs-lookup"><span data-stu-id="c4a11-168">Value could be empty even when the host device is Azure Active Directory registered.</span></span> <span data-ttu-id="c4a11-169">Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="c4a11-169">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c4a11-170">deviceModel</span><span class="sxs-lookup"><span data-stu-id="c4a11-170">deviceModel</span></span>|<span data-ttu-id="c4a11-171">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c4a11-171">String</span></span>|<span data-ttu-id="c4a11-172">O modelo de dispositivo para que o registro atual do aplicativo Inherited de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="c4a11-172">The device model for the current app registration  Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c4a11-173">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="c4a11-173">deviceManufacturer</span></span>|<span data-ttu-id="c4a11-174">String</span><span class="sxs-lookup"><span data-stu-id="c4a11-174">String</span></span>|<span data-ttu-id="c4a11-175">O fabricante do dispositivo para que o registro atual do aplicativo Inherited de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="c4a11-175">The device manufacturer for the current app registration  Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c4a11-176">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="c4a11-176">flaggedReasons</span></span>|<span data-ttu-id="c4a11-177">coleção [managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)</span><span class="sxs-lookup"><span data-stu-id="c4a11-177">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="c4a11-178">Zero ou mais motivos para a sinalização de um registro de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c4a11-178">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="c4a11-179">E.g.</span><span class="sxs-lookup"><span data-stu-id="c4a11-179">E.g.</span></span> <span data-ttu-id="c4a11-180">aplicativo em execução no dispositivo com raiz Inherited de [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="c4a11-180">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span></span> <span data-ttu-id="c4a11-181">Os valores possíveis são: `none` e `rootedDevice`.</span><span class="sxs-lookup"><span data-stu-id="c4a11-181">Possible values are: `none`, `rootedDevice`.</span></span>|
|<span data-ttu-id="c4a11-182">userId</span><span class="sxs-lookup"><span data-stu-id="c4a11-182">userId</span></span>|<span data-ttu-id="c4a11-183">String</span><span class="sxs-lookup"><span data-stu-id="c4a11-183">String</span></span>|<span data-ttu-id="c4a11-184">A ID de usuário à qual este registro de aplicativo pertence.</span><span class="sxs-lookup"><span data-stu-id="c4a11-184">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="c4a11-185">Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="c4a11-185">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c4a11-186">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="c4a11-186">appIdentifier</span></span>|[<span data-ttu-id="c4a11-187">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="c4a11-187">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="c4a11-188">O Identificador de pacote do aplicativo. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="c4a11-188">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c4a11-189">id</span><span class="sxs-lookup"><span data-stu-id="c4a11-189">id</span></span>|<span data-ttu-id="c4a11-190">String</span><span class="sxs-lookup"><span data-stu-id="c4a11-190">String</span></span>|<span data-ttu-id="c4a11-191">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c4a11-191">Key of the entity.</span></span> <span data-ttu-id="c4a11-192">Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="c4a11-192">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c4a11-193">version</span><span class="sxs-lookup"><span data-stu-id="c4a11-193">version</span></span>|<span data-ttu-id="c4a11-194">String</span><span class="sxs-lookup"><span data-stu-id="c4a11-194">String</span></span>|<span data-ttu-id="c4a11-195">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="c4a11-195">Version of the entity.</span></span> <span data-ttu-id="c4a11-196">Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="c4a11-196">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="c4a11-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4a11-197">Response</span></span>
<span data-ttu-id="c4a11-198">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c4a11-198">If successful, this method returns a `201 Created` response code and a [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4a11-199">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c4a11-199">Example</span></span>
### <a name="request"></a><span data-ttu-id="c4a11-200">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4a11-200">Request</span></span>
<span data-ttu-id="c4a11-201">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c4a11-201">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c4a11-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4a11-202">Response</span></span>
<span data-ttu-id="c4a11-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c4a11-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





