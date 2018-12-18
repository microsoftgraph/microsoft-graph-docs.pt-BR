---
title: Criar androidManagedAppRegistration
description: Cria um novo objeto androidManagedAppRegistration.
author: tfitzmac
ms.openlocfilehash: c05c698179f2f8fa54ab12282be6e397b9275408
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339505"
---
# <a name="create-androidmanagedappregistration"></a><span data-ttu-id="4ed2e-103">Criar androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="4ed2e-103">Create androidManagedAppRegistration</span></span>

> <span data-ttu-id="4ed2e-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4ed2e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4ed2e-105">Cria um novo objeto [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="4ed2e-105">Create a new [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4ed2e-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4ed2e-106">Prerequisites</span></span>
<span data-ttu-id="4ed2e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ed2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ed2e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4ed2e-109">Permission type</span></span>|<span data-ttu-id="4ed2e-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4ed2e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ed2e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4ed2e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4ed2e-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ed2e-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4ed2e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4ed2e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ed2e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ed2e-114">Not supported.</span></span>|
|<span data-ttu-id="4ed2e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4ed2e-115">Application</span></span>|<span data-ttu-id="4ed2e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ed2e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ed2e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4ed2e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="4ed2e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4ed2e-118">Request headers</span></span>
|<span data-ttu-id="4ed2e-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4ed2e-119">Header</span></span>|<span data-ttu-id="4ed2e-120">Valor</span><span class="sxs-lookup"><span data-stu-id="4ed2e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ed2e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4ed2e-121">Authorization</span></span>|<span data-ttu-id="4ed2e-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4ed2e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ed2e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="4ed2e-123">Accept</span></span>|<span data-ttu-id="4ed2e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4ed2e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ed2e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4ed2e-125">Request body</span></span>
<span data-ttu-id="4ed2e-126">No corpo da solicitação, forneça uma representação JSON do objeto androidManagedAppRegistration.</span><span class="sxs-lookup"><span data-stu-id="4ed2e-126">In the request body, supply a JSON representation for the androidManagedAppRegistration object.</span></span>

<span data-ttu-id="4ed2e-127">A tabela a seguir mostra as propriedades que são necessárias ao criar androidManagedAppRegistration.</span><span class="sxs-lookup"><span data-stu-id="4ed2e-127">The following table shows the properties that are required when you create the androidManagedAppRegistration.</span></span>

|<span data-ttu-id="4ed2e-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4ed2e-128">Property</span></span>|<span data-ttu-id="4ed2e-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="4ed2e-129">Type</span></span>|<span data-ttu-id="4ed2e-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ed2e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ed2e-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4ed2e-131">createdDateTime</span></span>|<span data-ttu-id="4ed2e-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ed2e-132">DateTimeOffset</span></span>|<span data-ttu-id="4ed2e-133">Data e hora de criação. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="4ed2e-133">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="4ed2e-134">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="4ed2e-134">lastSyncDateTime</span></span>|<span data-ttu-id="4ed2e-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ed2e-135">DateTimeOffset</span></span>|<span data-ttu-id="4ed2e-136">Data e hora em que o último aplicativo foi sincronizado com o serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="4ed2e-136">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="4ed2e-137">Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="4ed2e-137">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="4ed2e-138">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="4ed2e-138">applicationVersion</span></span>|<span data-ttu-id="4ed2e-139">String</span><span class="sxs-lookup"><span data-stu-id="4ed2e-139">String</span></span>|<span data-ttu-id="4ed2e-140">Versão do aplicativo. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="4ed2e-140">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="4ed2e-141">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="4ed2e-141">managementSdkVersion</span></span>|<span data-ttu-id="4ed2e-142">String</span><span class="sxs-lookup"><span data-stu-id="4ed2e-142">String</span></span>|<span data-ttu-id="4ed2e-143">Versão do SDK do gerenciamento de aplicativos. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="4ed2e-143">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="4ed2e-144">platformVersion</span><span class="sxs-lookup"><span data-stu-id="4ed2e-144">platformVersion</span></span>|<span data-ttu-id="4ed2e-145">String</span><span class="sxs-lookup"><span data-stu-id="4ed2e-145">String</span></span>|<span data-ttu-id="4ed2e-146">Versão do sistema operacional. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="4ed2e-146">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="4ed2e-147">deviceType</span><span class="sxs-lookup"><span data-stu-id="4ed2e-147">deviceType</span></span>|<span data-ttu-id="4ed2e-148">String</span><span class="sxs-lookup"><span data-stu-id="4ed2e-148">String</span></span>|<span data-ttu-id="4ed2e-149">Tipo de dispositivo do host. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="4ed2e-149">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="4ed2e-150">deviceTag</span><span class="sxs-lookup"><span data-stu-id="4ed2e-150">deviceTag</span></span>|<span data-ttu-id="4ed2e-151">String</span><span class="sxs-lookup"><span data-stu-id="4ed2e-151">String</span></span>|<span data-ttu-id="4ed2e-152">Uma tag gerada pelo SDK de gerenciamento, que ajuda a relacionar aplicativos hospedados no mesmo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4ed2e-152">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="4ed2e-153">Sem garantia de indicar aplicativos em todas as condições.</span><span class="sxs-lookup"><span data-stu-id="4ed2e-153">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="4ed2e-154">Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="4ed2e-154">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="4ed2e-155">deviceName</span><span class="sxs-lookup"><span data-stu-id="4ed2e-155">deviceName</span></span>|<span data-ttu-id="4ed2e-156">String</span><span class="sxs-lookup"><span data-stu-id="4ed2e-156">String</span></span>|<span data-ttu-id="4ed2e-157">Nome de dispositivo do host. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="4ed2e-157">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="4ed2e-158">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="4ed2e-158">flaggedReasons</span></span>|<span data-ttu-id="4ed2e-159">coleção [managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)</span><span class="sxs-lookup"><span data-stu-id="4ed2e-159">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="4ed2e-160">Zero ou mais motivos para a sinalização de um registro de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4ed2e-160">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="4ed2e-161">E.g.</span><span class="sxs-lookup"><span data-stu-id="4ed2e-161">E.g.</span></span> <span data-ttu-id="4ed2e-162">aplicativo em execução no dispositivo com raiz Inherited de [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="4ed2e-162">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span></span> <span data-ttu-id="4ed2e-163">Os valores possíveis são: `none` e `rootedDevice`.</span><span class="sxs-lookup"><span data-stu-id="4ed2e-163">Possible values are: `none`, `rootedDevice`.</span></span>|
|<span data-ttu-id="4ed2e-164">userId</span><span class="sxs-lookup"><span data-stu-id="4ed2e-164">userId</span></span>|<span data-ttu-id="4ed2e-165">String</span><span class="sxs-lookup"><span data-stu-id="4ed2e-165">String</span></span>|<span data-ttu-id="4ed2e-166">A ID de usuário à qual este registro de aplicativo pertence.</span><span class="sxs-lookup"><span data-stu-id="4ed2e-166">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="4ed2e-167">Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="4ed2e-167">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="4ed2e-168">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="4ed2e-168">appIdentifier</span></span>|[<span data-ttu-id="4ed2e-169">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="4ed2e-169">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="4ed2e-170">O Identificador de pacote do aplicativo. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="4ed2e-170">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="4ed2e-171">id</span><span class="sxs-lookup"><span data-stu-id="4ed2e-171">id</span></span>|<span data-ttu-id="4ed2e-172">String</span><span class="sxs-lookup"><span data-stu-id="4ed2e-172">String</span></span>|<span data-ttu-id="4ed2e-173">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4ed2e-173">Key of the entity.</span></span> <span data-ttu-id="4ed2e-174">Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="4ed2e-174">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="4ed2e-175">version</span><span class="sxs-lookup"><span data-stu-id="4ed2e-175">version</span></span>|<span data-ttu-id="4ed2e-176">String</span><span class="sxs-lookup"><span data-stu-id="4ed2e-176">String</span></span>|<span data-ttu-id="4ed2e-177">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="4ed2e-177">Version of the entity.</span></span> <span data-ttu-id="4ed2e-178">Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="4ed2e-178">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="4ed2e-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ed2e-179">Response</span></span>
<span data-ttu-id="4ed2e-180">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4ed2e-180">If successful, this method returns a `201 Created` response code and a [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ed2e-181">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4ed2e-181">Example</span></span>
### <a name="request"></a><span data-ttu-id="4ed2e-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4ed2e-182">Request</span></span>
<span data-ttu-id="4ed2e-183">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4ed2e-183">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations
Content-type: application/json
Content-length: 645

{
  "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "applicationVersion": "Application Version value",
  "managementSdkVersion": "Management Sdk Version value",
  "platformVersion": "Platform Version value",
  "deviceType": "Device Type value",
  "deviceTag": "Device Tag value",
  "deviceName": "Device Name value",
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

### <a name="response"></a><span data-ttu-id="4ed2e-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ed2e-184">Response</span></span>
<span data-ttu-id="4ed2e-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4ed2e-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 753

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



