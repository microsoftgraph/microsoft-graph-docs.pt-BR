---
title: Criar androidManagedStoreAppConfiguration
description: Criar um novo objeto androidManagedStoreAppConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 295f02e35e8d25b096678216817a11e9b4ac5c69
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32496860"
---
# <a name="create-androidmanagedstoreappconfiguration"></a><span data-ttu-id="2f240-103">Criar androidManagedStoreAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="2f240-103">Create androidManagedStoreAppConfiguration</span></span>

> <span data-ttu-id="2f240-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2f240-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f240-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2f240-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f240-106">Criar um novo objeto [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="2f240-106">Create a new [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f240-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2f240-107">Prerequisites</span></span>
<span data-ttu-id="2f240-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f240-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f240-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f240-110">Permission type</span></span>|<span data-ttu-id="2f240-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2f240-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f240-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f240-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2f240-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f240-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2f240-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f240-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f240-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f240-115">Not supported.</span></span>|
|<span data-ttu-id="2f240-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f240-116">Application</span></span>|<span data-ttu-id="2f240-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f240-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f240-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f240-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2f240-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f240-119">Request headers</span></span>
|<span data-ttu-id="2f240-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2f240-120">Header</span></span>|<span data-ttu-id="2f240-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2f240-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f240-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f240-122">Authorization</span></span>|<span data-ttu-id="2f240-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f240-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f240-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2f240-124">Accept</span></span>|<span data-ttu-id="2f240-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2f240-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f240-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f240-126">Request body</span></span>
<span data-ttu-id="2f240-127">No corpo da solicitação, forneça uma representação JSON do objeto androidManagedStoreAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="2f240-127">In the request body, supply a JSON representation for the androidManagedStoreAppConfiguration object.</span></span>

<span data-ttu-id="2f240-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidManagedStoreAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="2f240-128">The following table shows the properties that are required when you create the androidManagedStoreAppConfiguration.</span></span>

|<span data-ttu-id="2f240-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2f240-129">Property</span></span>|<span data-ttu-id="2f240-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f240-130">Type</span></span>|<span data-ttu-id="2f240-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f240-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f240-132">id</span><span class="sxs-lookup"><span data-stu-id="2f240-132">id</span></span>|<span data-ttu-id="2f240-133">String</span><span class="sxs-lookup"><span data-stu-id="2f240-133">String</span></span>|<span data-ttu-id="2f240-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2f240-134">Key of the entity.</span></span> <span data-ttu-id="2f240-135">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f240-135">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="2f240-136">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="2f240-136">targetedMobileApps</span></span>|<span data-ttu-id="2f240-137">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f240-137">String collection</span></span>|<span data-ttu-id="2f240-138">o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="2f240-138">the associated app.</span></span> <span data-ttu-id="2f240-139">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f240-139">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="2f240-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2f240-140">roleScopeTagIds</span></span>|<span data-ttu-id="2f240-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f240-141">String collection</span></span>|<span data-ttu-id="2f240-142">Lista de marcas de escopo para esta entidade de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2f240-142">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="2f240-143">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f240-143">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="2f240-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2f240-144">createdDateTime</span></span>|<span data-ttu-id="2f240-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f240-145">DateTimeOffset</span></span>|<span data-ttu-id="2f240-146">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="2f240-146">DateTime the object was created.</span></span> <span data-ttu-id="2f240-147">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f240-147">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="2f240-148">description</span><span class="sxs-lookup"><span data-stu-id="2f240-148">description</span></span>|<span data-ttu-id="2f240-149">String</span><span class="sxs-lookup"><span data-stu-id="2f240-149">String</span></span>|<span data-ttu-id="2f240-150">Descrição fornecida pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2f240-150">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2f240-151">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f240-151">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="2f240-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f240-152">lastModifiedDateTime</span></span>|<span data-ttu-id="2f240-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f240-153">DateTimeOffset</span></span>|<span data-ttu-id="2f240-154">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="2f240-154">DateTime the object was last modified.</span></span> <span data-ttu-id="2f240-155">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f240-155">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="2f240-156">displayName</span><span class="sxs-lookup"><span data-stu-id="2f240-156">displayName</span></span>|<span data-ttu-id="2f240-157">String</span><span class="sxs-lookup"><span data-stu-id="2f240-157">String</span></span>|<span data-ttu-id="2f240-158">Nome fornecido pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2f240-158">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2f240-159">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f240-159">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="2f240-160">version</span><span class="sxs-lookup"><span data-stu-id="2f240-160">version</span></span>|<span data-ttu-id="2f240-161">Int32</span><span class="sxs-lookup"><span data-stu-id="2f240-161">Int32</span></span>|<span data-ttu-id="2f240-162">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2f240-162">Version of the device configuration.</span></span> <span data-ttu-id="2f240-163">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f240-163">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="2f240-164">packageId</span><span class="sxs-lookup"><span data-stu-id="2f240-164">packageId</span></span>|<span data-ttu-id="2f240-165">String</span><span class="sxs-lookup"><span data-stu-id="2f240-165">String</span></span>|<span data-ttu-id="2f240-166">ID do pacote de configuração do aplicativo Enterprise Android.</span><span class="sxs-lookup"><span data-stu-id="2f240-166">Android Enterprise app configuration package id.</span></span>|
|<span data-ttu-id="2f240-167">payloadJson</span><span class="sxs-lookup"><span data-stu-id="2f240-167">payloadJson</span></span>|<span data-ttu-id="2f240-168">String</span><span class="sxs-lookup"><span data-stu-id="2f240-168">String</span></span>|<span data-ttu-id="2f240-169">Carga JSON da configuração do aplicativo empresarial Android.</span><span class="sxs-lookup"><span data-stu-id="2f240-169">Android Enterprise app configuration JSON payload.</span></span>|
|<span data-ttu-id="2f240-170">permissionActions</span><span class="sxs-lookup"><span data-stu-id="2f240-170">permissionActions</span></span>|<span data-ttu-id="2f240-171">coleção [androidPermissionAction](../resources/intune-apps-androidpermissionaction.md)</span><span class="sxs-lookup"><span data-stu-id="2f240-171">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="2f240-172">Lista de permissões de aplicativo Android e ações de permissão correspondentes.</span><span class="sxs-lookup"><span data-stu-id="2f240-172">List of Android app permissions and corresponding permission actions.</span></span>|
|<span data-ttu-id="2f240-173">appSupportsOemConfig</span><span class="sxs-lookup"><span data-stu-id="2f240-173">appSupportsOemConfig</span></span>|<span data-ttu-id="2f240-174">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f240-174">Boolean</span></span>|<span data-ttu-id="2f240-175">Se este AppConfig é ou não uma política de OEMConfig.</span><span class="sxs-lookup"><span data-stu-id="2f240-175">Whether or not this AppConfig is an OEMConfig policy.</span></span>|



## <a name="response"></a><span data-ttu-id="2f240-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f240-176">Response</span></span>
<span data-ttu-id="2f240-177">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f240-177">If successful, this method returns a `201 Created` response code and a [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f240-178">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f240-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f240-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f240-179">Request</span></span>
<span data-ttu-id="2f240-180">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f240-180">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2f240-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f240-181">Response</span></span>
<span data-ttu-id="2f240-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f240-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





