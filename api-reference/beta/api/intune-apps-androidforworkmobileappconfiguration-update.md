---
title: Atualizar androidForWorkMobileAppConfiguration
description: Atualiza as propriedades de um objeto androidForWorkMobileAppConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1dac2dfd25df66b6f73963a4523a1b6d1f374f84
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49253912"
---
# <a name="update-androidforworkmobileappconfiguration"></a><span data-ttu-id="4a567-103">Atualizar androidForWorkMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="4a567-103">Update androidForWorkMobileAppConfiguration</span></span>

<span data-ttu-id="4a567-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a567-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4a567-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4a567-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a567-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4a567-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a567-107">Atualiza as propriedades de um objeto [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="4a567-107">Update the properties of a [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4a567-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4a567-108">Prerequisites</span></span>
<span data-ttu-id="4a567-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a567-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a567-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4a567-111">Permission type</span></span>|<span data-ttu-id="4a567-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4a567-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a567-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4a567-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4a567-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a567-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4a567-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4a567-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a567-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4a567-116">Not supported.</span></span>|
|<span data-ttu-id="4a567-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4a567-117">Application</span></span>|<span data-ttu-id="4a567-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a567-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a567-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4a567-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="4a567-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4a567-120">Request headers</span></span>
|<span data-ttu-id="4a567-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4a567-121">Header</span></span>|<span data-ttu-id="4a567-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4a567-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a567-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4a567-123">Authorization</span></span>|<span data-ttu-id="4a567-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4a567-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a567-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4a567-125">Accept</span></span>|<span data-ttu-id="4a567-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4a567-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a567-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4a567-127">Request body</span></span>
<span data-ttu-id="4a567-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="4a567-128">In the request body, supply a JSON representation for the [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object.</span></span>

<span data-ttu-id="4a567-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4a567-129">The following table shows the properties that are required when you create the [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md).</span></span>

|<span data-ttu-id="4a567-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4a567-130">Property</span></span>|<span data-ttu-id="4a567-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a567-131">Type</span></span>|<span data-ttu-id="4a567-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a567-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a567-133">id</span><span class="sxs-lookup"><span data-stu-id="4a567-133">id</span></span>|<span data-ttu-id="4a567-134">String</span><span class="sxs-lookup"><span data-stu-id="4a567-134">String</span></span>|<span data-ttu-id="4a567-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4a567-135">Key of the entity.</span></span> <span data-ttu-id="4a567-136">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4a567-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="4a567-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="4a567-137">targetedMobileApps</span></span>|<span data-ttu-id="4a567-138">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a567-138">String collection</span></span>|<span data-ttu-id="4a567-139">o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="4a567-139">the associated app.</span></span> <span data-ttu-id="4a567-140">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4a567-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="4a567-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4a567-141">roleScopeTagIds</span></span>|<span data-ttu-id="4a567-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a567-142">String collection</span></span>|<span data-ttu-id="4a567-143">Lista de marcas de escopo para esta entidade de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4a567-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="4a567-144">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4a567-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="4a567-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4a567-145">createdDateTime</span></span>|<span data-ttu-id="4a567-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a567-146">DateTimeOffset</span></span>|<span data-ttu-id="4a567-147">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="4a567-147">DateTime the object was created.</span></span> <span data-ttu-id="4a567-148">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4a567-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="4a567-149">description</span><span class="sxs-lookup"><span data-stu-id="4a567-149">description</span></span>|<span data-ttu-id="4a567-150">String</span><span class="sxs-lookup"><span data-stu-id="4a567-150">String</span></span>|<span data-ttu-id="4a567-151">Descrição fornecida pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4a567-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4a567-152">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4a567-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="4a567-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4a567-153">lastModifiedDateTime</span></span>|<span data-ttu-id="4a567-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a567-154">DateTimeOffset</span></span>|<span data-ttu-id="4a567-155">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="4a567-155">DateTime the object was last modified.</span></span> <span data-ttu-id="4a567-156">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4a567-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="4a567-157">displayName</span><span class="sxs-lookup"><span data-stu-id="4a567-157">displayName</span></span>|<span data-ttu-id="4a567-158">String</span><span class="sxs-lookup"><span data-stu-id="4a567-158">String</span></span>|<span data-ttu-id="4a567-159">Nome fornecido pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4a567-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4a567-160">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4a567-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="4a567-161">version</span><span class="sxs-lookup"><span data-stu-id="4a567-161">version</span></span>|<span data-ttu-id="4a567-162">Int32</span><span class="sxs-lookup"><span data-stu-id="4a567-162">Int32</span></span>|<span data-ttu-id="4a567-163">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4a567-163">Version of the device configuration.</span></span> <span data-ttu-id="4a567-164">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4a567-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="4a567-165">packageId</span><span class="sxs-lookup"><span data-stu-id="4a567-165">packageId</span></span>|<span data-ttu-id="4a567-166">String</span><span class="sxs-lookup"><span data-stu-id="4a567-166">String</span></span>|<span data-ttu-id="4a567-167">ID do pacote de configuração do aplicativo Android for Work.</span><span class="sxs-lookup"><span data-stu-id="4a567-167">Android For Work app configuration package id.</span></span>|
|<span data-ttu-id="4a567-168">payloadJson</span><span class="sxs-lookup"><span data-stu-id="4a567-168">payloadJson</span></span>|<span data-ttu-id="4a567-169">String</span><span class="sxs-lookup"><span data-stu-id="4a567-169">String</span></span>|<span data-ttu-id="4a567-170">Carga JSON da configuração de aplicativo do Android for Work.</span><span class="sxs-lookup"><span data-stu-id="4a567-170">Android For Work app configuration JSON payload.</span></span>|
|<span data-ttu-id="4a567-171">permissionActions</span><span class="sxs-lookup"><span data-stu-id="4a567-171">permissionActions</span></span>|<span data-ttu-id="4a567-172">coleção [androidPermissionAction](../resources/intune-apps-androidpermissionaction.md)</span><span class="sxs-lookup"><span data-stu-id="4a567-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="4a567-173">Lista de permissões de aplicativo Android e ações de permissão correspondentes.</span><span class="sxs-lookup"><span data-stu-id="4a567-173">List of Android app permissions and corresponding permission actions.</span></span>|
|<span data-ttu-id="4a567-174">profileApplicability</span><span class="sxs-lookup"><span data-stu-id="4a567-174">profileApplicability</span></span>|[<span data-ttu-id="4a567-175">androidProfileApplicability</span><span class="sxs-lookup"><span data-stu-id="4a567-175">androidProfileApplicability</span></span>](../resources/intune-apps-androidprofileapplicability.md)|<span data-ttu-id="4a567-176">Aplicabilidade de perfil corporativo Android (AndroidWorkProfile, DeviceOwner ou default (aplica-se a ambos)).</span><span class="sxs-lookup"><span data-stu-id="4a567-176">Android Enterprise profile applicability (AndroidWorkProfile, DeviceOwner, or default (applies to both)).</span></span> <span data-ttu-id="4a567-177">Os valores possíveis são: `default`, `androidWorkProfile`, `androidDeviceOwner`.</span><span class="sxs-lookup"><span data-stu-id="4a567-177">Possible values are: `default`, `androidWorkProfile`, `androidDeviceOwner`.</span></span>|



## <a name="response"></a><span data-ttu-id="4a567-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a567-178">Response</span></span>
<span data-ttu-id="4a567-179">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4a567-179">If successful, this method returns a `200 OK` response code and an updated [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a567-180">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4a567-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a567-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4a567-181">Request</span></span>
<span data-ttu-id="4a567-182">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4a567-182">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4a567-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a567-183">Response</span></span>
<span data-ttu-id="4a567-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4a567-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




