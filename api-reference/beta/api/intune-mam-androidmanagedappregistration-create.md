---
title: Criar androidManagedAppRegistration
description: Cria um novo objeto androidManagedAppRegistration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d7db9b46f6615f5e49026014db7395f88e35200e
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39942504"
---
# <a name="create-androidmanagedappregistration"></a><span data-ttu-id="4fe14-103">Criar androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="4fe14-103">Create androidManagedAppRegistration</span></span>

> <span data-ttu-id="4fe14-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4fe14-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4fe14-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4fe14-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4fe14-106">Cria um novo objeto [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="4fe14-106">Create a new [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4fe14-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4fe14-107">Prerequisites</span></span>
<span data-ttu-id="4fe14-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4fe14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4fe14-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4fe14-110">Permission type</span></span>|<span data-ttu-id="4fe14-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4fe14-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4fe14-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4fe14-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4fe14-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fe14-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4fe14-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4fe14-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4fe14-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4fe14-115">Not supported.</span></span>|
|<span data-ttu-id="4fe14-116">Application</span><span class="sxs-lookup"><span data-stu-id="4fe14-116">Application</span></span>|<span data-ttu-id="4fe14-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fe14-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4fe14-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4fe14-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="4fe14-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4fe14-119">Request headers</span></span>
|<span data-ttu-id="4fe14-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4fe14-120">Header</span></span>|<span data-ttu-id="4fe14-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4fe14-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4fe14-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4fe14-122">Authorization</span></span>|<span data-ttu-id="4fe14-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4fe14-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4fe14-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4fe14-124">Accept</span></span>|<span data-ttu-id="4fe14-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4fe14-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4fe14-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4fe14-126">Request body</span></span>
<span data-ttu-id="4fe14-127">No corpo da solicitação, forneça uma representação JSON do objeto androidManagedAppRegistration.</span><span class="sxs-lookup"><span data-stu-id="4fe14-127">In the request body, supply a JSON representation for the androidManagedAppRegistration object.</span></span>

<span data-ttu-id="4fe14-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidManagedAppRegistration.</span><span class="sxs-lookup"><span data-stu-id="4fe14-128">The following table shows the properties that are required when you create the androidManagedAppRegistration.</span></span>

|<span data-ttu-id="4fe14-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4fe14-129">Property</span></span>|<span data-ttu-id="4fe14-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4fe14-130">Type</span></span>|<span data-ttu-id="4fe14-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4fe14-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fe14-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4fe14-132">createdDateTime</span></span>|<span data-ttu-id="4fe14-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4fe14-133">DateTimeOffset</span></span>|<span data-ttu-id="4fe14-134">Data e hora de criação. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="4fe14-134">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="4fe14-135">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="4fe14-135">lastSyncDateTime</span></span>|<span data-ttu-id="4fe14-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4fe14-136">DateTimeOffset</span></span>|<span data-ttu-id="4fe14-137">Data e hora em que o último aplicativo foi sincronizado com o serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="4fe14-137">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="4fe14-138">Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="4fe14-138">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="4fe14-139">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="4fe14-139">applicationVersion</span></span>|<span data-ttu-id="4fe14-140">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="4fe14-140">String</span></span>|<span data-ttu-id="4fe14-141">Versão do aplicativo. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="4fe14-141">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="4fe14-142">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="4fe14-142">managementSdkVersion</span></span>|<span data-ttu-id="4fe14-143">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="4fe14-143">String</span></span>|<span data-ttu-id="4fe14-144">Versão do SDK do gerenciamento de aplicativos. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="4fe14-144">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="4fe14-145">platformVersion</span><span class="sxs-lookup"><span data-stu-id="4fe14-145">platformVersion</span></span>|<span data-ttu-id="4fe14-146">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="4fe14-146">String</span></span>|<span data-ttu-id="4fe14-147">Versão do sistema operacional. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="4fe14-147">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="4fe14-148">deviceType</span><span class="sxs-lookup"><span data-stu-id="4fe14-148">deviceType</span></span>|<span data-ttu-id="4fe14-149">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="4fe14-149">String</span></span>|<span data-ttu-id="4fe14-150">Tipo de dispositivo do host. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="4fe14-150">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="4fe14-151">deviceTag</span><span class="sxs-lookup"><span data-stu-id="4fe14-151">deviceTag</span></span>|<span data-ttu-id="4fe14-152">String</span><span class="sxs-lookup"><span data-stu-id="4fe14-152">String</span></span>|<span data-ttu-id="4fe14-153">Uma tag gerada pelo SDK de gerenciamento, que ajuda a relacionar aplicativos hospedados no mesmo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4fe14-153">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="4fe14-154">Sem garantia de indicar aplicativos em todas as condições.</span><span class="sxs-lookup"><span data-stu-id="4fe14-154">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="4fe14-155">Herdada da [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="4fe14-155">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="4fe14-156">deviceName</span><span class="sxs-lookup"><span data-stu-id="4fe14-156">deviceName</span></span>|<span data-ttu-id="4fe14-157">String</span><span class="sxs-lookup"><span data-stu-id="4fe14-157">String</span></span>|<span data-ttu-id="4fe14-158">Nome de dispositivo do host. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="4fe14-158">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="4fe14-159">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="4fe14-159">managedDeviceId</span></span>|<span data-ttu-id="4fe14-160">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="4fe14-160">String</span></span>|<span data-ttu-id="4fe14-161">O identificador de dispositivo gerenciado do dispositivo host.</span><span class="sxs-lookup"><span data-stu-id="4fe14-161">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="4fe14-162">O valor pode ser vazio mesmo quando o dispositivo host é gerenciado.</span><span class="sxs-lookup"><span data-stu-id="4fe14-162">Value could be empty even when the host device is managed.</span></span> <span data-ttu-id="4fe14-163">Herdada da [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="4fe14-163">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="4fe14-164">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="4fe14-164">azureADDeviceId</span></span>|<span data-ttu-id="4fe14-165">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="4fe14-165">String</span></span>|<span data-ttu-id="4fe14-166">O identificador de dispositivo do Azure Active Directory do dispositivo host.</span><span class="sxs-lookup"><span data-stu-id="4fe14-166">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="4fe14-167">O valor pode ser vazio mesmo quando o dispositivo host é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4fe14-167">Value could be empty even when the host device is Azure Active Directory registered.</span></span> <span data-ttu-id="4fe14-168">Herdada da [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="4fe14-168">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="4fe14-169">deviceModel</span><span class="sxs-lookup"><span data-stu-id="4fe14-169">deviceModel</span></span>|<span data-ttu-id="4fe14-170">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="4fe14-170">String</span></span>|<span data-ttu-id="4fe14-171">O modelo de dispositivo para o registro de aplicativo atual herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="4fe14-171">The device model for the current app registration  Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="4fe14-172">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="4fe14-172">deviceManufacturer</span></span>|<span data-ttu-id="4fe14-173">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="4fe14-173">String</span></span>|<span data-ttu-id="4fe14-174">O fabricante do dispositivo para o registro de aplicativo atual herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="4fe14-174">The device manufacturer for the current app registration  Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="4fe14-175">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="4fe14-175">flaggedReasons</span></span>|<span data-ttu-id="4fe14-176">coleção [managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)</span><span class="sxs-lookup"><span data-stu-id="4fe14-176">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="4fe14-177">Zero ou mais motivos para a sinalização de um registro de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4fe14-177">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="4fe14-178">E.g.</span><span class="sxs-lookup"><span data-stu-id="4fe14-178">E.g.</span></span> <span data-ttu-id="4fe14-179">aplicativo em execução no dispositivo raiz herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="4fe14-179">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span></span> <span data-ttu-id="4fe14-180">Os valores possíveis são: `none`, `rootedDevice`, `androidBootloaderUnlocked`, `androidFactoryRomModified`.</span><span class="sxs-lookup"><span data-stu-id="4fe14-180">Possible values are: `none`, `rootedDevice`, `androidBootloaderUnlocked`, `androidFactoryRomModified`.</span></span>|
|<span data-ttu-id="4fe14-181">userId</span><span class="sxs-lookup"><span data-stu-id="4fe14-181">userId</span></span>|<span data-ttu-id="4fe14-182">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4fe14-182">String</span></span>|<span data-ttu-id="4fe14-183">A ID de usuário à qual este registro de aplicativo pertence.</span><span class="sxs-lookup"><span data-stu-id="4fe14-183">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="4fe14-184">Herdada da [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="4fe14-184">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="4fe14-185">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="4fe14-185">appIdentifier</span></span>|[<span data-ttu-id="4fe14-186">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="4fe14-186">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="4fe14-187">O Identificador de pacote do aplicativo. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="4fe14-187">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="4fe14-188">id</span><span class="sxs-lookup"><span data-stu-id="4fe14-188">id</span></span>|<span data-ttu-id="4fe14-189">String</span><span class="sxs-lookup"><span data-stu-id="4fe14-189">String</span></span>|<span data-ttu-id="4fe14-190">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4fe14-190">Key of the entity.</span></span> <span data-ttu-id="4fe14-191">Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="4fe14-191">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="4fe14-192">version</span><span class="sxs-lookup"><span data-stu-id="4fe14-192">version</span></span>|<span data-ttu-id="4fe14-193">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="4fe14-193">String</span></span>|<span data-ttu-id="4fe14-194">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="4fe14-194">Version of the entity.</span></span> <span data-ttu-id="4fe14-195">Herdada da [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="4fe14-195">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="4fe14-196">patchVersion</span><span class="sxs-lookup"><span data-stu-id="4fe14-196">patchVersion</span></span>|<span data-ttu-id="4fe14-197">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="4fe14-197">String</span></span>|<span data-ttu-id="4fe14-198">A versão do patch para o registro atual do aplicativo Android</span><span class="sxs-lookup"><span data-stu-id="4fe14-198">The patch version for the current android app registration</span></span>|



## <a name="response"></a><span data-ttu-id="4fe14-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="4fe14-199">Response</span></span>
<span data-ttu-id="4fe14-200">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4fe14-200">If successful, this method returns a `201 Created` response code and a [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4fe14-201">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4fe14-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="4fe14-202">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4fe14-202">Request</span></span>
<span data-ttu-id="4fe14-203">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4fe14-203">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations
Content-type: application/json
Content-length: 879

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
  "version": "Version value",
  "patchVersion": "Patch Version value"
}
```

### <a name="response"></a><span data-ttu-id="4fe14-204">Resposta</span><span class="sxs-lookup"><span data-stu-id="4fe14-204">Response</span></span>
<span data-ttu-id="4fe14-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4fe14-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 987

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
  "version": "Version value",
  "patchVersion": "Patch Version value"
}
```





