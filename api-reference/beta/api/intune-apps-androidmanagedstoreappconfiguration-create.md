---
title: Criar androidManagedStoreAppConfiguration
description: Criar um novo objeto androidManagedStoreAppConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: af0a0d02b7877c17c1211af4b7e8e01b208ea1f4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35952174"
---
# <a name="create-androidmanagedstoreappconfiguration"></a><span data-ttu-id="44c17-103">Criar androidManagedStoreAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="44c17-103">Create androidManagedStoreAppConfiguration</span></span>

> <span data-ttu-id="44c17-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="44c17-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44c17-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="44c17-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44c17-106">Criar um novo objeto [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="44c17-106">Create a new [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="44c17-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="44c17-107">Prerequisites</span></span>
<span data-ttu-id="44c17-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44c17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44c17-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="44c17-110">Permission type</span></span>|<span data-ttu-id="44c17-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="44c17-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44c17-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="44c17-112">Delegated (work or school account)</span></span>|<span data-ttu-id="44c17-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44c17-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="44c17-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="44c17-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44c17-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="44c17-115">Not supported.</span></span>|
|<span data-ttu-id="44c17-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="44c17-116">Application</span></span>|<span data-ttu-id="44c17-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="44c17-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="44c17-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="44c17-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="44c17-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="44c17-119">Request headers</span></span>
|<span data-ttu-id="44c17-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="44c17-120">Header</span></span>|<span data-ttu-id="44c17-121">Valor</span><span class="sxs-lookup"><span data-stu-id="44c17-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44c17-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="44c17-122">Authorization</span></span>|<span data-ttu-id="44c17-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="44c17-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44c17-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="44c17-124">Accept</span></span>|<span data-ttu-id="44c17-125">application/json</span><span class="sxs-lookup"><span data-stu-id="44c17-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44c17-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="44c17-126">Request body</span></span>
<span data-ttu-id="44c17-127">No corpo da solicitação, forneça uma representação JSON do objeto androidManagedStoreAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="44c17-127">In the request body, supply a JSON representation for the androidManagedStoreAppConfiguration object.</span></span>

<span data-ttu-id="44c17-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidManagedStoreAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="44c17-128">The following table shows the properties that are required when you create the androidManagedStoreAppConfiguration.</span></span>

|<span data-ttu-id="44c17-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="44c17-129">Property</span></span>|<span data-ttu-id="44c17-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="44c17-130">Type</span></span>|<span data-ttu-id="44c17-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="44c17-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44c17-132">id</span><span class="sxs-lookup"><span data-stu-id="44c17-132">id</span></span>|<span data-ttu-id="44c17-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="44c17-133">String</span></span>|<span data-ttu-id="44c17-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="44c17-134">Key of the entity.</span></span> <span data-ttu-id="44c17-135">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44c17-135">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="44c17-136">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="44c17-136">targetedMobileApps</span></span>|<span data-ttu-id="44c17-137">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="44c17-137">String collection</span></span>|<span data-ttu-id="44c17-138">o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="44c17-138">the associated app.</span></span> <span data-ttu-id="44c17-139">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44c17-139">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="44c17-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="44c17-140">roleScopeTagIds</span></span>|<span data-ttu-id="44c17-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="44c17-141">String collection</span></span>|<span data-ttu-id="44c17-142">Lista de marcas de escopo para esta entidade de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="44c17-142">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="44c17-143">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44c17-143">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="44c17-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="44c17-144">createdDateTime</span></span>|<span data-ttu-id="44c17-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44c17-145">DateTimeOffset</span></span>|<span data-ttu-id="44c17-146">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="44c17-146">DateTime the object was created.</span></span> <span data-ttu-id="44c17-147">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44c17-147">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="44c17-148">descrição</span><span class="sxs-lookup"><span data-stu-id="44c17-148">description</span></span>|<span data-ttu-id="44c17-149">String</span><span class="sxs-lookup"><span data-stu-id="44c17-149">String</span></span>|<span data-ttu-id="44c17-150">Descrição fornecida pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="44c17-150">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="44c17-151">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44c17-151">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="44c17-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="44c17-152">lastModifiedDateTime</span></span>|<span data-ttu-id="44c17-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44c17-153">DateTimeOffset</span></span>|<span data-ttu-id="44c17-154">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="44c17-154">DateTime the object was last modified.</span></span> <span data-ttu-id="44c17-155">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44c17-155">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="44c17-156">displayName</span><span class="sxs-lookup"><span data-stu-id="44c17-156">displayName</span></span>|<span data-ttu-id="44c17-157">String</span><span class="sxs-lookup"><span data-stu-id="44c17-157">String</span></span>|<span data-ttu-id="44c17-158">Nome fornecido pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="44c17-158">Admin provided name of the device configuration.</span></span> <span data-ttu-id="44c17-159">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44c17-159">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="44c17-160">version</span><span class="sxs-lookup"><span data-stu-id="44c17-160">version</span></span>|<span data-ttu-id="44c17-161">Int32</span><span class="sxs-lookup"><span data-stu-id="44c17-161">Int32</span></span>|<span data-ttu-id="44c17-162">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="44c17-162">Version of the device configuration.</span></span> <span data-ttu-id="44c17-163">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44c17-163">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="44c17-164">packageId</span><span class="sxs-lookup"><span data-stu-id="44c17-164">packageId</span></span>|<span data-ttu-id="44c17-165">String</span><span class="sxs-lookup"><span data-stu-id="44c17-165">String</span></span>|<span data-ttu-id="44c17-166">ID do pacote de configuração do aplicativo Enterprise Android.</span><span class="sxs-lookup"><span data-stu-id="44c17-166">Android Enterprise app configuration package id.</span></span>|
|<span data-ttu-id="44c17-167">payloadJson</span><span class="sxs-lookup"><span data-stu-id="44c17-167">payloadJson</span></span>|<span data-ttu-id="44c17-168">String</span><span class="sxs-lookup"><span data-stu-id="44c17-168">String</span></span>|<span data-ttu-id="44c17-169">Carga JSON da configuração do aplicativo empresarial Android.</span><span class="sxs-lookup"><span data-stu-id="44c17-169">Android Enterprise app configuration JSON payload.</span></span>|
|<span data-ttu-id="44c17-170">permissionActions</span><span class="sxs-lookup"><span data-stu-id="44c17-170">permissionActions</span></span>|<span data-ttu-id="44c17-171">coleção [androidPermissionAction](../resources/intune-apps-androidpermissionaction.md)</span><span class="sxs-lookup"><span data-stu-id="44c17-171">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="44c17-172">Lista de permissões de aplicativo Android e ações de permissão correspondentes.</span><span class="sxs-lookup"><span data-stu-id="44c17-172">List of Android app permissions and corresponding permission actions.</span></span>|
|<span data-ttu-id="44c17-173">appSupportsOemConfig</span><span class="sxs-lookup"><span data-stu-id="44c17-173">appSupportsOemConfig</span></span>|<span data-ttu-id="44c17-174">Booliano</span><span class="sxs-lookup"><span data-stu-id="44c17-174">Boolean</span></span>|<span data-ttu-id="44c17-175">Se este AppConfig é ou não uma política de OEMConfig.</span><span class="sxs-lookup"><span data-stu-id="44c17-175">Whether or not this AppConfig is an OEMConfig policy.</span></span>|



## <a name="response"></a><span data-ttu-id="44c17-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="44c17-176">Response</span></span>
<span data-ttu-id="44c17-177">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="44c17-177">If successful, this method returns a `201 Created` response code and a [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44c17-178">Exemplo</span><span class="sxs-lookup"><span data-stu-id="44c17-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="44c17-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="44c17-179">Request</span></span>
<span data-ttu-id="44c17-180">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="44c17-180">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations
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

### <a name="response"></a><span data-ttu-id="44c17-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="44c17-181">Response</span></span>
<span data-ttu-id="44c17-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="44c17-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





