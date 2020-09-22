---
title: Criar androidForWorkMobileAppConfiguration
description: Criar um novo objeto androidForWorkMobileAppConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4be8c6c6045e8050aa59fc081a7aa261145ef4cd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48006500"
---
# <a name="create-androidforworkmobileappconfiguration"></a><span data-ttu-id="5032c-103">Criar androidForWorkMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="5032c-103">Create androidForWorkMobileAppConfiguration</span></span>

<span data-ttu-id="5032c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5032c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5032c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5032c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5032c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5032c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5032c-107">Criar um novo objeto [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="5032c-107">Create a new [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5032c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5032c-108">Prerequisites</span></span>
<span data-ttu-id="5032c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5032c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5032c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5032c-111">Permission type</span></span>|<span data-ttu-id="5032c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5032c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5032c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5032c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5032c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5032c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5032c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5032c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5032c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5032c-116">Not supported.</span></span>|
|<span data-ttu-id="5032c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5032c-117">Application</span></span>|<span data-ttu-id="5032c-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5032c-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5032c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5032c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5032c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5032c-120">Request headers</span></span>
|<span data-ttu-id="5032c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5032c-121">Header</span></span>|<span data-ttu-id="5032c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5032c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5032c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5032c-123">Authorization</span></span>|<span data-ttu-id="5032c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5032c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5032c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5032c-125">Accept</span></span>|<span data-ttu-id="5032c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5032c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5032c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5032c-127">Request body</span></span>
<span data-ttu-id="5032c-128">No corpo da solicitação, forneça uma representação JSON do objeto androidForWorkMobileAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="5032c-128">In the request body, supply a JSON representation for the androidForWorkMobileAppConfiguration object.</span></span>

<span data-ttu-id="5032c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar androidForWorkMobileAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="5032c-129">The following table shows the properties that are required when you create the androidForWorkMobileAppConfiguration.</span></span>

|<span data-ttu-id="5032c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5032c-130">Property</span></span>|<span data-ttu-id="5032c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5032c-131">Type</span></span>|<span data-ttu-id="5032c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5032c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5032c-133">id</span><span class="sxs-lookup"><span data-stu-id="5032c-133">id</span></span>|<span data-ttu-id="5032c-134">String</span><span class="sxs-lookup"><span data-stu-id="5032c-134">String</span></span>|<span data-ttu-id="5032c-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5032c-135">Key of the entity.</span></span> <span data-ttu-id="5032c-136">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5032c-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5032c-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="5032c-137">targetedMobileApps</span></span>|<span data-ttu-id="5032c-138">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5032c-138">String collection</span></span>|<span data-ttu-id="5032c-139">o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="5032c-139">the associated app.</span></span> <span data-ttu-id="5032c-140">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5032c-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5032c-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5032c-141">roleScopeTagIds</span></span>|<span data-ttu-id="5032c-142">String collection</span><span class="sxs-lookup"><span data-stu-id="5032c-142">String collection</span></span>|<span data-ttu-id="5032c-143">Lista de marcas de escopo para esta entidade de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5032c-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="5032c-144">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5032c-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5032c-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5032c-145">createdDateTime</span></span>|<span data-ttu-id="5032c-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5032c-146">DateTimeOffset</span></span>|<span data-ttu-id="5032c-147">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="5032c-147">DateTime the object was created.</span></span> <span data-ttu-id="5032c-148">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5032c-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5032c-149">description</span><span class="sxs-lookup"><span data-stu-id="5032c-149">description</span></span>|<span data-ttu-id="5032c-150">String</span><span class="sxs-lookup"><span data-stu-id="5032c-150">String</span></span>|<span data-ttu-id="5032c-151">Descrição fornecida pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5032c-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5032c-152">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5032c-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5032c-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5032c-153">lastModifiedDateTime</span></span>|<span data-ttu-id="5032c-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5032c-154">DateTimeOffset</span></span>|<span data-ttu-id="5032c-155">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="5032c-155">DateTime the object was last modified.</span></span> <span data-ttu-id="5032c-156">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5032c-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5032c-157">displayName</span><span class="sxs-lookup"><span data-stu-id="5032c-157">displayName</span></span>|<span data-ttu-id="5032c-158">String</span><span class="sxs-lookup"><span data-stu-id="5032c-158">String</span></span>|<span data-ttu-id="5032c-159">Nome fornecido pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5032c-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5032c-160">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5032c-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5032c-161">version</span><span class="sxs-lookup"><span data-stu-id="5032c-161">version</span></span>|<span data-ttu-id="5032c-162">Int32</span><span class="sxs-lookup"><span data-stu-id="5032c-162">Int32</span></span>|<span data-ttu-id="5032c-163">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5032c-163">Version of the device configuration.</span></span> <span data-ttu-id="5032c-164">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5032c-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5032c-165">packageId</span><span class="sxs-lookup"><span data-stu-id="5032c-165">packageId</span></span>|<span data-ttu-id="5032c-166">String</span><span class="sxs-lookup"><span data-stu-id="5032c-166">String</span></span>|<span data-ttu-id="5032c-167">ID do pacote de configuração do aplicativo Android for Work.</span><span class="sxs-lookup"><span data-stu-id="5032c-167">Android For Work app configuration package id.</span></span>|
|<span data-ttu-id="5032c-168">payloadJson</span><span class="sxs-lookup"><span data-stu-id="5032c-168">payloadJson</span></span>|<span data-ttu-id="5032c-169">String</span><span class="sxs-lookup"><span data-stu-id="5032c-169">String</span></span>|<span data-ttu-id="5032c-170">Carga JSON da configuração de aplicativo do Android for Work.</span><span class="sxs-lookup"><span data-stu-id="5032c-170">Android For Work app configuration JSON payload.</span></span>|
|<span data-ttu-id="5032c-171">permissionActions</span><span class="sxs-lookup"><span data-stu-id="5032c-171">permissionActions</span></span>|<span data-ttu-id="5032c-172">coleção [androidPermissionAction](../resources/intune-apps-androidpermissionaction.md)</span><span class="sxs-lookup"><span data-stu-id="5032c-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="5032c-173">Lista de permissões de aplicativo Android e ações de permissão correspondentes.</span><span class="sxs-lookup"><span data-stu-id="5032c-173">List of Android app permissions and corresponding permission actions.</span></span>|
|<span data-ttu-id="5032c-174">profileApplicability</span><span class="sxs-lookup"><span data-stu-id="5032c-174">profileApplicability</span></span>|[<span data-ttu-id="5032c-175">androidProfileApplicability</span><span class="sxs-lookup"><span data-stu-id="5032c-175">androidProfileApplicability</span></span>](../resources/intune-apps-androidprofileapplicability.md)|<span data-ttu-id="5032c-176">Aplicabilidade de perfil corporativo Android (AndroidWorkProfile, DeviceOwner ou default (aplica-se a ambos)).</span><span class="sxs-lookup"><span data-stu-id="5032c-176">Android Enterprise profile applicability (AndroidWorkProfile, DeviceOwner, or default (applies to both)).</span></span> <span data-ttu-id="5032c-177">Os valores possíveis são: `default`, `androidWorkProfile`, `androidDeviceOwner`.</span><span class="sxs-lookup"><span data-stu-id="5032c-177">Possible values are: `default`, `androidWorkProfile`, `androidDeviceOwner`.</span></span>|



## <a name="response"></a><span data-ttu-id="5032c-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="5032c-178">Response</span></span>
<span data-ttu-id="5032c-179">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5032c-179">If successful, this method returns a `201 Created` response code and a [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5032c-180">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5032c-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="5032c-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5032c-181">Request</span></span>
<span data-ttu-id="5032c-182">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5032c-182">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations
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

### <a name="response"></a><span data-ttu-id="5032c-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="5032c-183">Response</span></span>
<span data-ttu-id="5032c-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5032c-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






