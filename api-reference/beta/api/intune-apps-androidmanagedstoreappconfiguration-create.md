---
title: Criar androidManagedStoreAppConfiguration
description: Crie um novo objeto de androidManagedStoreAppConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0d449c87ea880874a3a2d13e5fc466004fb4be8a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956042"
---
# <a name="create-androidmanagedstoreappconfiguration"></a><span data-ttu-id="84dc1-103">Criar androidManagedStoreAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="84dc1-103">Create androidManagedStoreAppConfiguration</span></span>

> <span data-ttu-id="84dc1-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="84dc1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="84dc1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="84dc1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="84dc1-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="84dc1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="84dc1-107">Crie um novo objeto de [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="84dc1-107">Create a new [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="84dc1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="84dc1-108">Prerequisites</span></span>
<span data-ttu-id="84dc1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84dc1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84dc1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="84dc1-111">Permission type</span></span>|<span data-ttu-id="84dc1-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="84dc1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84dc1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="84dc1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="84dc1-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84dc1-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="84dc1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="84dc1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84dc1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84dc1-116">Not supported.</span></span>|
|<span data-ttu-id="84dc1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="84dc1-117">Application</span></span>|<span data-ttu-id="84dc1-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84dc1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="84dc1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="84dc1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="84dc1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="84dc1-120">Request headers</span></span>
|<span data-ttu-id="84dc1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="84dc1-121">Header</span></span>|<span data-ttu-id="84dc1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="84dc1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84dc1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="84dc1-123">Authorization</span></span>|<span data-ttu-id="84dc1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="84dc1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84dc1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="84dc1-125">Accept</span></span>|<span data-ttu-id="84dc1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="84dc1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84dc1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="84dc1-127">Request body</span></span>
<span data-ttu-id="84dc1-128">No corpo da solicitação, fornece uma representação JSON para o objeto androidManagedStoreAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="84dc1-128">In the request body, supply a JSON representation for the androidManagedStoreAppConfiguration object.</span></span>

<span data-ttu-id="84dc1-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o androidManagedStoreAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="84dc1-129">The following table shows the properties that are required when you create the androidManagedStoreAppConfiguration.</span></span>

|<span data-ttu-id="84dc1-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="84dc1-130">Property</span></span>|<span data-ttu-id="84dc1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="84dc1-131">Type</span></span>|<span data-ttu-id="84dc1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="84dc1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84dc1-133">id</span><span class="sxs-lookup"><span data-stu-id="84dc1-133">id</span></span>|<span data-ttu-id="84dc1-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="84dc1-134">String</span></span>|<span data-ttu-id="84dc1-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="84dc1-135">Key of the entity.</span></span> <span data-ttu-id="84dc1-136">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84dc1-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="84dc1-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="84dc1-137">targetedMobileApps</span></span>|<span data-ttu-id="84dc1-138">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="84dc1-138">String collection</span></span>|<span data-ttu-id="84dc1-139">o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="84dc1-139">the associated app.</span></span> <span data-ttu-id="84dc1-140">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84dc1-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="84dc1-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="84dc1-141">roleScopeTagIds</span></span>|<span data-ttu-id="84dc1-142">String collection</span><span class="sxs-lookup"><span data-stu-id="84dc1-142">String collection</span></span>|<span data-ttu-id="84dc1-143">Lista de escopo marcas para essa entidade de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="84dc1-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="84dc1-144">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84dc1-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="84dc1-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="84dc1-145">createdDateTime</span></span>|<span data-ttu-id="84dc1-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84dc1-146">DateTimeOffset</span></span>|<span data-ttu-id="84dc1-147">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="84dc1-147">DateTime the object was created.</span></span> <span data-ttu-id="84dc1-148">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84dc1-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="84dc1-149">description</span><span class="sxs-lookup"><span data-stu-id="84dc1-149">description</span></span>|<span data-ttu-id="84dc1-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="84dc1-150">String</span></span>|<span data-ttu-id="84dc1-151">Descrição fornecida pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="84dc1-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="84dc1-152">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84dc1-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="84dc1-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="84dc1-153">lastModifiedDateTime</span></span>|<span data-ttu-id="84dc1-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84dc1-154">DateTimeOffset</span></span>|<span data-ttu-id="84dc1-155">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="84dc1-155">DateTime the object was last modified.</span></span> <span data-ttu-id="84dc1-156">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84dc1-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="84dc1-157">displayName</span><span class="sxs-lookup"><span data-stu-id="84dc1-157">displayName</span></span>|<span data-ttu-id="84dc1-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="84dc1-158">String</span></span>|<span data-ttu-id="84dc1-159">Nome fornecido pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="84dc1-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="84dc1-160">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84dc1-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="84dc1-161">version</span><span class="sxs-lookup"><span data-stu-id="84dc1-161">version</span></span>|<span data-ttu-id="84dc1-162">Int32</span><span class="sxs-lookup"><span data-stu-id="84dc1-162">Int32</span></span>|<span data-ttu-id="84dc1-163">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="84dc1-163">Version of the device configuration.</span></span> <span data-ttu-id="84dc1-164">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84dc1-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="84dc1-165">packageId</span><span class="sxs-lookup"><span data-stu-id="84dc1-165">packageId</span></span>|<span data-ttu-id="84dc1-166">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="84dc1-166">String</span></span>|<span data-ttu-id="84dc1-167">Android Enterprise app configuração id do pacote.</span><span class="sxs-lookup"><span data-stu-id="84dc1-167">Android Enterprise app configuration package id.</span></span>|
|<span data-ttu-id="84dc1-168">payloadJson</span><span class="sxs-lookup"><span data-stu-id="84dc1-168">payloadJson</span></span>|<span data-ttu-id="84dc1-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="84dc1-169">String</span></span>|<span data-ttu-id="84dc1-170">Carga dos JSON de configuração de aplicativo do Android Enterprise.</span><span class="sxs-lookup"><span data-stu-id="84dc1-170">Android Enterprise app configuration JSON payload.</span></span>|
|<span data-ttu-id="84dc1-171">permissionActions</span><span class="sxs-lookup"><span data-stu-id="84dc1-171">permissionActions</span></span>|<span data-ttu-id="84dc1-172">coleção [androidPermissionAction](../resources/intune-apps-androidpermissionaction.md)</span><span class="sxs-lookup"><span data-stu-id="84dc1-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="84dc1-173">Lista de permissões do aplicativo Android e ações correspondentes de permissão.</span><span class="sxs-lookup"><span data-stu-id="84dc1-173">List of Android app permissions and corresponding permission actions.</span></span>|



## <a name="response"></a><span data-ttu-id="84dc1-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="84dc1-174">Response</span></span>
<span data-ttu-id="84dc1-175">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="84dc1-175">If successful, this method returns a `201 Created` response code and a [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84dc1-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="84dc1-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="84dc1-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="84dc1-177">Request</span></span>
<span data-ttu-id="84dc1-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="84dc1-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations
Content-type: application/json
Content-length: 623

{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfiguration",
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
  ],
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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
  ]
}
```

### <a name="response"></a><span data-ttu-id="84dc1-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="84dc1-179">Response</span></span>
<span data-ttu-id="84dc1-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="84dc1-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 731

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
  ]
}
```





