---
title: Criar androidManagedAppRegistration
description: Cria um novo objeto androidManagedAppRegistration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4b4b2db4b6b725caddf5323450a993aff685af8e
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52745440"
---
# <a name="create-androidmanagedappregistration"></a><span data-ttu-id="d23ad-103">Criar androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="d23ad-103">Create androidManagedAppRegistration</span></span>

<span data-ttu-id="d23ad-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d23ad-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d23ad-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d23ad-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d23ad-106">Cria um novo objeto [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="d23ad-106">Create a new [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d23ad-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d23ad-107">Prerequisites</span></span>
<span data-ttu-id="d23ad-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d23ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d23ad-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d23ad-110">Permission type</span></span>|<span data-ttu-id="d23ad-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d23ad-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d23ad-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d23ad-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d23ad-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d23ad-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d23ad-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d23ad-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d23ad-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d23ad-115">Not supported.</span></span>|
|<span data-ttu-id="d23ad-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d23ad-116">Application</span></span>|<span data-ttu-id="d23ad-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d23ad-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d23ad-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d23ad-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="d23ad-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d23ad-119">Request headers</span></span>
|<span data-ttu-id="d23ad-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d23ad-120">Header</span></span>|<span data-ttu-id="d23ad-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d23ad-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d23ad-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d23ad-122">Authorization</span></span>|<span data-ttu-id="d23ad-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d23ad-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d23ad-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d23ad-124">Accept</span></span>|<span data-ttu-id="d23ad-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d23ad-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d23ad-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d23ad-126">Request body</span></span>
<span data-ttu-id="d23ad-127">No corpo da solicitação, forneça uma representação JSON do objeto androidManagedAppRegistration.</span><span class="sxs-lookup"><span data-stu-id="d23ad-127">In the request body, supply a JSON representation for the androidManagedAppRegistration object.</span></span>

<span data-ttu-id="d23ad-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidManagedAppRegistration.</span><span class="sxs-lookup"><span data-stu-id="d23ad-128">The following table shows the properties that are required when you create the androidManagedAppRegistration.</span></span>

|<span data-ttu-id="d23ad-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d23ad-129">Property</span></span>|<span data-ttu-id="d23ad-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d23ad-130">Type</span></span>|<span data-ttu-id="d23ad-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d23ad-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d23ad-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d23ad-132">createdDateTime</span></span>|<span data-ttu-id="d23ad-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d23ad-133">DateTimeOffset</span></span>|<span data-ttu-id="d23ad-134">Data e hora de criação. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d23ad-134">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d23ad-135">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d23ad-135">lastSyncDateTime</span></span>|<span data-ttu-id="d23ad-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d23ad-136">DateTimeOffset</span></span>|<span data-ttu-id="d23ad-137">Data e hora em que o último aplicativo foi sincronizado com o serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="d23ad-137">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="d23ad-138">Herdada da [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d23ad-138">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d23ad-139">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="d23ad-139">applicationVersion</span></span>|<span data-ttu-id="d23ad-140">String</span><span class="sxs-lookup"><span data-stu-id="d23ad-140">String</span></span>|<span data-ttu-id="d23ad-141">Versão do aplicativo. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d23ad-141">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d23ad-142">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="d23ad-142">managementSdkVersion</span></span>|<span data-ttu-id="d23ad-143">String</span><span class="sxs-lookup"><span data-stu-id="d23ad-143">String</span></span>|<span data-ttu-id="d23ad-144">Versão do SDK do gerenciamento de aplicativos. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d23ad-144">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d23ad-145">platformVersion</span><span class="sxs-lookup"><span data-stu-id="d23ad-145">platformVersion</span></span>|<span data-ttu-id="d23ad-146">String</span><span class="sxs-lookup"><span data-stu-id="d23ad-146">String</span></span>|<span data-ttu-id="d23ad-147">Versão do sistema operacional. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d23ad-147">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d23ad-148">deviceType</span><span class="sxs-lookup"><span data-stu-id="d23ad-148">deviceType</span></span>|<span data-ttu-id="d23ad-149">String</span><span class="sxs-lookup"><span data-stu-id="d23ad-149">String</span></span>|<span data-ttu-id="d23ad-150">Tipo de dispositivo do host. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d23ad-150">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d23ad-151">deviceTag</span><span class="sxs-lookup"><span data-stu-id="d23ad-151">deviceTag</span></span>|<span data-ttu-id="d23ad-152">String</span><span class="sxs-lookup"><span data-stu-id="d23ad-152">String</span></span>|<span data-ttu-id="d23ad-153">Uma tag gerada pelo SDK de gerenciamento, que ajuda a relacionar aplicativos hospedados no mesmo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d23ad-153">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="d23ad-154">Sem garantia de indicar aplicativos em todas as condições.</span><span class="sxs-lookup"><span data-stu-id="d23ad-154">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="d23ad-155">Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d23ad-155">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d23ad-156">deviceName</span><span class="sxs-lookup"><span data-stu-id="d23ad-156">deviceName</span></span>|<span data-ttu-id="d23ad-157">String</span><span class="sxs-lookup"><span data-stu-id="d23ad-157">String</span></span>|<span data-ttu-id="d23ad-158">Nome de dispositivo do host. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d23ad-158">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d23ad-159">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="d23ad-159">flaggedReasons</span></span>|<span data-ttu-id="d23ad-160">[Coleção managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)</span><span class="sxs-lookup"><span data-stu-id="d23ad-160">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="d23ad-161">Zero ou mais motivos para a sinalização de um registro de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d23ad-161">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="d23ad-162">E.g.</span><span class="sxs-lookup"><span data-stu-id="d23ad-162">E.g.</span></span> <span data-ttu-id="d23ad-163">aplicativo em execução no dispositivo raiz Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="d23ad-163">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span></span> <span data-ttu-id="d23ad-164">Os valores possíveis são: `none` e `rootedDevice`.</span><span class="sxs-lookup"><span data-stu-id="d23ad-164">Possible values are: `none`, `rootedDevice`.</span></span>|
|<span data-ttu-id="d23ad-165">userId</span><span class="sxs-lookup"><span data-stu-id="d23ad-165">userId</span></span>|<span data-ttu-id="d23ad-166">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d23ad-166">String</span></span>|<span data-ttu-id="d23ad-167">A ID de usuário à qual este registro de aplicativo pertence.</span><span class="sxs-lookup"><span data-stu-id="d23ad-167">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="d23ad-168">Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d23ad-168">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d23ad-169">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="d23ad-169">appIdentifier</span></span>|[<span data-ttu-id="d23ad-170">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="d23ad-170">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="d23ad-171">O Identificador de pacote do aplicativo. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d23ad-171">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d23ad-172">id</span><span class="sxs-lookup"><span data-stu-id="d23ad-172">id</span></span>|<span data-ttu-id="d23ad-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d23ad-173">String</span></span>|<span data-ttu-id="d23ad-174">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d23ad-174">Key of the entity.</span></span> <span data-ttu-id="d23ad-175">Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d23ad-175">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d23ad-176">version</span><span class="sxs-lookup"><span data-stu-id="d23ad-176">version</span></span>|<span data-ttu-id="d23ad-177">String</span><span class="sxs-lookup"><span data-stu-id="d23ad-177">String</span></span>|<span data-ttu-id="d23ad-178">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="d23ad-178">Version of the entity.</span></span> <span data-ttu-id="d23ad-179">Herdada da [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d23ad-179">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="d23ad-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="d23ad-180">Response</span></span>
<span data-ttu-id="d23ad-181">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d23ad-181">If successful, this method returns a `201 Created` response code and a [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d23ad-182">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d23ad-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="d23ad-183">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d23ad-183">Request</span></span>
<span data-ttu-id="d23ad-184">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d23ad-184">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d23ad-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="d23ad-185">Response</span></span>
<span data-ttu-id="d23ad-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d23ad-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




