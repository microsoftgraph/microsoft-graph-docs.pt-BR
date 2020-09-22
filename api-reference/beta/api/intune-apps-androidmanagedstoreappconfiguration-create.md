---
title: Criar androidManagedStoreAppConfiguration
description: Criar um novo objeto androidManagedStoreAppConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 00274e76a8ef752e8030d68324df01438011c94a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48006395"
---
# <a name="create-androidmanagedstoreappconfiguration"></a><span data-ttu-id="45c9e-103">Criar androidManagedStoreAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="45c9e-103">Create androidManagedStoreAppConfiguration</span></span>

<span data-ttu-id="45c9e-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="45c9e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="45c9e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="45c9e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45c9e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="45c9e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45c9e-107">Criar um novo objeto [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="45c9e-107">Create a new [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45c9e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="45c9e-108">Prerequisites</span></span>
<span data-ttu-id="45c9e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45c9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45c9e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="45c9e-111">Permission type</span></span>|<span data-ttu-id="45c9e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="45c9e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45c9e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="45c9e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="45c9e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45c9e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="45c9e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="45c9e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45c9e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45c9e-116">Not supported.</span></span>|
|<span data-ttu-id="45c9e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="45c9e-117">Application</span></span>|<span data-ttu-id="45c9e-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45c9e-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="45c9e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="45c9e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="45c9e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="45c9e-120">Request headers</span></span>
|<span data-ttu-id="45c9e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="45c9e-121">Header</span></span>|<span data-ttu-id="45c9e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="45c9e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45c9e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="45c9e-123">Authorization</span></span>|<span data-ttu-id="45c9e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="45c9e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45c9e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="45c9e-125">Accept</span></span>|<span data-ttu-id="45c9e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="45c9e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45c9e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="45c9e-127">Request body</span></span>
<span data-ttu-id="45c9e-128">No corpo da solicitação, forneça uma representação JSON do objeto androidManagedStoreAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="45c9e-128">In the request body, supply a JSON representation for the androidManagedStoreAppConfiguration object.</span></span>

<span data-ttu-id="45c9e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar androidManagedStoreAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="45c9e-129">The following table shows the properties that are required when you create the androidManagedStoreAppConfiguration.</span></span>

|<span data-ttu-id="45c9e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="45c9e-130">Property</span></span>|<span data-ttu-id="45c9e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="45c9e-131">Type</span></span>|<span data-ttu-id="45c9e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="45c9e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45c9e-133">id</span><span class="sxs-lookup"><span data-stu-id="45c9e-133">id</span></span>|<span data-ttu-id="45c9e-134">String</span><span class="sxs-lookup"><span data-stu-id="45c9e-134">String</span></span>|<span data-ttu-id="45c9e-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="45c9e-135">Key of the entity.</span></span> <span data-ttu-id="45c9e-136">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45c9e-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="45c9e-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="45c9e-137">targetedMobileApps</span></span>|<span data-ttu-id="45c9e-138">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="45c9e-138">String collection</span></span>|<span data-ttu-id="45c9e-139">o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="45c9e-139">the associated app.</span></span> <span data-ttu-id="45c9e-140">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45c9e-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="45c9e-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="45c9e-141">roleScopeTagIds</span></span>|<span data-ttu-id="45c9e-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="45c9e-142">String collection</span></span>|<span data-ttu-id="45c9e-143">Lista de marcas de escopo para esta entidade de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="45c9e-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="45c9e-144">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45c9e-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="45c9e-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="45c9e-145">createdDateTime</span></span>|<span data-ttu-id="45c9e-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45c9e-146">DateTimeOffset</span></span>|<span data-ttu-id="45c9e-147">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="45c9e-147">DateTime the object was created.</span></span> <span data-ttu-id="45c9e-148">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45c9e-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="45c9e-149">description</span><span class="sxs-lookup"><span data-stu-id="45c9e-149">description</span></span>|<span data-ttu-id="45c9e-150">String</span><span class="sxs-lookup"><span data-stu-id="45c9e-150">String</span></span>|<span data-ttu-id="45c9e-151">Descrição fornecida pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45c9e-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="45c9e-152">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45c9e-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="45c9e-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="45c9e-153">lastModifiedDateTime</span></span>|<span data-ttu-id="45c9e-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45c9e-154">DateTimeOffset</span></span>|<span data-ttu-id="45c9e-155">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="45c9e-155">DateTime the object was last modified.</span></span> <span data-ttu-id="45c9e-156">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45c9e-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="45c9e-157">displayName</span><span class="sxs-lookup"><span data-stu-id="45c9e-157">displayName</span></span>|<span data-ttu-id="45c9e-158">String</span><span class="sxs-lookup"><span data-stu-id="45c9e-158">String</span></span>|<span data-ttu-id="45c9e-159">Nome fornecido pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45c9e-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="45c9e-160">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45c9e-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="45c9e-161">version</span><span class="sxs-lookup"><span data-stu-id="45c9e-161">version</span></span>|<span data-ttu-id="45c9e-162">Int32</span><span class="sxs-lookup"><span data-stu-id="45c9e-162">Int32</span></span>|<span data-ttu-id="45c9e-163">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45c9e-163">Version of the device configuration.</span></span> <span data-ttu-id="45c9e-164">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45c9e-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="45c9e-165">packageId</span><span class="sxs-lookup"><span data-stu-id="45c9e-165">packageId</span></span>|<span data-ttu-id="45c9e-166">String</span><span class="sxs-lookup"><span data-stu-id="45c9e-166">String</span></span>|<span data-ttu-id="45c9e-167">ID do pacote de configuração do aplicativo Enterprise Android.</span><span class="sxs-lookup"><span data-stu-id="45c9e-167">Android Enterprise app configuration package id.</span></span>|
|<span data-ttu-id="45c9e-168">payloadJson</span><span class="sxs-lookup"><span data-stu-id="45c9e-168">payloadJson</span></span>|<span data-ttu-id="45c9e-169">String</span><span class="sxs-lookup"><span data-stu-id="45c9e-169">String</span></span>|<span data-ttu-id="45c9e-170">Carga JSON da configuração do aplicativo empresarial Android.</span><span class="sxs-lookup"><span data-stu-id="45c9e-170">Android Enterprise app configuration JSON payload.</span></span>|
|<span data-ttu-id="45c9e-171">permissionActions</span><span class="sxs-lookup"><span data-stu-id="45c9e-171">permissionActions</span></span>|<span data-ttu-id="45c9e-172">coleção [androidPermissionAction](../resources/intune-apps-androidpermissionaction.md)</span><span class="sxs-lookup"><span data-stu-id="45c9e-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="45c9e-173">Lista de permissões de aplicativo Android e ações de permissão correspondentes.</span><span class="sxs-lookup"><span data-stu-id="45c9e-173">List of Android app permissions and corresponding permission actions.</span></span>|
|<span data-ttu-id="45c9e-174">appSupportsOemConfig</span><span class="sxs-lookup"><span data-stu-id="45c9e-174">appSupportsOemConfig</span></span>|<span data-ttu-id="45c9e-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="45c9e-175">Boolean</span></span>|<span data-ttu-id="45c9e-176">Se este AppConfig é ou não uma política de OEMConfig.</span><span class="sxs-lookup"><span data-stu-id="45c9e-176">Whether or not this AppConfig is an OEMConfig policy.</span></span>|
|<span data-ttu-id="45c9e-177">profileApplicability</span><span class="sxs-lookup"><span data-stu-id="45c9e-177">profileApplicability</span></span>|[<span data-ttu-id="45c9e-178">androidProfileApplicability</span><span class="sxs-lookup"><span data-stu-id="45c9e-178">androidProfileApplicability</span></span>](../resources/intune-apps-androidprofileapplicability.md)|<span data-ttu-id="45c9e-179">Aplicabilidade de perfil corporativo Android (AndroidWorkProfile, DeviceOwner ou default (aplica-se a ambos)).</span><span class="sxs-lookup"><span data-stu-id="45c9e-179">Android Enterprise profile applicability (AndroidWorkProfile, DeviceOwner, or default (applies to both)).</span></span> <span data-ttu-id="45c9e-180">Os valores possíveis são: `default`, `androidWorkProfile`, `androidDeviceOwner`.</span><span class="sxs-lookup"><span data-stu-id="45c9e-180">Possible values are: `default`, `androidWorkProfile`, `androidDeviceOwner`.</span></span>|



## <a name="response"></a><span data-ttu-id="45c9e-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="45c9e-181">Response</span></span>
<span data-ttu-id="45c9e-182">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="45c9e-182">If successful, this method returns a `201 Created` response code and a [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45c9e-183">Exemplo</span><span class="sxs-lookup"><span data-stu-id="45c9e-183">Example</span></span>

### <a name="request"></a><span data-ttu-id="45c9e-184">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45c9e-184">Request</span></span>
<span data-ttu-id="45c9e-185">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="45c9e-185">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations
Content-type: application/json
Content-length: 641

{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfiguration",
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
  ],
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "packageId": "Package Id value",
  "payloadJson": "Payload Json value",
  "permissionActions": [
    {
      "@odata.type": "microsoft.graph.androidPermissionAction",
      "permission": "Permission value",
      "action": "autoGrant"
    }
  ],
  "appSupportsOemConfig": true,
  "profileApplicability": "androidWorkProfile"
}
```

### <a name="response"></a><span data-ttu-id="45c9e-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="45c9e-186">Response</span></span>
<span data-ttu-id="45c9e-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="45c9e-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 813

{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfiguration",
  "id": "919a9335-9335-919a-3593-9a9135939a91",
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
  ],
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "packageId": "Package Id value",
  "payloadJson": "Payload Json value",
  "permissionActions": [
    {
      "@odata.type": "microsoft.graph.androidPermissionAction",
      "permission": "Permission value",
      "action": "autoGrant"
    }
  ],
  "appSupportsOemConfig": true,
  "profileApplicability": "androidWorkProfile"
}
```






