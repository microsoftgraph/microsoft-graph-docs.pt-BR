---
title: Criar androidManagedAppRegistration
description: Cria um novo objeto androidManagedAppRegistration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 84fc753a055e64549b0042d24acedf83827271df
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841550"
---
# <a name="create-androidmanagedappregistration"></a><span data-ttu-id="050da-103">Criar androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="050da-103">Create androidManagedAppRegistration</span></span>

> <span data-ttu-id="050da-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="050da-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="050da-105">Cria um novo objeto [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="050da-105">Create a new [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="050da-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="050da-106">Prerequisites</span></span>
<span data-ttu-id="050da-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="050da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="050da-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="050da-109">Permission type</span></span>|<span data-ttu-id="050da-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="050da-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="050da-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="050da-111">Delegated (work or school account)</span></span>|<span data-ttu-id="050da-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="050da-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="050da-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="050da-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="050da-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="050da-114">Not supported.</span></span>|
|<span data-ttu-id="050da-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="050da-115">Application</span></span>|<span data-ttu-id="050da-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="050da-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="050da-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="050da-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="050da-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="050da-118">Request headers</span></span>
|<span data-ttu-id="050da-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="050da-119">Header</span></span>|<span data-ttu-id="050da-120">Valor</span><span class="sxs-lookup"><span data-stu-id="050da-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="050da-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="050da-121">Authorization</span></span>|<span data-ttu-id="050da-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="050da-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="050da-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="050da-123">Accept</span></span>|<span data-ttu-id="050da-124">application/json</span><span class="sxs-lookup"><span data-stu-id="050da-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="050da-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="050da-125">Request body</span></span>
<span data-ttu-id="050da-126">No corpo da solicitação, forneça uma representação JSON do objeto androidManagedAppRegistration.</span><span class="sxs-lookup"><span data-stu-id="050da-126">In the request body, supply a JSON representation for the androidManagedAppRegistration object.</span></span>

<span data-ttu-id="050da-127">A tabela a seguir mostra as propriedades que são necessárias ao criar androidManagedAppRegistration.</span><span class="sxs-lookup"><span data-stu-id="050da-127">The following table shows the properties that are required when you create the androidManagedAppRegistration.</span></span>

|<span data-ttu-id="050da-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="050da-128">Property</span></span>|<span data-ttu-id="050da-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="050da-129">Type</span></span>|<span data-ttu-id="050da-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="050da-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="050da-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="050da-131">createdDateTime</span></span>|<span data-ttu-id="050da-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="050da-132">DateTimeOffset</span></span>|<span data-ttu-id="050da-133">Data e hora de criação. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="050da-133">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="050da-134">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="050da-134">lastSyncDateTime</span></span>|<span data-ttu-id="050da-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="050da-135">DateTimeOffset</span></span>|<span data-ttu-id="050da-136">Data e hora em que o último aplicativo foi sincronizado com o serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="050da-136">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="050da-137">Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="050da-137">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="050da-138">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="050da-138">applicationVersion</span></span>|<span data-ttu-id="050da-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="050da-139">String</span></span>|<span data-ttu-id="050da-140">Versão do aplicativo. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="050da-140">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="050da-141">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="050da-141">managementSdkVersion</span></span>|<span data-ttu-id="050da-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="050da-142">String</span></span>|<span data-ttu-id="050da-143">Versão do SDK do gerenciamento de aplicativos. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="050da-143">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="050da-144">platformVersion</span><span class="sxs-lookup"><span data-stu-id="050da-144">platformVersion</span></span>|<span data-ttu-id="050da-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="050da-145">String</span></span>|<span data-ttu-id="050da-146">Versão do sistema operacional. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="050da-146">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="050da-147">deviceType</span><span class="sxs-lookup"><span data-stu-id="050da-147">deviceType</span></span>|<span data-ttu-id="050da-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="050da-148">String</span></span>|<span data-ttu-id="050da-149">Tipo de dispositivo do host. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="050da-149">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="050da-150">deviceTag</span><span class="sxs-lookup"><span data-stu-id="050da-150">deviceTag</span></span>|<span data-ttu-id="050da-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="050da-151">String</span></span>|<span data-ttu-id="050da-152">Uma tag gerada pelo SDK de gerenciamento, que ajuda a relacionar aplicativos hospedados no mesmo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="050da-152">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="050da-153">Sem garantia de indicar aplicativos em todas as condições.</span><span class="sxs-lookup"><span data-stu-id="050da-153">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="050da-154">Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="050da-154">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="050da-155">deviceName</span><span class="sxs-lookup"><span data-stu-id="050da-155">deviceName</span></span>|<span data-ttu-id="050da-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="050da-156">String</span></span>|<span data-ttu-id="050da-157">Nome de dispositivo do host. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="050da-157">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="050da-158">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="050da-158">flaggedReasons</span></span>|<span data-ttu-id="050da-159">coleção [managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)</span><span class="sxs-lookup"><span data-stu-id="050da-159">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="050da-160">Zero ou mais motivos para a sinalização de um registro de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="050da-160">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="050da-161">E.g.</span><span class="sxs-lookup"><span data-stu-id="050da-161">E.g.</span></span> <span data-ttu-id="050da-162">aplicativo em execução no dispositivo com raiz Inherited de [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="050da-162">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span></span> <span data-ttu-id="050da-163">Os valores possíveis são: `none` e `rootedDevice`.</span><span class="sxs-lookup"><span data-stu-id="050da-163">Possible values are: `none`, `rootedDevice`.</span></span>|
|<span data-ttu-id="050da-164">userId</span><span class="sxs-lookup"><span data-stu-id="050da-164">userId</span></span>|<span data-ttu-id="050da-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="050da-165">String</span></span>|<span data-ttu-id="050da-166">A ID de usuário à qual este registro de aplicativo pertence.</span><span class="sxs-lookup"><span data-stu-id="050da-166">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="050da-167">Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="050da-167">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="050da-168">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="050da-168">appIdentifier</span></span>|[<span data-ttu-id="050da-169">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="050da-169">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="050da-170">O Identificador de pacote do aplicativo. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="050da-170">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="050da-171">id</span><span class="sxs-lookup"><span data-stu-id="050da-171">id</span></span>|<span data-ttu-id="050da-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="050da-172">String</span></span>|<span data-ttu-id="050da-173">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="050da-173">Key of the entity.</span></span> <span data-ttu-id="050da-174">Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="050da-174">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="050da-175">version</span><span class="sxs-lookup"><span data-stu-id="050da-175">version</span></span>|<span data-ttu-id="050da-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="050da-176">String</span></span>|<span data-ttu-id="050da-177">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="050da-177">Version of the entity.</span></span> <span data-ttu-id="050da-178">Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="050da-178">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="050da-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="050da-179">Response</span></span>
<span data-ttu-id="050da-180">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="050da-180">If successful, this method returns a `201 Created` response code and a [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="050da-181">Exemplo</span><span class="sxs-lookup"><span data-stu-id="050da-181">Example</span></span>
### <a name="request"></a><span data-ttu-id="050da-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="050da-182">Request</span></span>
<span data-ttu-id="050da-183">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="050da-183">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="050da-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="050da-184">Response</span></span>
<span data-ttu-id="050da-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="050da-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



