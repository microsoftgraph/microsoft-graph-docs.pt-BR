---
title: Criar androidForWorkMobileAppConfiguration
description: Criar um novo objeto androidForWorkMobileAppConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 15a8fb8d1b1485eae922bf302dd76fcc786a6fd3
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30958645"
---
# <a name="create-androidforworkmobileappconfiguration"></a><span data-ttu-id="a0276-103">Criar androidForWorkMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="a0276-103">Create androidForWorkMobileAppConfiguration</span></span>

> <span data-ttu-id="a0276-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a0276-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0276-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a0276-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0276-106">Criar um novo objeto [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a0276-106">Create a new [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0276-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a0276-107">Prerequisites</span></span>
<span data-ttu-id="a0276-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0276-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0276-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0276-110">Permission type</span></span>|<span data-ttu-id="a0276-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a0276-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0276-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0276-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a0276-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0276-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a0276-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0276-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0276-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0276-115">Not supported.</span></span>|
|<span data-ttu-id="a0276-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0276-116">Application</span></span>|<span data-ttu-id="a0276-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0276-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0276-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0276-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a0276-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0276-119">Request headers</span></span>
|<span data-ttu-id="a0276-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a0276-120">Header</span></span>|<span data-ttu-id="a0276-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a0276-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0276-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0276-122">Authorization</span></span>|<span data-ttu-id="a0276-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a0276-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0276-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a0276-124">Accept</span></span>|<span data-ttu-id="a0276-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a0276-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0276-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0276-126">Request body</span></span>
<span data-ttu-id="a0276-127">No corpo da solicitação, forneça uma representação JSON do objeto androidForWorkMobileAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a0276-127">In the request body, supply a JSON representation for the androidForWorkMobileAppConfiguration object.</span></span>

<span data-ttu-id="a0276-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidForWorkMobileAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a0276-128">The following table shows the properties that are required when you create the androidForWorkMobileAppConfiguration.</span></span>

|<span data-ttu-id="a0276-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a0276-129">Property</span></span>|<span data-ttu-id="a0276-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0276-130">Type</span></span>|<span data-ttu-id="a0276-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0276-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0276-132">id</span><span class="sxs-lookup"><span data-stu-id="a0276-132">id</span></span>|<span data-ttu-id="a0276-133">String</span><span class="sxs-lookup"><span data-stu-id="a0276-133">String</span></span>|<span data-ttu-id="a0276-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a0276-134">Key of the entity.</span></span> <span data-ttu-id="a0276-135">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0276-135">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="a0276-136">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="a0276-136">targetedMobileApps</span></span>|<span data-ttu-id="a0276-137">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0276-137">String collection</span></span>|<span data-ttu-id="a0276-138">o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="a0276-138">the associated app.</span></span> <span data-ttu-id="a0276-139">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0276-139">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="a0276-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a0276-140">roleScopeTagIds</span></span>|<span data-ttu-id="a0276-141">Coleção String</span><span class="sxs-lookup"><span data-stu-id="a0276-141">String collection</span></span>|<span data-ttu-id="a0276-142">Lista de marcas de escopo para esta entidade de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a0276-142">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="a0276-143">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0276-143">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="a0276-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a0276-144">createdDateTime</span></span>|<span data-ttu-id="a0276-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0276-145">DateTimeOffset</span></span>|<span data-ttu-id="a0276-146">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="a0276-146">DateTime the object was created.</span></span> <span data-ttu-id="a0276-147">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0276-147">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="a0276-148">descrição</span><span class="sxs-lookup"><span data-stu-id="a0276-148">description</span></span>|<span data-ttu-id="a0276-149">String</span><span class="sxs-lookup"><span data-stu-id="a0276-149">String</span></span>|<span data-ttu-id="a0276-150">Descrição fornecida pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a0276-150">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a0276-151">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0276-151">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="a0276-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a0276-152">lastModifiedDateTime</span></span>|<span data-ttu-id="a0276-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0276-153">DateTimeOffset</span></span>|<span data-ttu-id="a0276-154">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="a0276-154">DateTime the object was last modified.</span></span> <span data-ttu-id="a0276-155">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0276-155">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="a0276-156">displayName</span><span class="sxs-lookup"><span data-stu-id="a0276-156">displayName</span></span>|<span data-ttu-id="a0276-157">String</span><span class="sxs-lookup"><span data-stu-id="a0276-157">String</span></span>|<span data-ttu-id="a0276-158">Nome fornecido pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a0276-158">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a0276-159">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0276-159">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="a0276-160">version</span><span class="sxs-lookup"><span data-stu-id="a0276-160">version</span></span>|<span data-ttu-id="a0276-161">Int32</span><span class="sxs-lookup"><span data-stu-id="a0276-161">Int32</span></span>|<span data-ttu-id="a0276-162">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a0276-162">Version of the device configuration.</span></span> <span data-ttu-id="a0276-163">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0276-163">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="a0276-164">packageId</span><span class="sxs-lookup"><span data-stu-id="a0276-164">packageId</span></span>|<span data-ttu-id="a0276-165">String</span><span class="sxs-lookup"><span data-stu-id="a0276-165">String</span></span>|<span data-ttu-id="a0276-166">ID do pacote de configuração do aplicativo Android for Work.</span><span class="sxs-lookup"><span data-stu-id="a0276-166">Android For Work app configuration package id.</span></span>|
|<span data-ttu-id="a0276-167">payloadJson</span><span class="sxs-lookup"><span data-stu-id="a0276-167">payloadJson</span></span>|<span data-ttu-id="a0276-168">String</span><span class="sxs-lookup"><span data-stu-id="a0276-168">String</span></span>|<span data-ttu-id="a0276-169">Carga JSON da configuração de aplicativo do Android for Work.</span><span class="sxs-lookup"><span data-stu-id="a0276-169">Android For Work app configuration JSON payload.</span></span>|
|<span data-ttu-id="a0276-170">permissionActions</span><span class="sxs-lookup"><span data-stu-id="a0276-170">permissionActions</span></span>|<span data-ttu-id="a0276-171">coleção [androidPermissionAction](../resources/intune-apps-androidpermissionaction.md)</span><span class="sxs-lookup"><span data-stu-id="a0276-171">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="a0276-172">Lista de permissões de aplicativo Android e ações de permissão correspondentes.</span><span class="sxs-lookup"><span data-stu-id="a0276-172">List of Android app permissions and corresponding permission actions.</span></span>|



## <a name="response"></a><span data-ttu-id="a0276-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0276-173">Response</span></span>
<span data-ttu-id="a0276-174">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0276-174">If successful, this method returns a `201 Created` response code and a [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0276-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a0276-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0276-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0276-176">Request</span></span>
<span data-ttu-id="a0276-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a0276-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a0276-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0276-178">Response</span></span>
<span data-ttu-id="a0276-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a0276-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




