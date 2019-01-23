---
title: Criar androidForWorkMobileAppConfiguration
description: Crie um novo objeto de androidForWorkMobileAppConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bbe57c72e4b00a6e289934e7503c862ad3db5d4a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414141"
---
# <a name="create-androidforworkmobileappconfiguration"></a><span data-ttu-id="2872f-103">Criar androidForWorkMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="2872f-103">Create androidForWorkMobileAppConfiguration</span></span>

> <span data-ttu-id="2872f-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="2872f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2872f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2872f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2872f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="2872f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2872f-107">Crie um novo objeto de [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="2872f-107">Create a new [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2872f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2872f-108">Prerequisites</span></span>
<span data-ttu-id="2872f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2872f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2872f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2872f-111">Permission type</span></span>|<span data-ttu-id="2872f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2872f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2872f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2872f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2872f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2872f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2872f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2872f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2872f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2872f-116">Not supported.</span></span>|
|<span data-ttu-id="2872f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2872f-117">Application</span></span>|<span data-ttu-id="2872f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2872f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2872f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2872f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2872f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2872f-120">Request headers</span></span>
|<span data-ttu-id="2872f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2872f-121">Header</span></span>|<span data-ttu-id="2872f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2872f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2872f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2872f-123">Authorization</span></span>|<span data-ttu-id="2872f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2872f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2872f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2872f-125">Accept</span></span>|<span data-ttu-id="2872f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2872f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2872f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2872f-127">Request body</span></span>
<span data-ttu-id="2872f-128">No corpo da solicitação, fornece uma representação JSON para o objeto androidForWorkMobileAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="2872f-128">In the request body, supply a JSON representation for the androidForWorkMobileAppConfiguration object.</span></span>

<span data-ttu-id="2872f-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o androidForWorkMobileAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="2872f-129">The following table shows the properties that are required when you create the androidForWorkMobileAppConfiguration.</span></span>

|<span data-ttu-id="2872f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2872f-130">Property</span></span>|<span data-ttu-id="2872f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2872f-131">Type</span></span>|<span data-ttu-id="2872f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2872f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2872f-133">id</span><span class="sxs-lookup"><span data-stu-id="2872f-133">id</span></span>|<span data-ttu-id="2872f-134">String</span><span class="sxs-lookup"><span data-stu-id="2872f-134">String</span></span>|<span data-ttu-id="2872f-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2872f-135">Key of the entity.</span></span> <span data-ttu-id="2872f-136">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2872f-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="2872f-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="2872f-137">targetedMobileApps</span></span>|<span data-ttu-id="2872f-138">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2872f-138">String collection</span></span>|<span data-ttu-id="2872f-139">o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="2872f-139">the associated app.</span></span> <span data-ttu-id="2872f-140">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2872f-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="2872f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2872f-141">roleScopeTagIds</span></span>|<span data-ttu-id="2872f-142">String collection</span><span class="sxs-lookup"><span data-stu-id="2872f-142">String collection</span></span>|<span data-ttu-id="2872f-143">Lista de escopo marcas para essa entidade de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2872f-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="2872f-144">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2872f-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="2872f-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2872f-145">createdDateTime</span></span>|<span data-ttu-id="2872f-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2872f-146">DateTimeOffset</span></span>|<span data-ttu-id="2872f-147">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="2872f-147">DateTime the object was created.</span></span> <span data-ttu-id="2872f-148">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2872f-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="2872f-149">description</span><span class="sxs-lookup"><span data-stu-id="2872f-149">description</span></span>|<span data-ttu-id="2872f-150">String</span><span class="sxs-lookup"><span data-stu-id="2872f-150">String</span></span>|<span data-ttu-id="2872f-151">Descrição fornecida pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2872f-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2872f-152">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2872f-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="2872f-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2872f-153">lastModifiedDateTime</span></span>|<span data-ttu-id="2872f-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2872f-154">DateTimeOffset</span></span>|<span data-ttu-id="2872f-155">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="2872f-155">DateTime the object was last modified.</span></span> <span data-ttu-id="2872f-156">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2872f-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="2872f-157">displayName</span><span class="sxs-lookup"><span data-stu-id="2872f-157">displayName</span></span>|<span data-ttu-id="2872f-158">String</span><span class="sxs-lookup"><span data-stu-id="2872f-158">String</span></span>|<span data-ttu-id="2872f-159">Nome fornecido pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2872f-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2872f-160">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2872f-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="2872f-161">version</span><span class="sxs-lookup"><span data-stu-id="2872f-161">version</span></span>|<span data-ttu-id="2872f-162">Int32</span><span class="sxs-lookup"><span data-stu-id="2872f-162">Int32</span></span>|<span data-ttu-id="2872f-163">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2872f-163">Version of the device configuration.</span></span> <span data-ttu-id="2872f-164">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2872f-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="2872f-165">packageId</span><span class="sxs-lookup"><span data-stu-id="2872f-165">packageId</span></span>|<span data-ttu-id="2872f-166">String</span><span class="sxs-lookup"><span data-stu-id="2872f-166">String</span></span>|<span data-ttu-id="2872f-167">Id do pacote de configuração de aplicativo de Android para trabalho.</span><span class="sxs-lookup"><span data-stu-id="2872f-167">Android For Work app configuration package id.</span></span>|
|<span data-ttu-id="2872f-168">payloadJson</span><span class="sxs-lookup"><span data-stu-id="2872f-168">payloadJson</span></span>|<span data-ttu-id="2872f-169">String</span><span class="sxs-lookup"><span data-stu-id="2872f-169">String</span></span>|<span data-ttu-id="2872f-170">Carga JSON de configuração de aplicativo Android para trabalho.</span><span class="sxs-lookup"><span data-stu-id="2872f-170">Android For Work app configuration JSON payload.</span></span>|
|<span data-ttu-id="2872f-171">permissionActions</span><span class="sxs-lookup"><span data-stu-id="2872f-171">permissionActions</span></span>|<span data-ttu-id="2872f-172">coleção [androidPermissionAction](../resources/intune-apps-androidpermissionaction.md)</span><span class="sxs-lookup"><span data-stu-id="2872f-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="2872f-173">Lista de permissões do aplicativo Android e ações correspondentes de permissão.</span><span class="sxs-lookup"><span data-stu-id="2872f-173">List of Android app permissions and corresponding permission actions.</span></span>|



## <a name="response"></a><span data-ttu-id="2872f-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="2872f-174">Response</span></span>
<span data-ttu-id="2872f-175">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2872f-175">If successful, this method returns a `201 Created` response code and a [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2872f-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2872f-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="2872f-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2872f-177">Request</span></span>
<span data-ttu-id="2872f-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2872f-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2872f-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="2872f-179">Response</span></span>
<span data-ttu-id="2872f-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2872f-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




