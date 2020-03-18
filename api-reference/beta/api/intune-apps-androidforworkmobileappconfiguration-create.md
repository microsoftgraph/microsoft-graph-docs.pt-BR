---
title: Criar androidForWorkMobileAppConfiguration
description: Criar um novo objeto androidForWorkMobileAppConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5361f039a7d4f05260d76ff5a49ae3767f51296e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42762361"
---
# <a name="create-androidforworkmobileappconfiguration"></a><span data-ttu-id="b0e68-103">Criar androidForWorkMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="b0e68-103">Create androidForWorkMobileAppConfiguration</span></span>

> <span data-ttu-id="b0e68-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b0e68-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0e68-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b0e68-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0e68-106">Criar um novo objeto [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="b0e68-106">Create a new [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b0e68-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b0e68-107">Prerequisites</span></span>
<span data-ttu-id="b0e68-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0e68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0e68-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b0e68-110">Permission type</span></span>|<span data-ttu-id="b0e68-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b0e68-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0e68-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b0e68-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b0e68-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0e68-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b0e68-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b0e68-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0e68-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0e68-115">Not supported.</span></span>|
|<span data-ttu-id="b0e68-116">Application</span><span class="sxs-lookup"><span data-stu-id="b0e68-116">Application</span></span>|<span data-ttu-id="b0e68-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0e68-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0e68-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b0e68-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b0e68-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b0e68-119">Request headers</span></span>
|<span data-ttu-id="b0e68-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b0e68-120">Header</span></span>|<span data-ttu-id="b0e68-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b0e68-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0e68-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b0e68-122">Authorization</span></span>|<span data-ttu-id="b0e68-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b0e68-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0e68-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b0e68-124">Accept</span></span>|<span data-ttu-id="b0e68-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b0e68-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0e68-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b0e68-126">Request body</span></span>
<span data-ttu-id="b0e68-127">No corpo da solicitação, forneça uma representação JSON do objeto androidForWorkMobileAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="b0e68-127">In the request body, supply a JSON representation for the androidForWorkMobileAppConfiguration object.</span></span>

<span data-ttu-id="b0e68-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidForWorkMobileAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="b0e68-128">The following table shows the properties that are required when you create the androidForWorkMobileAppConfiguration.</span></span>

|<span data-ttu-id="b0e68-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0e68-129">Property</span></span>|<span data-ttu-id="b0e68-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0e68-130">Type</span></span>|<span data-ttu-id="b0e68-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0e68-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0e68-132">id</span><span class="sxs-lookup"><span data-stu-id="b0e68-132">id</span></span>|<span data-ttu-id="b0e68-133">String</span><span class="sxs-lookup"><span data-stu-id="b0e68-133">String</span></span>|<span data-ttu-id="b0e68-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b0e68-134">Key of the entity.</span></span> <span data-ttu-id="b0e68-135">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0e68-135">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b0e68-136">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="b0e68-136">targetedMobileApps</span></span>|<span data-ttu-id="b0e68-137">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0e68-137">String collection</span></span>|<span data-ttu-id="b0e68-138">o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="b0e68-138">the associated app.</span></span> <span data-ttu-id="b0e68-139">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0e68-139">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b0e68-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b0e68-140">roleScopeTagIds</span></span>|<span data-ttu-id="b0e68-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0e68-141">String collection</span></span>|<span data-ttu-id="b0e68-142">Lista de marcas de escopo para esta entidade de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b0e68-142">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="b0e68-143">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0e68-143">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b0e68-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b0e68-144">createdDateTime</span></span>|<span data-ttu-id="b0e68-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0e68-145">DateTimeOffset</span></span>|<span data-ttu-id="b0e68-146">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="b0e68-146">DateTime the object was created.</span></span> <span data-ttu-id="b0e68-147">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0e68-147">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b0e68-148">description</span><span class="sxs-lookup"><span data-stu-id="b0e68-148">description</span></span>|<span data-ttu-id="b0e68-149">String</span><span class="sxs-lookup"><span data-stu-id="b0e68-149">String</span></span>|<span data-ttu-id="b0e68-150">Descrição fornecida pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b0e68-150">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b0e68-151">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0e68-151">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b0e68-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b0e68-152">lastModifiedDateTime</span></span>|<span data-ttu-id="b0e68-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0e68-153">DateTimeOffset</span></span>|<span data-ttu-id="b0e68-154">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="b0e68-154">DateTime the object was last modified.</span></span> <span data-ttu-id="b0e68-155">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0e68-155">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b0e68-156">displayName</span><span class="sxs-lookup"><span data-stu-id="b0e68-156">displayName</span></span>|<span data-ttu-id="b0e68-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0e68-157">String</span></span>|<span data-ttu-id="b0e68-158">Nome fornecido pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b0e68-158">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b0e68-159">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0e68-159">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b0e68-160">version</span><span class="sxs-lookup"><span data-stu-id="b0e68-160">version</span></span>|<span data-ttu-id="b0e68-161">Int32</span><span class="sxs-lookup"><span data-stu-id="b0e68-161">Int32</span></span>|<span data-ttu-id="b0e68-162">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b0e68-162">Version of the device configuration.</span></span> <span data-ttu-id="b0e68-163">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0e68-163">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b0e68-164">packageId</span><span class="sxs-lookup"><span data-stu-id="b0e68-164">packageId</span></span>|<span data-ttu-id="b0e68-165">String</span><span class="sxs-lookup"><span data-stu-id="b0e68-165">String</span></span>|<span data-ttu-id="b0e68-166">ID do pacote de configuração do aplicativo Android for Work.</span><span class="sxs-lookup"><span data-stu-id="b0e68-166">Android For Work app configuration package id.</span></span>|
|<span data-ttu-id="b0e68-167">payloadJson</span><span class="sxs-lookup"><span data-stu-id="b0e68-167">payloadJson</span></span>|<span data-ttu-id="b0e68-168">String</span><span class="sxs-lookup"><span data-stu-id="b0e68-168">String</span></span>|<span data-ttu-id="b0e68-169">Carga JSON da configuração de aplicativo do Android for Work.</span><span class="sxs-lookup"><span data-stu-id="b0e68-169">Android For Work app configuration JSON payload.</span></span>|
|<span data-ttu-id="b0e68-170">permissionActions</span><span class="sxs-lookup"><span data-stu-id="b0e68-170">permissionActions</span></span>|<span data-ttu-id="b0e68-171">coleção [androidPermissionAction](../resources/intune-apps-androidpermissionaction.md)</span><span class="sxs-lookup"><span data-stu-id="b0e68-171">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="b0e68-172">Lista de permissões de aplicativo Android e ações de permissão correspondentes.</span><span class="sxs-lookup"><span data-stu-id="b0e68-172">List of Android app permissions and corresponding permission actions.</span></span>|



## <a name="response"></a><span data-ttu-id="b0e68-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0e68-173">Response</span></span>
<span data-ttu-id="b0e68-174">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b0e68-174">If successful, this method returns a `201 Created` response code and a [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0e68-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b0e68-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="b0e68-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b0e68-176">Request</span></span>
<span data-ttu-id="b0e68-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b0e68-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations
Content-type: application/json
Content-length: 560

{
  "@odata.type": "#microsoft.graph.androidForWorkMobileAppConfiguration",
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
  ]
}
```

### <a name="response"></a><span data-ttu-id="b0e68-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0e68-178">Response</span></span>
<span data-ttu-id="b0e68-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b0e68-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 732

{
  "@odata.type": "#microsoft.graph.androidForWorkMobileAppConfiguration",
  "id": "6204ae6d-ae6d-6204-6dae-04626dae0462",
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




