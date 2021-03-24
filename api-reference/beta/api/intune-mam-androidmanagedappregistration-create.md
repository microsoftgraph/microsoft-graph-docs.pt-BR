---
title: Criar androidManagedAppRegistration
description: Cria um novo objeto androidManagedAppRegistration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d3c0b4901db4ee277b4f2470bc62aaffd00bbea3
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145527"
---
# <a name="create-androidmanagedappregistration"></a><span data-ttu-id="092f8-103">Criar androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="092f8-103">Create androidManagedAppRegistration</span></span>

<span data-ttu-id="092f8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="092f8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="092f8-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="092f8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="092f8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="092f8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="092f8-107">Cria um novo objeto [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="092f8-107">Create a new [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="092f8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="092f8-108">Prerequisites</span></span>
<span data-ttu-id="092f8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="092f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="092f8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="092f8-111">Permission type</span></span>|<span data-ttu-id="092f8-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="092f8-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="092f8-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="092f8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="092f8-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="092f8-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="092f8-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="092f8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="092f8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="092f8-116">Not supported.</span></span>|
|<span data-ttu-id="092f8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="092f8-117">Application</span></span>|<span data-ttu-id="092f8-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="092f8-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="092f8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="092f8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="092f8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="092f8-120">Request headers</span></span>
|<span data-ttu-id="092f8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="092f8-121">Header</span></span>|<span data-ttu-id="092f8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="092f8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="092f8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="092f8-123">Authorization</span></span>|<span data-ttu-id="092f8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="092f8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="092f8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="092f8-125">Accept</span></span>|<span data-ttu-id="092f8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="092f8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="092f8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="092f8-127">Request body</span></span>
<span data-ttu-id="092f8-128">No corpo da solicitação, forneça uma representação JSON do objeto androidManagedAppRegistration.</span><span class="sxs-lookup"><span data-stu-id="092f8-128">In the request body, supply a JSON representation for the androidManagedAppRegistration object.</span></span>

<span data-ttu-id="092f8-129">A tabela a seguir mostra as propriedades que são necessárias ao criar androidManagedAppRegistration.</span><span class="sxs-lookup"><span data-stu-id="092f8-129">The following table shows the properties that are required when you create the androidManagedAppRegistration.</span></span>

|<span data-ttu-id="092f8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="092f8-130">Property</span></span>|<span data-ttu-id="092f8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="092f8-131">Type</span></span>|<span data-ttu-id="092f8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="092f8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="092f8-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="092f8-133">createdDateTime</span></span>|<span data-ttu-id="092f8-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="092f8-134">DateTimeOffset</span></span>|<span data-ttu-id="092f8-135">Data e hora de criação. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="092f8-135">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="092f8-136">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="092f8-136">lastSyncDateTime</span></span>|<span data-ttu-id="092f8-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="092f8-137">DateTimeOffset</span></span>|<span data-ttu-id="092f8-138">Data e hora em que o último aplicativo foi sincronizado com o serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="092f8-138">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="092f8-139">Herdada da [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="092f8-139">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="092f8-140">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="092f8-140">applicationVersion</span></span>|<span data-ttu-id="092f8-141">String</span><span class="sxs-lookup"><span data-stu-id="092f8-141">String</span></span>|<span data-ttu-id="092f8-142">Versão do aplicativo. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="092f8-142">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="092f8-143">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="092f8-143">managementSdkVersion</span></span>|<span data-ttu-id="092f8-144">String</span><span class="sxs-lookup"><span data-stu-id="092f8-144">String</span></span>|<span data-ttu-id="092f8-145">Versão do SDK do gerenciamento de aplicativos. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="092f8-145">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="092f8-146">platformVersion</span><span class="sxs-lookup"><span data-stu-id="092f8-146">platformVersion</span></span>|<span data-ttu-id="092f8-147">String</span><span class="sxs-lookup"><span data-stu-id="092f8-147">String</span></span>|<span data-ttu-id="092f8-148">Versão do sistema operacional. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="092f8-148">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="092f8-149">deviceType</span><span class="sxs-lookup"><span data-stu-id="092f8-149">deviceType</span></span>|<span data-ttu-id="092f8-150">String</span><span class="sxs-lookup"><span data-stu-id="092f8-150">String</span></span>|<span data-ttu-id="092f8-151">Tipo de dispositivo do host. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="092f8-151">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="092f8-152">deviceTag</span><span class="sxs-lookup"><span data-stu-id="092f8-152">deviceTag</span></span>|<span data-ttu-id="092f8-153">String</span><span class="sxs-lookup"><span data-stu-id="092f8-153">String</span></span>|<span data-ttu-id="092f8-154">Uma tag gerada pelo SDK de gerenciamento, que ajuda a relacionar aplicativos hospedados no mesmo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="092f8-154">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="092f8-155">Sem garantia de indicar aplicativos em todas as condições.</span><span class="sxs-lookup"><span data-stu-id="092f8-155">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="092f8-156">Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="092f8-156">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="092f8-157">deviceName</span><span class="sxs-lookup"><span data-stu-id="092f8-157">deviceName</span></span>|<span data-ttu-id="092f8-158">String</span><span class="sxs-lookup"><span data-stu-id="092f8-158">String</span></span>|<span data-ttu-id="092f8-159">Nome de dispositivo do host. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="092f8-159">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="092f8-160">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="092f8-160">managedDeviceId</span></span>|<span data-ttu-id="092f8-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="092f8-161">String</span></span>|<span data-ttu-id="092f8-162">O identificador de Dispositivo Gerenciado do dispositivo host.</span><span class="sxs-lookup"><span data-stu-id="092f8-162">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="092f8-163">O valor pode estar vazio mesmo quando o dispositivo host é gerenciado.</span><span class="sxs-lookup"><span data-stu-id="092f8-163">Value could be empty even when the host device is managed.</span></span> <span data-ttu-id="092f8-164">Herdada da [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="092f8-164">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="092f8-165">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="092f8-165">azureADDeviceId</span></span>|<span data-ttu-id="092f8-166">String</span><span class="sxs-lookup"><span data-stu-id="092f8-166">String</span></span>|<span data-ttu-id="092f8-167">O identificador do Dispositivo do Azure Active Directory do dispositivo host.</span><span class="sxs-lookup"><span data-stu-id="092f8-167">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="092f8-168">O valor pode estar vazio mesmo quando o dispositivo host é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="092f8-168">Value could be empty even when the host device is Azure Active Directory registered.</span></span> <span data-ttu-id="092f8-169">Herdada da [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="092f8-169">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="092f8-170">deviceModel</span><span class="sxs-lookup"><span data-stu-id="092f8-170">deviceModel</span></span>|<span data-ttu-id="092f8-171">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="092f8-171">String</span></span>|<span data-ttu-id="092f8-172">O modelo de dispositivo para o registro de aplicativo atual Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="092f8-172">The device model for the current app registration  Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="092f8-173">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="092f8-173">deviceManufacturer</span></span>|<span data-ttu-id="092f8-174">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="092f8-174">String</span></span>|<span data-ttu-id="092f8-175">O fabricante do dispositivo para o registro de aplicativo atual Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="092f8-175">The device manufacturer for the current app registration  Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="092f8-176">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="092f8-176">flaggedReasons</span></span>|<span data-ttu-id="092f8-177">[Coleção managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)</span><span class="sxs-lookup"><span data-stu-id="092f8-177">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="092f8-178">Zero ou mais motivos para a sinalização de um registro de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="092f8-178">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="092f8-179">E.g.</span><span class="sxs-lookup"><span data-stu-id="092f8-179">E.g.</span></span> <span data-ttu-id="092f8-180">aplicativo em execução no dispositivo raiz Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="092f8-180">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span></span> <span data-ttu-id="092f8-181">Os valores possíveis são: `none`, `rootedDevice`, `androidBootloaderUnlocked`, `androidFactoryRomModified`.</span><span class="sxs-lookup"><span data-stu-id="092f8-181">Possible values are: `none`, `rootedDevice`, `androidBootloaderUnlocked`, `androidFactoryRomModified`.</span></span>|
|<span data-ttu-id="092f8-182">userId</span><span class="sxs-lookup"><span data-stu-id="092f8-182">userId</span></span>|<span data-ttu-id="092f8-183">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="092f8-183">String</span></span>|<span data-ttu-id="092f8-184">A ID de usuário à qual este registro de aplicativo pertence.</span><span class="sxs-lookup"><span data-stu-id="092f8-184">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="092f8-185">Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="092f8-185">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="092f8-186">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="092f8-186">appIdentifier</span></span>|[<span data-ttu-id="092f8-187">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="092f8-187">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="092f8-188">O Identificador de pacote do aplicativo. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="092f8-188">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="092f8-189">id</span><span class="sxs-lookup"><span data-stu-id="092f8-189">id</span></span>|<span data-ttu-id="092f8-190">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="092f8-190">String</span></span>|<span data-ttu-id="092f8-191">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="092f8-191">Key of the entity.</span></span> <span data-ttu-id="092f8-192">Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="092f8-192">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="092f8-193">version</span><span class="sxs-lookup"><span data-stu-id="092f8-193">version</span></span>|<span data-ttu-id="092f8-194">String</span><span class="sxs-lookup"><span data-stu-id="092f8-194">String</span></span>|<span data-ttu-id="092f8-195">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="092f8-195">Version of the entity.</span></span> <span data-ttu-id="092f8-196">Herdada da [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="092f8-196">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="092f8-197">patchVersion</span><span class="sxs-lookup"><span data-stu-id="092f8-197">patchVersion</span></span>|<span data-ttu-id="092f8-198">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="092f8-198">String</span></span>|<span data-ttu-id="092f8-199">A versão de patch para o registro atual do aplicativo android</span><span class="sxs-lookup"><span data-stu-id="092f8-199">The patch version for the current android app registration</span></span>|



## <a name="response"></a><span data-ttu-id="092f8-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="092f8-200">Response</span></span>
<span data-ttu-id="092f8-201">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="092f8-201">If successful, this method returns a `201 Created` response code and a [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="092f8-202">Exemplo</span><span class="sxs-lookup"><span data-stu-id="092f8-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="092f8-203">Solicitação</span><span class="sxs-lookup"><span data-stu-id="092f8-203">Request</span></span>
<span data-ttu-id="092f8-204">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="092f8-204">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="092f8-205">Resposta</span><span class="sxs-lookup"><span data-stu-id="092f8-205">Response</span></span>
<span data-ttu-id="092f8-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="092f8-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




