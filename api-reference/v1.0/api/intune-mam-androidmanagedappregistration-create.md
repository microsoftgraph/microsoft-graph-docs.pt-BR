---
title: Criar androidManagedAppRegistration
description: Cria um novo objeto androidManagedAppRegistration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2f6f1882d83a5dd0e994e0462521941cd31ed0ab
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015964"
---
# <a name="create-androidmanagedappregistration"></a><span data-ttu-id="122e8-103">Criar androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="122e8-103">Create androidManagedAppRegistration</span></span>

<span data-ttu-id="122e8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="122e8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="122e8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="122e8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="122e8-106">Cria um novo objeto [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="122e8-106">Create a new [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="122e8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="122e8-107">Prerequisites</span></span>
<span data-ttu-id="122e8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="122e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="122e8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="122e8-110">Permission type</span></span>|<span data-ttu-id="122e8-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="122e8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="122e8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="122e8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="122e8-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="122e8-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="122e8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="122e8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="122e8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="122e8-115">Not supported.</span></span>|
|<span data-ttu-id="122e8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="122e8-116">Application</span></span>|<span data-ttu-id="122e8-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="122e8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="122e8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="122e8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="122e8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="122e8-119">Request headers</span></span>
|<span data-ttu-id="122e8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="122e8-120">Header</span></span>|<span data-ttu-id="122e8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="122e8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="122e8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="122e8-122">Authorization</span></span>|<span data-ttu-id="122e8-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="122e8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="122e8-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="122e8-124">Accept</span></span>|<span data-ttu-id="122e8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="122e8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="122e8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="122e8-126">Request body</span></span>
<span data-ttu-id="122e8-127">No corpo da solicitação, forneça uma representação JSON do objeto androidManagedAppRegistration.</span><span class="sxs-lookup"><span data-stu-id="122e8-127">In the request body, supply a JSON representation for the androidManagedAppRegistration object.</span></span>

<span data-ttu-id="122e8-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidManagedAppRegistration.</span><span class="sxs-lookup"><span data-stu-id="122e8-128">The following table shows the properties that are required when you create the androidManagedAppRegistration.</span></span>

|<span data-ttu-id="122e8-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="122e8-129">Property</span></span>|<span data-ttu-id="122e8-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="122e8-130">Type</span></span>|<span data-ttu-id="122e8-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="122e8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="122e8-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="122e8-132">createdDateTime</span></span>|<span data-ttu-id="122e8-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="122e8-133">DateTimeOffset</span></span>|<span data-ttu-id="122e8-134">Data e hora de criação. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="122e8-134">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="122e8-135">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="122e8-135">lastSyncDateTime</span></span>|<span data-ttu-id="122e8-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="122e8-136">DateTimeOffset</span></span>|<span data-ttu-id="122e8-137">Data e hora em que o último aplicativo foi sincronizado com o serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="122e8-137">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="122e8-138">Herdada da [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="122e8-138">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="122e8-139">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="122e8-139">applicationVersion</span></span>|<span data-ttu-id="122e8-140">String</span><span class="sxs-lookup"><span data-stu-id="122e8-140">String</span></span>|<span data-ttu-id="122e8-141">Versão do aplicativo. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="122e8-141">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="122e8-142">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="122e8-142">managementSdkVersion</span></span>|<span data-ttu-id="122e8-143">String</span><span class="sxs-lookup"><span data-stu-id="122e8-143">String</span></span>|<span data-ttu-id="122e8-144">Versão do SDK do gerenciamento de aplicativos. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="122e8-144">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="122e8-145">platformVersion</span><span class="sxs-lookup"><span data-stu-id="122e8-145">platformVersion</span></span>|<span data-ttu-id="122e8-146">String</span><span class="sxs-lookup"><span data-stu-id="122e8-146">String</span></span>|<span data-ttu-id="122e8-147">Versão do sistema operacional. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="122e8-147">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="122e8-148">deviceType</span><span class="sxs-lookup"><span data-stu-id="122e8-148">deviceType</span></span>|<span data-ttu-id="122e8-149">String</span><span class="sxs-lookup"><span data-stu-id="122e8-149">String</span></span>|<span data-ttu-id="122e8-150">Tipo de dispositivo do host. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="122e8-150">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="122e8-151">deviceTag</span><span class="sxs-lookup"><span data-stu-id="122e8-151">deviceTag</span></span>|<span data-ttu-id="122e8-152">String</span><span class="sxs-lookup"><span data-stu-id="122e8-152">String</span></span>|<span data-ttu-id="122e8-153">Uma tag gerada pelo SDK de gerenciamento, que ajuda a relacionar aplicativos hospedados no mesmo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="122e8-153">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="122e8-154">Sem garantia de indicar aplicativos em todas as condições.</span><span class="sxs-lookup"><span data-stu-id="122e8-154">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="122e8-155">Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="122e8-155">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="122e8-156">deviceName</span><span class="sxs-lookup"><span data-stu-id="122e8-156">deviceName</span></span>|<span data-ttu-id="122e8-157">String</span><span class="sxs-lookup"><span data-stu-id="122e8-157">String</span></span>|<span data-ttu-id="122e8-158">Nome de dispositivo do host. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="122e8-158">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="122e8-159">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="122e8-159">flaggedReasons</span></span>|<span data-ttu-id="122e8-160">coleção [managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)</span><span class="sxs-lookup"><span data-stu-id="122e8-160">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="122e8-161">Zero ou mais motivos para a sinalização de um registro de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="122e8-161">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="122e8-162">E.g.</span><span class="sxs-lookup"><span data-stu-id="122e8-162">E.g.</span></span> <span data-ttu-id="122e8-163">aplicativo em execução no dispositivo raiz herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="122e8-163">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span></span> <span data-ttu-id="122e8-164">Os valores possíveis são: `none` e `rootedDevice`.</span><span class="sxs-lookup"><span data-stu-id="122e8-164">Possible values are: `none`, `rootedDevice`.</span></span>|
|<span data-ttu-id="122e8-165">userId</span><span class="sxs-lookup"><span data-stu-id="122e8-165">userId</span></span>|<span data-ttu-id="122e8-166">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="122e8-166">String</span></span>|<span data-ttu-id="122e8-167">A ID de usuário à qual este registro de aplicativo pertence.</span><span class="sxs-lookup"><span data-stu-id="122e8-167">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="122e8-168">Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="122e8-168">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="122e8-169">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="122e8-169">appIdentifier</span></span>|[<span data-ttu-id="122e8-170">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="122e8-170">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="122e8-171">O Identificador de pacote do aplicativo. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="122e8-171">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="122e8-172">id</span><span class="sxs-lookup"><span data-stu-id="122e8-172">id</span></span>|<span data-ttu-id="122e8-173">String</span><span class="sxs-lookup"><span data-stu-id="122e8-173">String</span></span>|<span data-ttu-id="122e8-174">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="122e8-174">Key of the entity.</span></span> <span data-ttu-id="122e8-175">Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="122e8-175">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="122e8-176">version</span><span class="sxs-lookup"><span data-stu-id="122e8-176">version</span></span>|<span data-ttu-id="122e8-177">String</span><span class="sxs-lookup"><span data-stu-id="122e8-177">String</span></span>|<span data-ttu-id="122e8-178">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="122e8-178">Version of the entity.</span></span> <span data-ttu-id="122e8-179">Herdada da [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="122e8-179">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="122e8-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="122e8-180">Response</span></span>
<span data-ttu-id="122e8-181">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="122e8-181">If successful, this method returns a `201 Created` response code and a [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="122e8-182">Exemplo</span><span class="sxs-lookup"><span data-stu-id="122e8-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="122e8-183">Solicitação</span><span class="sxs-lookup"><span data-stu-id="122e8-183">Request</span></span>
<span data-ttu-id="122e8-184">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="122e8-184">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="122e8-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="122e8-185">Response</span></span>
<span data-ttu-id="122e8-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="122e8-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









