---
title: Atualizar androidForWorkMobileAppConfiguration
description: Atualiza as propriedades de um objeto androidForWorkMobileAppConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a1003f7a4db7ecc8138544697a898656334b8b06
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48006416"
---
# <a name="update-androidforworkmobileappconfiguration"></a><span data-ttu-id="becfe-103">Atualizar androidForWorkMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="becfe-103">Update androidForWorkMobileAppConfiguration</span></span>

<span data-ttu-id="becfe-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="becfe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="becfe-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="becfe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="becfe-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="becfe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="becfe-107">Atualiza as propriedades de um objeto [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="becfe-107">Update the properties of a [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="becfe-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="becfe-108">Prerequisites</span></span>
<span data-ttu-id="becfe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="becfe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="becfe-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="becfe-111">Permission type</span></span>|<span data-ttu-id="becfe-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="becfe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="becfe-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="becfe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="becfe-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="becfe-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="becfe-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="becfe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="becfe-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="becfe-116">Not supported.</span></span>|
|<span data-ttu-id="becfe-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="becfe-117">Application</span></span>|<span data-ttu-id="becfe-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="becfe-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="becfe-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="becfe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="becfe-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="becfe-120">Request headers</span></span>
|<span data-ttu-id="becfe-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="becfe-121">Header</span></span>|<span data-ttu-id="becfe-122">Valor</span><span class="sxs-lookup"><span data-stu-id="becfe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="becfe-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="becfe-123">Authorization</span></span>|<span data-ttu-id="becfe-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="becfe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="becfe-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="becfe-125">Accept</span></span>|<span data-ttu-id="becfe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="becfe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="becfe-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="becfe-127">Request body</span></span>
<span data-ttu-id="becfe-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="becfe-128">In the request body, supply a JSON representation for the [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object.</span></span>

<span data-ttu-id="becfe-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="becfe-129">The following table shows the properties that are required when you create the [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md).</span></span>

|<span data-ttu-id="becfe-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="becfe-130">Property</span></span>|<span data-ttu-id="becfe-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="becfe-131">Type</span></span>|<span data-ttu-id="becfe-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="becfe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="becfe-133">id</span><span class="sxs-lookup"><span data-stu-id="becfe-133">id</span></span>|<span data-ttu-id="becfe-134">String</span><span class="sxs-lookup"><span data-stu-id="becfe-134">String</span></span>|<span data-ttu-id="becfe-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="becfe-135">Key of the entity.</span></span> <span data-ttu-id="becfe-136">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="becfe-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="becfe-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="becfe-137">targetedMobileApps</span></span>|<span data-ttu-id="becfe-138">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="becfe-138">String collection</span></span>|<span data-ttu-id="becfe-139">o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="becfe-139">the associated app.</span></span> <span data-ttu-id="becfe-140">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="becfe-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="becfe-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="becfe-141">roleScopeTagIds</span></span>|<span data-ttu-id="becfe-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="becfe-142">String collection</span></span>|<span data-ttu-id="becfe-143">Lista de marcas de escopo para esta entidade de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="becfe-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="becfe-144">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="becfe-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="becfe-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="becfe-145">createdDateTime</span></span>|<span data-ttu-id="becfe-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="becfe-146">DateTimeOffset</span></span>|<span data-ttu-id="becfe-147">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="becfe-147">DateTime the object was created.</span></span> <span data-ttu-id="becfe-148">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="becfe-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="becfe-149">description</span><span class="sxs-lookup"><span data-stu-id="becfe-149">description</span></span>|<span data-ttu-id="becfe-150">String</span><span class="sxs-lookup"><span data-stu-id="becfe-150">String</span></span>|<span data-ttu-id="becfe-151">Descrição fornecida pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="becfe-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="becfe-152">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="becfe-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="becfe-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="becfe-153">lastModifiedDateTime</span></span>|<span data-ttu-id="becfe-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="becfe-154">DateTimeOffset</span></span>|<span data-ttu-id="becfe-155">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="becfe-155">DateTime the object was last modified.</span></span> <span data-ttu-id="becfe-156">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="becfe-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="becfe-157">displayName</span><span class="sxs-lookup"><span data-stu-id="becfe-157">displayName</span></span>|<span data-ttu-id="becfe-158">String</span><span class="sxs-lookup"><span data-stu-id="becfe-158">String</span></span>|<span data-ttu-id="becfe-159">Nome fornecido pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="becfe-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="becfe-160">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="becfe-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="becfe-161">version</span><span class="sxs-lookup"><span data-stu-id="becfe-161">version</span></span>|<span data-ttu-id="becfe-162">Int32</span><span class="sxs-lookup"><span data-stu-id="becfe-162">Int32</span></span>|<span data-ttu-id="becfe-163">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="becfe-163">Version of the device configuration.</span></span> <span data-ttu-id="becfe-164">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="becfe-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="becfe-165">packageId</span><span class="sxs-lookup"><span data-stu-id="becfe-165">packageId</span></span>|<span data-ttu-id="becfe-166">String</span><span class="sxs-lookup"><span data-stu-id="becfe-166">String</span></span>|<span data-ttu-id="becfe-167">ID do pacote de configuração do aplicativo Android for Work.</span><span class="sxs-lookup"><span data-stu-id="becfe-167">Android For Work app configuration package id.</span></span>|
|<span data-ttu-id="becfe-168">payloadJson</span><span class="sxs-lookup"><span data-stu-id="becfe-168">payloadJson</span></span>|<span data-ttu-id="becfe-169">String</span><span class="sxs-lookup"><span data-stu-id="becfe-169">String</span></span>|<span data-ttu-id="becfe-170">Carga JSON da configuração de aplicativo do Android for Work.</span><span class="sxs-lookup"><span data-stu-id="becfe-170">Android For Work app configuration JSON payload.</span></span>|
|<span data-ttu-id="becfe-171">permissionActions</span><span class="sxs-lookup"><span data-stu-id="becfe-171">permissionActions</span></span>|<span data-ttu-id="becfe-172">coleção [androidPermissionAction](../resources/intune-apps-androidpermissionaction.md)</span><span class="sxs-lookup"><span data-stu-id="becfe-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="becfe-173">Lista de permissões de aplicativo Android e ações de permissão correspondentes.</span><span class="sxs-lookup"><span data-stu-id="becfe-173">List of Android app permissions and corresponding permission actions.</span></span>|
|<span data-ttu-id="becfe-174">profileApplicability</span><span class="sxs-lookup"><span data-stu-id="becfe-174">profileApplicability</span></span>|[<span data-ttu-id="becfe-175">androidProfileApplicability</span><span class="sxs-lookup"><span data-stu-id="becfe-175">androidProfileApplicability</span></span>](../resources/intune-apps-androidprofileapplicability.md)|<span data-ttu-id="becfe-176">Aplicabilidade de perfil corporativo Android (AndroidWorkProfile, DeviceOwner ou default (aplica-se a ambos)).</span><span class="sxs-lookup"><span data-stu-id="becfe-176">Android Enterprise profile applicability (AndroidWorkProfile, DeviceOwner, or default (applies to both)).</span></span> <span data-ttu-id="becfe-177">Os valores possíveis são: `default`, `androidWorkProfile`, `androidDeviceOwner`.</span><span class="sxs-lookup"><span data-stu-id="becfe-177">Possible values are: `default`, `androidWorkProfile`, `androidDeviceOwner`.</span></span>|



## <a name="response"></a><span data-ttu-id="becfe-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="becfe-178">Response</span></span>
<span data-ttu-id="becfe-179">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="becfe-179">If successful, this method returns a `200 OK` response code and an updated [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="becfe-180">Exemplo</span><span class="sxs-lookup"><span data-stu-id="becfe-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="becfe-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="becfe-181">Request</span></span>
<span data-ttu-id="becfe-182">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="becfe-182">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
Content-type: application/json
Content-length: 609

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
  ],
  "profileApplicability": "androidWorkProfile"
}
```

### <a name="response"></a><span data-ttu-id="becfe-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="becfe-183">Response</span></span>
<span data-ttu-id="becfe-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="becfe-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 781

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
  ],
  "profileApplicability": "androidWorkProfile"
}
```






