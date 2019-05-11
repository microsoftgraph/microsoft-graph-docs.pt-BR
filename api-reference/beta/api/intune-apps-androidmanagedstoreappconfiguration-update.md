---
title: Atualizar androidManagedStoreAppConfiguration
description: Atualiza as propriedades de um objeto androidManagedStoreAppConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7a2b1db8cf8f0a075edf5b291095b80f9bde361f
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33937201"
---
# <a name="update-androidmanagedstoreappconfiguration"></a><span data-ttu-id="a6a15-103">Atualizar androidManagedStoreAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="a6a15-103">Update androidManagedStoreAppConfiguration</span></span>

> <span data-ttu-id="a6a15-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a6a15-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6a15-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a6a15-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6a15-106">Atualiza as propriedades de um objeto [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a6a15-106">Update the properties of a [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6a15-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a6a15-107">Prerequisites</span></span>
<span data-ttu-id="a6a15-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6a15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6a15-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6a15-110">Permission type</span></span>|<span data-ttu-id="a6a15-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a6a15-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6a15-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6a15-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a6a15-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6a15-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a6a15-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6a15-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6a15-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6a15-115">Not supported.</span></span>|
|<span data-ttu-id="a6a15-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a6a15-116">Application</span></span>|<span data-ttu-id="a6a15-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6a15-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6a15-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a6a15-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a6a15-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a6a15-119">Request headers</span></span>
|<span data-ttu-id="a6a15-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a6a15-120">Header</span></span>|<span data-ttu-id="a6a15-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a6a15-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6a15-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a6a15-122">Authorization</span></span>|<span data-ttu-id="a6a15-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6a15-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6a15-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a6a15-124">Accept</span></span>|<span data-ttu-id="a6a15-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a6a15-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6a15-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a6a15-126">Request body</span></span>
<span data-ttu-id="a6a15-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a6a15-127">In the request body, supply a JSON representation for the [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object.</span></span>

<span data-ttu-id="a6a15-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a6a15-128">The following table shows the properties that are required when you create the [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md).</span></span>

|<span data-ttu-id="a6a15-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a6a15-129">Property</span></span>|<span data-ttu-id="a6a15-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6a15-130">Type</span></span>|<span data-ttu-id="a6a15-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6a15-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6a15-132">id</span><span class="sxs-lookup"><span data-stu-id="a6a15-132">id</span></span>|<span data-ttu-id="a6a15-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6a15-133">String</span></span>|<span data-ttu-id="a6a15-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a6a15-134">Key of the entity.</span></span> <span data-ttu-id="a6a15-135">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6a15-135">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="a6a15-136">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="a6a15-136">targetedMobileApps</span></span>|<span data-ttu-id="a6a15-137">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6a15-137">String collection</span></span>|<span data-ttu-id="a6a15-138">o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="a6a15-138">the associated app.</span></span> <span data-ttu-id="a6a15-139">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6a15-139">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="a6a15-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a6a15-140">roleScopeTagIds</span></span>|<span data-ttu-id="a6a15-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6a15-141">String collection</span></span>|<span data-ttu-id="a6a15-142">Lista de marcas de escopo para esta entidade de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a6a15-142">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="a6a15-143">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6a15-143">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="a6a15-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a6a15-144">createdDateTime</span></span>|<span data-ttu-id="a6a15-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6a15-145">DateTimeOffset</span></span>|<span data-ttu-id="a6a15-146">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="a6a15-146">DateTime the object was created.</span></span> <span data-ttu-id="a6a15-147">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6a15-147">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="a6a15-148">description</span><span class="sxs-lookup"><span data-stu-id="a6a15-148">description</span></span>|<span data-ttu-id="a6a15-149">String</span><span class="sxs-lookup"><span data-stu-id="a6a15-149">String</span></span>|<span data-ttu-id="a6a15-150">Descrição fornecida pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a6a15-150">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a6a15-151">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6a15-151">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="a6a15-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a6a15-152">lastModifiedDateTime</span></span>|<span data-ttu-id="a6a15-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6a15-153">DateTimeOffset</span></span>|<span data-ttu-id="a6a15-154">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="a6a15-154">DateTime the object was last modified.</span></span> <span data-ttu-id="a6a15-155">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6a15-155">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="a6a15-156">displayName</span><span class="sxs-lookup"><span data-stu-id="a6a15-156">displayName</span></span>|<span data-ttu-id="a6a15-157">String</span><span class="sxs-lookup"><span data-stu-id="a6a15-157">String</span></span>|<span data-ttu-id="a6a15-158">Nome fornecido pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a6a15-158">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a6a15-159">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6a15-159">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="a6a15-160">version</span><span class="sxs-lookup"><span data-stu-id="a6a15-160">version</span></span>|<span data-ttu-id="a6a15-161">Int32</span><span class="sxs-lookup"><span data-stu-id="a6a15-161">Int32</span></span>|<span data-ttu-id="a6a15-162">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a6a15-162">Version of the device configuration.</span></span> <span data-ttu-id="a6a15-163">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6a15-163">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="a6a15-164">packageId</span><span class="sxs-lookup"><span data-stu-id="a6a15-164">packageId</span></span>|<span data-ttu-id="a6a15-165">String</span><span class="sxs-lookup"><span data-stu-id="a6a15-165">String</span></span>|<span data-ttu-id="a6a15-166">ID do pacote de configuração do aplicativo Enterprise Android.</span><span class="sxs-lookup"><span data-stu-id="a6a15-166">Android Enterprise app configuration package id.</span></span>|
|<span data-ttu-id="a6a15-167">payloadJson</span><span class="sxs-lookup"><span data-stu-id="a6a15-167">payloadJson</span></span>|<span data-ttu-id="a6a15-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6a15-168">String</span></span>|<span data-ttu-id="a6a15-169">Carga JSON da configuração do aplicativo empresarial Android.</span><span class="sxs-lookup"><span data-stu-id="a6a15-169">Android Enterprise app configuration JSON payload.</span></span>|
|<span data-ttu-id="a6a15-170">permissionActions</span><span class="sxs-lookup"><span data-stu-id="a6a15-170">permissionActions</span></span>|<span data-ttu-id="a6a15-171">coleção [androidPermissionAction](../resources/intune-apps-androidpermissionaction.md)</span><span class="sxs-lookup"><span data-stu-id="a6a15-171">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="a6a15-172">Lista de permissões de aplicativo Android e ações de permissão correspondentes.</span><span class="sxs-lookup"><span data-stu-id="a6a15-172">List of Android app permissions and corresponding permission actions.</span></span>|
|<span data-ttu-id="a6a15-173">appSupportsOemConfig</span><span class="sxs-lookup"><span data-stu-id="a6a15-173">appSupportsOemConfig</span></span>|<span data-ttu-id="a6a15-174">Booliano</span><span class="sxs-lookup"><span data-stu-id="a6a15-174">Boolean</span></span>|<span data-ttu-id="a6a15-175">Se este AppConfig é ou não uma política de OEMConfig.</span><span class="sxs-lookup"><span data-stu-id="a6a15-175">Whether or not this AppConfig is an OEMConfig policy.</span></span>|



## <a name="response"></a><span data-ttu-id="a6a15-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6a15-176">Response</span></span>
<span data-ttu-id="a6a15-177">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a6a15-177">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6a15-178">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a6a15-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6a15-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6a15-179">Request</span></span>
<span data-ttu-id="a6a15-180">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6a15-180">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
Content-type: application/json
Content-length: 592

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
  "appSupportsOemConfig": true
}
```

### <a name="response"></a><span data-ttu-id="a6a15-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6a15-181">Response</span></span>
<span data-ttu-id="a6a15-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a6a15-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 764

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
  "appSupportsOemConfig": true
}
```




