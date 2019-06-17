---
title: Atualizar androidForWorkMobileAppConfiguration
description: Atualiza as propriedades de um objeto androidForWorkMobileAppConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 27b94ddfdec232f7d3d92b81414077af255aeef9
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34966373"
---
# <a name="update-androidforworkmobileappconfiguration"></a><span data-ttu-id="5ccfc-103">Atualizar androidForWorkMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="5ccfc-103">Update androidForWorkMobileAppConfiguration</span></span>

> <span data-ttu-id="5ccfc-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5ccfc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ccfc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5ccfc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ccfc-106">Atualiza as propriedades de um objeto [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="5ccfc-106">Update the properties of a [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5ccfc-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5ccfc-107">Prerequisites</span></span>
<span data-ttu-id="5ccfc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ccfc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ccfc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ccfc-110">Permission type</span></span>|<span data-ttu-id="5ccfc-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5ccfc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ccfc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ccfc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5ccfc-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ccfc-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5ccfc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ccfc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ccfc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ccfc-115">Not supported.</span></span>|
|<span data-ttu-id="5ccfc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ccfc-116">Application</span></span>|<span data-ttu-id="5ccfc-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ccfc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ccfc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ccfc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5ccfc-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ccfc-119">Request headers</span></span>
|<span data-ttu-id="5ccfc-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5ccfc-120">Header</span></span>|<span data-ttu-id="5ccfc-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5ccfc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ccfc-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ccfc-122">Authorization</span></span>|<span data-ttu-id="5ccfc-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ccfc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ccfc-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5ccfc-124">Accept</span></span>|<span data-ttu-id="5ccfc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5ccfc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ccfc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ccfc-126">Request body</span></span>
<span data-ttu-id="5ccfc-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="5ccfc-127">In the request body, supply a JSON representation for the [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object.</span></span>

<span data-ttu-id="5ccfc-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5ccfc-128">The following table shows the properties that are required when you create the [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md).</span></span>

|<span data-ttu-id="5ccfc-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5ccfc-129">Property</span></span>|<span data-ttu-id="5ccfc-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ccfc-130">Type</span></span>|<span data-ttu-id="5ccfc-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ccfc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ccfc-132">id</span><span class="sxs-lookup"><span data-stu-id="5ccfc-132">id</span></span>|<span data-ttu-id="5ccfc-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ccfc-133">String</span></span>|<span data-ttu-id="5ccfc-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5ccfc-134">Key of the entity.</span></span> <span data-ttu-id="5ccfc-135">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ccfc-135">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5ccfc-136">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="5ccfc-136">targetedMobileApps</span></span>|<span data-ttu-id="5ccfc-137">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ccfc-137">String collection</span></span>|<span data-ttu-id="5ccfc-138">o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="5ccfc-138">the associated app.</span></span> <span data-ttu-id="5ccfc-139">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ccfc-139">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5ccfc-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5ccfc-140">roleScopeTagIds</span></span>|<span data-ttu-id="5ccfc-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ccfc-141">String collection</span></span>|<span data-ttu-id="5ccfc-142">Lista de marcas de escopo para esta entidade de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5ccfc-142">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="5ccfc-143">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ccfc-143">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5ccfc-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5ccfc-144">createdDateTime</span></span>|<span data-ttu-id="5ccfc-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ccfc-145">DateTimeOffset</span></span>|<span data-ttu-id="5ccfc-146">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="5ccfc-146">DateTime the object was created.</span></span> <span data-ttu-id="5ccfc-147">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ccfc-147">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5ccfc-148">descrição</span><span class="sxs-lookup"><span data-stu-id="5ccfc-148">description</span></span>|<span data-ttu-id="5ccfc-149">String</span><span class="sxs-lookup"><span data-stu-id="5ccfc-149">String</span></span>|<span data-ttu-id="5ccfc-150">Descrição fornecida pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5ccfc-150">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5ccfc-151">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ccfc-151">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5ccfc-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5ccfc-152">lastModifiedDateTime</span></span>|<span data-ttu-id="5ccfc-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ccfc-153">DateTimeOffset</span></span>|<span data-ttu-id="5ccfc-154">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="5ccfc-154">DateTime the object was last modified.</span></span> <span data-ttu-id="5ccfc-155">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ccfc-155">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5ccfc-156">displayName</span><span class="sxs-lookup"><span data-stu-id="5ccfc-156">displayName</span></span>|<span data-ttu-id="5ccfc-157">String</span><span class="sxs-lookup"><span data-stu-id="5ccfc-157">String</span></span>|<span data-ttu-id="5ccfc-158">Nome fornecido pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5ccfc-158">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5ccfc-159">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ccfc-159">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5ccfc-160">version</span><span class="sxs-lookup"><span data-stu-id="5ccfc-160">version</span></span>|<span data-ttu-id="5ccfc-161">Int32</span><span class="sxs-lookup"><span data-stu-id="5ccfc-161">Int32</span></span>|<span data-ttu-id="5ccfc-162">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5ccfc-162">Version of the device configuration.</span></span> <span data-ttu-id="5ccfc-163">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ccfc-163">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5ccfc-164">packageId</span><span class="sxs-lookup"><span data-stu-id="5ccfc-164">packageId</span></span>|<span data-ttu-id="5ccfc-165">String</span><span class="sxs-lookup"><span data-stu-id="5ccfc-165">String</span></span>|<span data-ttu-id="5ccfc-166">ID do pacote de configuração do aplicativo Android for Work.</span><span class="sxs-lookup"><span data-stu-id="5ccfc-166">Android For Work app configuration package id.</span></span>|
|<span data-ttu-id="5ccfc-167">payloadJson</span><span class="sxs-lookup"><span data-stu-id="5ccfc-167">payloadJson</span></span>|<span data-ttu-id="5ccfc-168">String</span><span class="sxs-lookup"><span data-stu-id="5ccfc-168">String</span></span>|<span data-ttu-id="5ccfc-169">Carga JSON da configuração de aplicativo do Android for Work.</span><span class="sxs-lookup"><span data-stu-id="5ccfc-169">Android For Work app configuration JSON payload.</span></span>|
|<span data-ttu-id="5ccfc-170">permissionActions</span><span class="sxs-lookup"><span data-stu-id="5ccfc-170">permissionActions</span></span>|<span data-ttu-id="5ccfc-171">coleção [androidPermissionAction](../resources/intune-apps-androidpermissionaction.md)</span><span class="sxs-lookup"><span data-stu-id="5ccfc-171">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="5ccfc-172">Lista de permissões de aplicativo Android e ações de permissão correspondentes.</span><span class="sxs-lookup"><span data-stu-id="5ccfc-172">List of Android app permissions and corresponding permission actions.</span></span>|



## <a name="response"></a><span data-ttu-id="5ccfc-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ccfc-173">Response</span></span>
<span data-ttu-id="5ccfc-174">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ccfc-174">If successful, this method returns a `200 OK` response code and an updated [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ccfc-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5ccfc-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ccfc-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ccfc-176">Request</span></span>
<span data-ttu-id="5ccfc-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ccfc-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5ccfc-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ccfc-178">Response</span></span>
<span data-ttu-id="5ccfc-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5ccfc-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





