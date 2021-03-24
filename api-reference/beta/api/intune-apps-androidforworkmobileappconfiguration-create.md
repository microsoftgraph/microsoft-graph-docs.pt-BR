---
title: Criar androidForWorkMobileAppConfiguration
description: Crie um novo objeto androidForWorkMobileAppConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8c243e6179d98ef4de82b954feb2a266efb2722e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51144519"
---
# <a name="create-androidforworkmobileappconfiguration"></a><span data-ttu-id="b7970-103">Criar androidForWorkMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="b7970-103">Create androidForWorkMobileAppConfiguration</span></span>

<span data-ttu-id="b7970-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7970-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b7970-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b7970-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7970-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b7970-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7970-107">Crie um novo [objeto androidForWorkMobileAppConfiguration.](../resources/intune-apps-androidforworkmobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b7970-107">Create a new [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b7970-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b7970-108">Prerequisites</span></span>
<span data-ttu-id="b7970-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7970-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7970-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b7970-111">Permission type</span></span>|<span data-ttu-id="b7970-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b7970-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7970-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b7970-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b7970-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7970-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b7970-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b7970-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7970-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b7970-116">Not supported.</span></span>|
|<span data-ttu-id="b7970-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b7970-117">Application</span></span>|<span data-ttu-id="b7970-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7970-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7970-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b7970-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b7970-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b7970-120">Request headers</span></span>
|<span data-ttu-id="b7970-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b7970-121">Header</span></span>|<span data-ttu-id="b7970-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b7970-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7970-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b7970-123">Authorization</span></span>|<span data-ttu-id="b7970-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b7970-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7970-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b7970-125">Accept</span></span>|<span data-ttu-id="b7970-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b7970-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7970-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b7970-127">Request body</span></span>
<span data-ttu-id="b7970-128">No corpo da solicitação, fornece uma representação JSON para o objeto androidForWorkMobileAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="b7970-128">In the request body, supply a JSON representation for the androidForWorkMobileAppConfiguration object.</span></span>

<span data-ttu-id="b7970-129">A tabela a seguir mostra as propriedades necessárias ao criar o androidForWorkMobileAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="b7970-129">The following table shows the properties that are required when you create the androidForWorkMobileAppConfiguration.</span></span>

|<span data-ttu-id="b7970-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b7970-130">Property</span></span>|<span data-ttu-id="b7970-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b7970-131">Type</span></span>|<span data-ttu-id="b7970-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7970-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7970-133">id</span><span class="sxs-lookup"><span data-stu-id="b7970-133">id</span></span>|<span data-ttu-id="b7970-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b7970-134">String</span></span>|<span data-ttu-id="b7970-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b7970-135">Key of the entity.</span></span> <span data-ttu-id="b7970-136">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b7970-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b7970-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="b7970-137">targetedMobileApps</span></span>|<span data-ttu-id="b7970-138">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b7970-138">String collection</span></span>|<span data-ttu-id="b7970-139">o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="b7970-139">the associated app.</span></span> <span data-ttu-id="b7970-140">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b7970-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b7970-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b7970-141">roleScopeTagIds</span></span>|<span data-ttu-id="b7970-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b7970-142">String collection</span></span>|<span data-ttu-id="b7970-143">Lista de Marcas de Escopo para esta entidade de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b7970-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="b7970-144">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b7970-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b7970-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b7970-145">createdDateTime</span></span>|<span data-ttu-id="b7970-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b7970-146">DateTimeOffset</span></span>|<span data-ttu-id="b7970-147">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="b7970-147">DateTime the object was created.</span></span> <span data-ttu-id="b7970-148">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b7970-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b7970-149">descrição</span><span class="sxs-lookup"><span data-stu-id="b7970-149">description</span></span>|<span data-ttu-id="b7970-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b7970-150">String</span></span>|<span data-ttu-id="b7970-151">Descrição fornecida pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b7970-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b7970-152">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b7970-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b7970-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b7970-153">lastModifiedDateTime</span></span>|<span data-ttu-id="b7970-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b7970-154">DateTimeOffset</span></span>|<span data-ttu-id="b7970-155">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="b7970-155">DateTime the object was last modified.</span></span> <span data-ttu-id="b7970-156">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b7970-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b7970-157">displayName</span><span class="sxs-lookup"><span data-stu-id="b7970-157">displayName</span></span>|<span data-ttu-id="b7970-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b7970-158">String</span></span>|<span data-ttu-id="b7970-159">Nome fornecido pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b7970-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b7970-160">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b7970-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b7970-161">version</span><span class="sxs-lookup"><span data-stu-id="b7970-161">version</span></span>|<span data-ttu-id="b7970-162">Int32</span><span class="sxs-lookup"><span data-stu-id="b7970-162">Int32</span></span>|<span data-ttu-id="b7970-163">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b7970-163">Version of the device configuration.</span></span> <span data-ttu-id="b7970-164">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b7970-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b7970-165">packageId</span><span class="sxs-lookup"><span data-stu-id="b7970-165">packageId</span></span>|<span data-ttu-id="b7970-166">String</span><span class="sxs-lookup"><span data-stu-id="b7970-166">String</span></span>|<span data-ttu-id="b7970-167">ID do pacote de configuração do aplicativo Android For Work.</span><span class="sxs-lookup"><span data-stu-id="b7970-167">Android For Work app configuration package id.</span></span>|
|<span data-ttu-id="b7970-168">payloadJson</span><span class="sxs-lookup"><span data-stu-id="b7970-168">payloadJson</span></span>|<span data-ttu-id="b7970-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b7970-169">String</span></span>|<span data-ttu-id="b7970-170">Carregamento JSON de configuração do aplicativo Android For Work.</span><span class="sxs-lookup"><span data-stu-id="b7970-170">Android For Work app configuration JSON payload.</span></span>|
|<span data-ttu-id="b7970-171">permissionActions</span><span class="sxs-lookup"><span data-stu-id="b7970-171">permissionActions</span></span>|<span data-ttu-id="b7970-172">[Coleção androidPermissionAction](../resources/intune-apps-androidpermissionaction.md)</span><span class="sxs-lookup"><span data-stu-id="b7970-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="b7970-173">Lista de permissões de aplicativo Android e ações de permissão correspondentes.</span><span class="sxs-lookup"><span data-stu-id="b7970-173">List of Android app permissions and corresponding permission actions.</span></span>|
|<span data-ttu-id="b7970-174">profileApplicability</span><span class="sxs-lookup"><span data-stu-id="b7970-174">profileApplicability</span></span>|[<span data-ttu-id="b7970-175">androidProfileApplicability</span><span class="sxs-lookup"><span data-stu-id="b7970-175">androidProfileApplicability</span></span>](../resources/intune-apps-androidprofileapplicability.md)|<span data-ttu-id="b7970-176">Aplicabilidade de perfil do Android Enterprise (AndroidWorkProfile, DeviceOwner ou padrão (aplica-se a ambos)).</span><span class="sxs-lookup"><span data-stu-id="b7970-176">Android Enterprise profile applicability (AndroidWorkProfile, DeviceOwner, or default (applies to both)).</span></span> <span data-ttu-id="b7970-177">Os valores possíveis são: `default`, `androidWorkProfile`, `androidDeviceOwner`.</span><span class="sxs-lookup"><span data-stu-id="b7970-177">Possible values are: `default`, `androidWorkProfile`, `androidDeviceOwner`.</span></span>|



## <a name="response"></a><span data-ttu-id="b7970-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7970-178">Response</span></span>
<span data-ttu-id="b7970-179">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b7970-179">If successful, this method returns a `201 Created` response code and a [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7970-180">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b7970-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="b7970-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b7970-181">Request</span></span>
<span data-ttu-id="b7970-182">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b7970-182">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b7970-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7970-183">Response</span></span>
<span data-ttu-id="b7970-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b7970-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




