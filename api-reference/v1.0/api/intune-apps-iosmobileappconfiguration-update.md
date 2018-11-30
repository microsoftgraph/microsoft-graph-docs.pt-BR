---
title: Atualizar iosMobileAppConfiguration
description: Atualiza as propriedades de um objeto iosMobileAppConfiguration.
ms.openlocfilehash: dcd89e79b2e3c3008a2ac03a3115e8d766d0f1e6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005535"
---
# <a name="update-iosmobileappconfiguration"></a><span data-ttu-id="6762d-103">Atualizar iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="6762d-103">Update iosMobileAppConfiguration</span></span>

> <span data-ttu-id="6762d-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6762d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6762d-105">Atualiza as propriedades de um objeto [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6762d-105">Update the properties of a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6762d-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6762d-106">Prerequisites</span></span>
<span data-ttu-id="6762d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6762d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6762d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6762d-109">Permission type</span></span>|<span data-ttu-id="6762d-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6762d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6762d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6762d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6762d-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6762d-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6762d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6762d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6762d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6762d-114">Not supported.</span></span>|
|<span data-ttu-id="6762d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6762d-115">Application</span></span>|<span data-ttu-id="6762d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6762d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6762d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6762d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6762d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6762d-118">Request headers</span></span>
|<span data-ttu-id="6762d-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6762d-119">Header</span></span>|<span data-ttu-id="6762d-120">Valor</span><span class="sxs-lookup"><span data-stu-id="6762d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6762d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6762d-121">Authorization</span></span>|<span data-ttu-id="6762d-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6762d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6762d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="6762d-123">Accept</span></span>|<span data-ttu-id="6762d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6762d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6762d-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6762d-125">Request body</span></span>
<span data-ttu-id="6762d-126">No corpo da solicitação, forneça uma representação JSON do objeto [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6762d-126">In the request body, supply a JSON representation for the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

<span data-ttu-id="6762d-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6762d-127">The following table shows the properties that are required when you create the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span></span>

|<span data-ttu-id="6762d-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6762d-128">Property</span></span>|<span data-ttu-id="6762d-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="6762d-129">Type</span></span>|<span data-ttu-id="6762d-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="6762d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6762d-131">id</span><span class="sxs-lookup"><span data-stu-id="6762d-131">id</span></span>|<span data-ttu-id="6762d-132">String</span><span class="sxs-lookup"><span data-stu-id="6762d-132">String</span></span>|<span data-ttu-id="6762d-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6762d-133">Key of the entity.</span></span> <span data-ttu-id="6762d-134">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6762d-134">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="6762d-135">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="6762d-135">targetedMobileApps</span></span>|<span data-ttu-id="6762d-136">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6762d-136">String collection</span></span>|<span data-ttu-id="6762d-137">o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="6762d-137">the associated app.</span></span> <span data-ttu-id="6762d-138">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6762d-138">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="6762d-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6762d-139">createdDateTime</span></span>|<span data-ttu-id="6762d-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6762d-140">DateTimeOffset</span></span>|<span data-ttu-id="6762d-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="6762d-141">DateTime the object was created.</span></span> <span data-ttu-id="6762d-142">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6762d-142">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="6762d-143">description</span><span class="sxs-lookup"><span data-stu-id="6762d-143">description</span></span>|<span data-ttu-id="6762d-144">String</span><span class="sxs-lookup"><span data-stu-id="6762d-144">String</span></span>|<span data-ttu-id="6762d-145">Descrição fornecida pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6762d-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6762d-146">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6762d-146">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="6762d-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6762d-147">lastModifiedDateTime</span></span>|<span data-ttu-id="6762d-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6762d-148">DateTimeOffset</span></span>|<span data-ttu-id="6762d-149">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="6762d-149">DateTime the object was last modified.</span></span> <span data-ttu-id="6762d-150">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6762d-150">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="6762d-151">displayName</span><span class="sxs-lookup"><span data-stu-id="6762d-151">displayName</span></span>|<span data-ttu-id="6762d-152">String</span><span class="sxs-lookup"><span data-stu-id="6762d-152">String</span></span>|<span data-ttu-id="6762d-153">Nome fornecido pelo administrador da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6762d-153">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6762d-154">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6762d-154">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="6762d-155">version</span><span class="sxs-lookup"><span data-stu-id="6762d-155">version</span></span>|<span data-ttu-id="6762d-156">Int32</span><span class="sxs-lookup"><span data-stu-id="6762d-156">Int32</span></span>|<span data-ttu-id="6762d-157">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6762d-157">Version of the device configuration.</span></span> <span data-ttu-id="6762d-158">Herdada de [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6762d-158">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="6762d-159">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="6762d-159">encodedSettingXml</span></span>|<span data-ttu-id="6762d-160">Binário</span><span class="sxs-lookup"><span data-stu-id="6762d-160">Binary</span></span>|<span data-ttu-id="6762d-161">Binário Base64 de configuração do aplicativo MDM.</span><span class="sxs-lookup"><span data-stu-id="6762d-161">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="6762d-162">configurações</span><span class="sxs-lookup"><span data-stu-id="6762d-162">settings</span></span>|<span data-ttu-id="6762d-163">Coleção de [appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md)</span><span class="sxs-lookup"><span data-stu-id="6762d-163">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="6762d-164">Itens de configuração de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6762d-164">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="6762d-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="6762d-165">Response</span></span>
<span data-ttu-id="6762d-166">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6762d-166">If successful, this method returns a `200 OK` response code and an updated [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6762d-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6762d-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="6762d-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6762d-168">Request</span></span>
<span data-ttu-id="6762d-169">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6762d-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
Content-type: application/json
Content-length: 534

{
  "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "encodedSettingXml": "ZW5jb2RlZFNldHRpbmdYbWw=",
  "settings": [
    {
      "@odata.type": "microsoft.graph.appConfigurationSettingItem",
      "appConfigKey": "App Config Key value",
      "appConfigKeyType": "integerType",
      "appConfigKeyValue": "App Config Key Value value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="6762d-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="6762d-170">Response</span></span>
<span data-ttu-id="6762d-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6762d-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 706

{
  "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
  "id": "b2c33191-3191-b2c3-9131-c3b29131c3b2",
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
  ],
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "encodedSettingXml": "ZW5jb2RlZFNldHRpbmdYbWw=",
  "settings": [
    {
      "@odata.type": "microsoft.graph.appConfigurationSettingItem",
      "appConfigKey": "App Config Key value",
      "appConfigKeyType": "integerType",
      "appConfigKeyValue": "App Config Key Value value"
    }
  ]
}
```



