---
title: Atualizar androidManagedStoreAppConfiguration
description: Atualiza as propriedades de um objeto androidManagedStoreAppConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0441c234a3e33717b8f8c96b0a58614061f78621
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48006374"
---
# <a name="update-androidmanagedstoreappconfiguration"></a><span data-ttu-id="ebc90-103">Atualizar androidManagedStoreAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="ebc90-103">Update androidManagedStoreAppConfiguration</span></span>

<span data-ttu-id="ebc90-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ebc90-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ebc90-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ebc90-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ebc90-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ebc90-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebc90-107">Atualiza as propriedades de um objeto [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ebc90-107">Update the properties of a [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ebc90-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ebc90-108">Prerequisites</span></span>
<span data-ttu-id="ebc90-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebc90-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebc90-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ebc90-111">Permission type</span></span>|<span data-ttu-id="ebc90-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ebc90-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ebc90-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ebc90-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ebc90-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebc90-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ebc90-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ebc90-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ebc90-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ebc90-116">Not supported.</span></span>|
|<span data-ttu-id="ebc90-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ebc90-117">Application</span></span>|<span data-ttu-id="ebc90-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebc90-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ebc90-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ebc90-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ebc90-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ebc90-120">Request headers</span></span>
|<span data-ttu-id="ebc90-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ebc90-121">Header</span></span>|<span data-ttu-id="ebc90-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ebc90-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ebc90-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ebc90-123">Authorization</span></span>|<span data-ttu-id="ebc90-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ebc90-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ebc90-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ebc90-125">Accept</span></span>|<span data-ttu-id="ebc90-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ebc90-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebc90-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ebc90-127">Request body</span></span>
<span data-ttu-id="ebc90-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ebc90-128">In the request body, supply a JSON representation for the [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object.</span></span>

<span data-ttu-id="ebc90-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ebc90-129">The following table shows the properties that are required when you create the [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md).</span></span>

|<span data-ttu-id="ebc90-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ebc90-130">Property</span></span>|<span data-ttu-id="ebc90-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ebc90-131">Type</span></span>|<span data-ttu-id="ebc90-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ebc90-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebc90-133">id</span><span class="sxs-lookup"><span data-stu-id="ebc90-133">id</span></span>|<span data-ttu-id="ebc90-134">String</span><span class="sxs-lookup"><span data-stu-id="ebc90-134">String</span></span>|<span data-ttu-id="ebc90-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ebc90-135">Key of the entity.</span></span> <span data-ttu-id="ebc90-136">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ebc90-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ebc90-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="ebc90-137">targetedMobileApps</span></span>|<span data-ttu-id="ebc90-138">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ebc90-138">String collection</span></span>|<span data-ttu-id="ebc90-139">o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="ebc90-139">the associated app.</span></span> <span data-ttu-id="ebc90-140">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ebc90-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ebc90-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ebc90-141">roleScopeTagIds</span></span>|<span data-ttu-id="ebc90-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ebc90-142">String collection</span></span>|<span data-ttu-id="ebc90-143">Lista de marcas de escopo para esta entidade de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ebc90-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="ebc90-144">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ebc90-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ebc90-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ebc90-145">createdDateTime</span></span>|<span data-ttu-id="ebc90-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebc90-146">DateTimeOffset</span></span>|<span data-ttu-id="ebc90-147">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="ebc90-147">DateTime the object was created.</span></span> <span data-ttu-id="ebc90-148">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ebc90-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ebc90-149">description</span><span class="sxs-lookup"><span data-stu-id="ebc90-149">description</span></span>|<span data-ttu-id="ebc90-150">String</span><span class="sxs-lookup"><span data-stu-id="ebc90-150">String</span></span>|<span data-ttu-id="ebc90-151">Descrição fornecida pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ebc90-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ebc90-152">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ebc90-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ebc90-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ebc90-153">lastModifiedDateTime</span></span>|<span data-ttu-id="ebc90-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebc90-154">DateTimeOffset</span></span>|<span data-ttu-id="ebc90-155">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="ebc90-155">DateTime the object was last modified.</span></span> <span data-ttu-id="ebc90-156">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ebc90-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ebc90-157">displayName</span><span class="sxs-lookup"><span data-stu-id="ebc90-157">displayName</span></span>|<span data-ttu-id="ebc90-158">String</span><span class="sxs-lookup"><span data-stu-id="ebc90-158">String</span></span>|<span data-ttu-id="ebc90-159">Nome fornecido pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ebc90-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ebc90-160">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ebc90-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ebc90-161">version</span><span class="sxs-lookup"><span data-stu-id="ebc90-161">version</span></span>|<span data-ttu-id="ebc90-162">Int32</span><span class="sxs-lookup"><span data-stu-id="ebc90-162">Int32</span></span>|<span data-ttu-id="ebc90-163">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ebc90-163">Version of the device configuration.</span></span> <span data-ttu-id="ebc90-164">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ebc90-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ebc90-165">packageId</span><span class="sxs-lookup"><span data-stu-id="ebc90-165">packageId</span></span>|<span data-ttu-id="ebc90-166">String</span><span class="sxs-lookup"><span data-stu-id="ebc90-166">String</span></span>|<span data-ttu-id="ebc90-167">ID do pacote de configuração do aplicativo Enterprise Android.</span><span class="sxs-lookup"><span data-stu-id="ebc90-167">Android Enterprise app configuration package id.</span></span>|
|<span data-ttu-id="ebc90-168">payloadJson</span><span class="sxs-lookup"><span data-stu-id="ebc90-168">payloadJson</span></span>|<span data-ttu-id="ebc90-169">String</span><span class="sxs-lookup"><span data-stu-id="ebc90-169">String</span></span>|<span data-ttu-id="ebc90-170">Carga JSON da configuração do aplicativo empresarial Android.</span><span class="sxs-lookup"><span data-stu-id="ebc90-170">Android Enterprise app configuration JSON payload.</span></span>|
|<span data-ttu-id="ebc90-171">permissionActions</span><span class="sxs-lookup"><span data-stu-id="ebc90-171">permissionActions</span></span>|<span data-ttu-id="ebc90-172">coleção [androidPermissionAction](../resources/intune-apps-androidpermissionaction.md)</span><span class="sxs-lookup"><span data-stu-id="ebc90-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="ebc90-173">Lista de permissões de aplicativo Android e ações de permissão correspondentes.</span><span class="sxs-lookup"><span data-stu-id="ebc90-173">List of Android app permissions and corresponding permission actions.</span></span>|
|<span data-ttu-id="ebc90-174">appSupportsOemConfig</span><span class="sxs-lookup"><span data-stu-id="ebc90-174">appSupportsOemConfig</span></span>|<span data-ttu-id="ebc90-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="ebc90-175">Boolean</span></span>|<span data-ttu-id="ebc90-176">Se este AppConfig é ou não uma política de OEMConfig.</span><span class="sxs-lookup"><span data-stu-id="ebc90-176">Whether or not this AppConfig is an OEMConfig policy.</span></span>|
|<span data-ttu-id="ebc90-177">profileApplicability</span><span class="sxs-lookup"><span data-stu-id="ebc90-177">profileApplicability</span></span>|[<span data-ttu-id="ebc90-178">androidProfileApplicability</span><span class="sxs-lookup"><span data-stu-id="ebc90-178">androidProfileApplicability</span></span>](../resources/intune-apps-androidprofileapplicability.md)|<span data-ttu-id="ebc90-179">Aplicabilidade de perfil corporativo Android (AndroidWorkProfile, DeviceOwner ou default (aplica-se a ambos)).</span><span class="sxs-lookup"><span data-stu-id="ebc90-179">Android Enterprise profile applicability (AndroidWorkProfile, DeviceOwner, or default (applies to both)).</span></span> <span data-ttu-id="ebc90-180">Os valores possíveis são: `default`, `androidWorkProfile`, `androidDeviceOwner`.</span><span class="sxs-lookup"><span data-stu-id="ebc90-180">Possible values are: `default`, `androidWorkProfile`, `androidDeviceOwner`.</span></span>|



## <a name="response"></a><span data-ttu-id="ebc90-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebc90-181">Response</span></span>
<span data-ttu-id="ebc90-182">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ebc90-182">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebc90-183">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ebc90-183">Example</span></span>

### <a name="request"></a><span data-ttu-id="ebc90-184">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ebc90-184">Request</span></span>
<span data-ttu-id="ebc90-185">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ebc90-185">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
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

### <a name="response"></a><span data-ttu-id="ebc90-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebc90-186">Response</span></span>
<span data-ttu-id="ebc90-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ebc90-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






