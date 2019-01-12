---
title: Atualizar androidForWorkMobileAppConfiguration
description: Atualize as propriedades de um objeto androidForWorkMobileAppConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 20f28ee3268e8e05563d1ed67d3dbe30e82cb801
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964890"
---
# <a name="update-androidforworkmobileappconfiguration"></a><span data-ttu-id="4f6d0-103">Atualizar androidForWorkMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="4f6d0-103">Update androidForWorkMobileAppConfiguration</span></span>

> <span data-ttu-id="4f6d0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4f6d0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4f6d0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4f6d0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4f6d0-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4f6d0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4f6d0-107">Atualize as propriedades de um objeto [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="4f6d0-107">Update the properties of a [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4f6d0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4f6d0-108">Prerequisites</span></span>
<span data-ttu-id="4f6d0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f6d0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f6d0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4f6d0-111">Permission type</span></span>|<span data-ttu-id="4f6d0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4f6d0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f6d0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4f6d0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4f6d0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f6d0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4f6d0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4f6d0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f6d0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f6d0-116">Not supported.</span></span>|
|<span data-ttu-id="4f6d0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4f6d0-117">Application</span></span>|<span data-ttu-id="4f6d0-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f6d0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f6d0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4f6d0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="4f6d0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4f6d0-120">Request headers</span></span>
|<span data-ttu-id="4f6d0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4f6d0-121">Header</span></span>|<span data-ttu-id="4f6d0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4f6d0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f6d0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4f6d0-123">Authorization</span></span>|<span data-ttu-id="4f6d0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4f6d0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f6d0-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4f6d0-125">Accept</span></span>|<span data-ttu-id="4f6d0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4f6d0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f6d0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4f6d0-127">Request body</span></span>
<span data-ttu-id="4f6d0-128">No corpo da solicitação, fornece uma representação JSON para o objeto [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="4f6d0-128">In the request body, supply a JSON representation for the [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object.</span></span>

<span data-ttu-id="4f6d0-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4f6d0-129">The following table shows the properties that are required when you create the [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md).</span></span>

|<span data-ttu-id="4f6d0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4f6d0-130">Property</span></span>|<span data-ttu-id="4f6d0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4f6d0-131">Type</span></span>|<span data-ttu-id="4f6d0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f6d0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f6d0-133">id</span><span class="sxs-lookup"><span data-stu-id="4f6d0-133">id</span></span>|<span data-ttu-id="4f6d0-134">String</span><span class="sxs-lookup"><span data-stu-id="4f6d0-134">String</span></span>|<span data-ttu-id="4f6d0-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4f6d0-135">Key of the entity.</span></span> <span data-ttu-id="4f6d0-136">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f6d0-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="4f6d0-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="4f6d0-137">targetedMobileApps</span></span>|<span data-ttu-id="4f6d0-138">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4f6d0-138">String collection</span></span>|<span data-ttu-id="4f6d0-139">o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="4f6d0-139">the associated app.</span></span> <span data-ttu-id="4f6d0-140">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f6d0-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="4f6d0-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4f6d0-141">roleScopeTagIds</span></span>|<span data-ttu-id="4f6d0-142">String collection</span><span class="sxs-lookup"><span data-stu-id="4f6d0-142">String collection</span></span>|<span data-ttu-id="4f6d0-143">Lista de escopo marcas para essa entidade de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4f6d0-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="4f6d0-144">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f6d0-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="4f6d0-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4f6d0-145">createdDateTime</span></span>|<span data-ttu-id="4f6d0-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f6d0-146">DateTimeOffset</span></span>|<span data-ttu-id="4f6d0-147">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="4f6d0-147">DateTime the object was created.</span></span> <span data-ttu-id="4f6d0-148">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f6d0-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="4f6d0-149">description</span><span class="sxs-lookup"><span data-stu-id="4f6d0-149">description</span></span>|<span data-ttu-id="4f6d0-150">String</span><span class="sxs-lookup"><span data-stu-id="4f6d0-150">String</span></span>|<span data-ttu-id="4f6d0-151">Descrição fornecida pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4f6d0-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4f6d0-152">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f6d0-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="4f6d0-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4f6d0-153">lastModifiedDateTime</span></span>|<span data-ttu-id="4f6d0-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f6d0-154">DateTimeOffset</span></span>|<span data-ttu-id="4f6d0-155">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="4f6d0-155">DateTime the object was last modified.</span></span> <span data-ttu-id="4f6d0-156">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f6d0-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="4f6d0-157">displayName</span><span class="sxs-lookup"><span data-stu-id="4f6d0-157">displayName</span></span>|<span data-ttu-id="4f6d0-158">String</span><span class="sxs-lookup"><span data-stu-id="4f6d0-158">String</span></span>|<span data-ttu-id="4f6d0-159">Nome fornecido pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4f6d0-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4f6d0-160">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f6d0-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="4f6d0-161">version</span><span class="sxs-lookup"><span data-stu-id="4f6d0-161">version</span></span>|<span data-ttu-id="4f6d0-162">Int32</span><span class="sxs-lookup"><span data-stu-id="4f6d0-162">Int32</span></span>|<span data-ttu-id="4f6d0-163">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4f6d0-163">Version of the device configuration.</span></span> <span data-ttu-id="4f6d0-164">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f6d0-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="4f6d0-165">packageId</span><span class="sxs-lookup"><span data-stu-id="4f6d0-165">packageId</span></span>|<span data-ttu-id="4f6d0-166">String</span><span class="sxs-lookup"><span data-stu-id="4f6d0-166">String</span></span>|<span data-ttu-id="4f6d0-167">Id do pacote de configuração de aplicativo de Android para trabalho.</span><span class="sxs-lookup"><span data-stu-id="4f6d0-167">Android For Work app configuration package id.</span></span>|
|<span data-ttu-id="4f6d0-168">payloadJson</span><span class="sxs-lookup"><span data-stu-id="4f6d0-168">payloadJson</span></span>|<span data-ttu-id="4f6d0-169">String</span><span class="sxs-lookup"><span data-stu-id="4f6d0-169">String</span></span>|<span data-ttu-id="4f6d0-170">Carga JSON de configuração de aplicativo Android para trabalho.</span><span class="sxs-lookup"><span data-stu-id="4f6d0-170">Android For Work app configuration JSON payload.</span></span>|
|<span data-ttu-id="4f6d0-171">permissionActions</span><span class="sxs-lookup"><span data-stu-id="4f6d0-171">permissionActions</span></span>|<span data-ttu-id="4f6d0-172">coleção [androidPermissionAction](../resources/intune-apps-androidpermissionaction.md)</span><span class="sxs-lookup"><span data-stu-id="4f6d0-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="4f6d0-173">Lista de permissões do aplicativo Android e ações correspondentes de permissão.</span><span class="sxs-lookup"><span data-stu-id="4f6d0-173">List of Android app permissions and corresponding permission actions.</span></span>|



## <a name="response"></a><span data-ttu-id="4f6d0-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f6d0-174">Response</span></span>
<span data-ttu-id="4f6d0-175">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4f6d0-175">If successful, this method returns a `200 OK` response code and an updated [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f6d0-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4f6d0-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="4f6d0-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4f6d0-177">Request</span></span>
<span data-ttu-id="4f6d0-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4f6d0-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
Content-type: application/json
Content-length: 549

{
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

### <a name="response"></a><span data-ttu-id="4f6d0-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f6d0-179">Response</span></span>
<span data-ttu-id="4f6d0-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4f6d0-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





