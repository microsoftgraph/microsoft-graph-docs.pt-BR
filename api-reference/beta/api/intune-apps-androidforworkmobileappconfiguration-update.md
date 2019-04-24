---
title: Atualizar androidForWorkMobileAppConfiguration
description: Atualiza as propriedades de um objeto androidForWorkMobileAppConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9df7c49d2a67363e3a6b4f66c6b610798ccce23c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32497476"
---
# <a name="update-androidforworkmobileappconfiguration"></a><span data-ttu-id="8a259-103">Atualizar androidForWorkMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="8a259-103">Update androidForWorkMobileAppConfiguration</span></span>

> <span data-ttu-id="8a259-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8a259-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8a259-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8a259-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a259-106">Atualiza as propriedades de um objeto [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="8a259-106">Update the properties of a [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8a259-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8a259-107">Prerequisites</span></span>
<span data-ttu-id="8a259-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a259-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a259-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8a259-110">Permission type</span></span>|<span data-ttu-id="8a259-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8a259-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a259-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8a259-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8a259-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a259-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8a259-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8a259-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a259-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a259-115">Not supported.</span></span>|
|<span data-ttu-id="8a259-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8a259-116">Application</span></span>|<span data-ttu-id="8a259-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a259-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a259-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8a259-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="8a259-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8a259-119">Request headers</span></span>
|<span data-ttu-id="8a259-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8a259-120">Header</span></span>|<span data-ttu-id="8a259-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8a259-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a259-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8a259-122">Authorization</span></span>|<span data-ttu-id="8a259-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8a259-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8a259-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8a259-124">Accept</span></span>|<span data-ttu-id="8a259-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8a259-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a259-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8a259-126">Request body</span></span>
<span data-ttu-id="8a259-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="8a259-127">In the request body, supply a JSON representation for the [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object.</span></span>

<span data-ttu-id="8a259-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8a259-128">The following table shows the properties that are required when you create the [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md).</span></span>

|<span data-ttu-id="8a259-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8a259-129">Property</span></span>|<span data-ttu-id="8a259-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="8a259-130">Type</span></span>|<span data-ttu-id="8a259-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a259-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a259-132">id</span><span class="sxs-lookup"><span data-stu-id="8a259-132">id</span></span>|<span data-ttu-id="8a259-133">String</span><span class="sxs-lookup"><span data-stu-id="8a259-133">String</span></span>|<span data-ttu-id="8a259-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8a259-134">Key of the entity.</span></span> <span data-ttu-id="8a259-135">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8a259-135">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="8a259-136">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="8a259-136">targetedMobileApps</span></span>|<span data-ttu-id="8a259-137">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8a259-137">String collection</span></span>|<span data-ttu-id="8a259-138">o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="8a259-138">the associated app.</span></span> <span data-ttu-id="8a259-139">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8a259-139">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="8a259-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8a259-140">roleScopeTagIds</span></span>|<span data-ttu-id="8a259-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8a259-141">String collection</span></span>|<span data-ttu-id="8a259-142">Lista de marcas de escopo para esta entidade de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8a259-142">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="8a259-143">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8a259-143">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="8a259-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8a259-144">createdDateTime</span></span>|<span data-ttu-id="8a259-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a259-145">DateTimeOffset</span></span>|<span data-ttu-id="8a259-146">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="8a259-146">DateTime the object was created.</span></span> <span data-ttu-id="8a259-147">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8a259-147">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="8a259-148">description</span><span class="sxs-lookup"><span data-stu-id="8a259-148">description</span></span>|<span data-ttu-id="8a259-149">String</span><span class="sxs-lookup"><span data-stu-id="8a259-149">String</span></span>|<span data-ttu-id="8a259-150">Descrição fornecida pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8a259-150">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8a259-151">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8a259-151">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="8a259-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8a259-152">lastModifiedDateTime</span></span>|<span data-ttu-id="8a259-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a259-153">DateTimeOffset</span></span>|<span data-ttu-id="8a259-154">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="8a259-154">DateTime the object was last modified.</span></span> <span data-ttu-id="8a259-155">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8a259-155">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="8a259-156">displayName</span><span class="sxs-lookup"><span data-stu-id="8a259-156">displayName</span></span>|<span data-ttu-id="8a259-157">String</span><span class="sxs-lookup"><span data-stu-id="8a259-157">String</span></span>|<span data-ttu-id="8a259-158">Nome fornecido pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8a259-158">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8a259-159">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8a259-159">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="8a259-160">version</span><span class="sxs-lookup"><span data-stu-id="8a259-160">version</span></span>|<span data-ttu-id="8a259-161">Int32</span><span class="sxs-lookup"><span data-stu-id="8a259-161">Int32</span></span>|<span data-ttu-id="8a259-162">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8a259-162">Version of the device configuration.</span></span> <span data-ttu-id="8a259-163">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8a259-163">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="8a259-164">packageId</span><span class="sxs-lookup"><span data-stu-id="8a259-164">packageId</span></span>|<span data-ttu-id="8a259-165">String</span><span class="sxs-lookup"><span data-stu-id="8a259-165">String</span></span>|<span data-ttu-id="8a259-166">ID do pacote de configuração do aplicativo Android for Work.</span><span class="sxs-lookup"><span data-stu-id="8a259-166">Android For Work app configuration package id.</span></span>|
|<span data-ttu-id="8a259-167">payloadJson</span><span class="sxs-lookup"><span data-stu-id="8a259-167">payloadJson</span></span>|<span data-ttu-id="8a259-168">String</span><span class="sxs-lookup"><span data-stu-id="8a259-168">String</span></span>|<span data-ttu-id="8a259-169">Carga JSON da configuração de aplicativo do Android for Work.</span><span class="sxs-lookup"><span data-stu-id="8a259-169">Android For Work app configuration JSON payload.</span></span>|
|<span data-ttu-id="8a259-170">permissionActions</span><span class="sxs-lookup"><span data-stu-id="8a259-170">permissionActions</span></span>|<span data-ttu-id="8a259-171">coleção [androidPermissionAction](../resources/intune-apps-androidpermissionaction.md)</span><span class="sxs-lookup"><span data-stu-id="8a259-171">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="8a259-172">Lista de permissões de aplicativo Android e ações de permissão correspondentes.</span><span class="sxs-lookup"><span data-stu-id="8a259-172">List of Android app permissions and corresponding permission actions.</span></span>|



## <a name="response"></a><span data-ttu-id="8a259-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a259-173">Response</span></span>
<span data-ttu-id="8a259-174">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8a259-174">If successful, this method returns a `200 OK` response code and an updated [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a259-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8a259-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="8a259-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8a259-176">Request</span></span>
<span data-ttu-id="8a259-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8a259-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
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

### <a name="response"></a><span data-ttu-id="8a259-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a259-178">Response</span></span>
<span data-ttu-id="8a259-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8a259-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





