---
title: Atualizar macOSDeviceFeaturesConfiguration
description: Atualizar as propriedades de um objeto macOSDeviceFeaturesConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e9023fa910fb6bd19de92c685f008a4edb7e3e10
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852259"
---
# <a name="update-macosdevicefeaturesconfiguration"></a><span data-ttu-id="200cd-103">Atualizar macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="200cd-103">Update macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="200cd-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="200cd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="200cd-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="200cd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="200cd-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="200cd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="200cd-107">Atualizar as propriedades de um objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="200cd-107">Update the properties of a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="200cd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="200cd-108">Prerequisites</span></span>
<span data-ttu-id="200cd-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="200cd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="200cd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="200cd-111">Permission type</span></span>|<span data-ttu-id="200cd-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="200cd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="200cd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="200cd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="200cd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="200cd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="200cd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="200cd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="200cd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="200cd-116">Not supported.</span></span>|
|<span data-ttu-id="200cd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="200cd-117">Application</span></span>|<span data-ttu-id="200cd-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="200cd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="200cd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="200cd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="200cd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="200cd-120">Request headers</span></span>
|<span data-ttu-id="200cd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="200cd-121">Header</span></span>|<span data-ttu-id="200cd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="200cd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="200cd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="200cd-123">Authorization</span></span>|<span data-ttu-id="200cd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="200cd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="200cd-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="200cd-125">Accept</span></span>|<span data-ttu-id="200cd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="200cd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="200cd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="200cd-127">Request body</span></span>
<span data-ttu-id="200cd-128">No corpo da solicitação, forneça uma representação JSON do objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="200cd-128">In the request body, supply a JSON representation for the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="200cd-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="200cd-129">The following table shows the properties that are required when you create the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="200cd-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="200cd-130">Property</span></span>|<span data-ttu-id="200cd-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="200cd-131">Type</span></span>|<span data-ttu-id="200cd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="200cd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="200cd-133">id</span><span class="sxs-lookup"><span data-stu-id="200cd-133">id</span></span>|<span data-ttu-id="200cd-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="200cd-134">String</span></span>|<span data-ttu-id="200cd-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="200cd-135">Key of the entity.</span></span> <span data-ttu-id="200cd-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="200cd-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="200cd-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="200cd-137">lastModifiedDateTime</span></span>|<span data-ttu-id="200cd-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="200cd-138">DateTimeOffset</span></span>|<span data-ttu-id="200cd-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="200cd-139">DateTime the object was last modified.</span></span> <span data-ttu-id="200cd-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="200cd-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="200cd-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="200cd-141">roleScopeTagIds</span></span>|<span data-ttu-id="200cd-142">String collection</span><span class="sxs-lookup"><span data-stu-id="200cd-142">String collection</span></span>|<span data-ttu-id="200cd-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="200cd-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="200cd-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="200cd-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="200cd-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="200cd-145">supportsScopeTags</span></span>|<span data-ttu-id="200cd-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="200cd-146">Boolean</span></span>|<span data-ttu-id="200cd-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="200cd-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="200cd-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="200cd-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="200cd-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="200cd-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="200cd-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="200cd-150">This property is read-only.</span></span> <span data-ttu-id="200cd-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="200cd-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="200cd-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="200cd-152">createdDateTime</span></span>|<span data-ttu-id="200cd-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="200cd-153">DateTimeOffset</span></span>|<span data-ttu-id="200cd-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="200cd-154">DateTime the object was created.</span></span> <span data-ttu-id="200cd-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="200cd-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="200cd-156">description</span><span class="sxs-lookup"><span data-stu-id="200cd-156">description</span></span>|<span data-ttu-id="200cd-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="200cd-157">String</span></span>|<span data-ttu-id="200cd-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="200cd-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="200cd-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="200cd-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="200cd-160">displayName</span><span class="sxs-lookup"><span data-stu-id="200cd-160">displayName</span></span>|<span data-ttu-id="200cd-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="200cd-161">String</span></span>|<span data-ttu-id="200cd-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="200cd-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="200cd-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="200cd-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="200cd-164">version</span><span class="sxs-lookup"><span data-stu-id="200cd-164">version</span></span>|<span data-ttu-id="200cd-165">Int32</span><span class="sxs-lookup"><span data-stu-id="200cd-165">Int32</span></span>|<span data-ttu-id="200cd-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="200cd-166">Version of the device configuration.</span></span> <span data-ttu-id="200cd-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="200cd-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="200cd-168">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="200cd-168">airPrintDestinations</span></span>|<span data-ttu-id="200cd-169">coleção [airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md)</span><span class="sxs-lookup"><span data-stu-id="200cd-169">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="200cd-170">Uma matriz de impressoras AirPrint que sempre devem ser exibidos.</span><span class="sxs-lookup"><span data-stu-id="200cd-170">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="200cd-171">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="200cd-171">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="200cd-172">Herdado de [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="200cd-172">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|



## <a name="response"></a><span data-ttu-id="200cd-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="200cd-173">Response</span></span>
<span data-ttu-id="200cd-174">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="200cd-174">If successful, this method returns a `200 OK` response code and an updated [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="200cd-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="200cd-175">Example</span></span>
### <a name="request"></a><span data-ttu-id="200cd-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="200cd-176">Request</span></span>
<span data-ttu-id="200cd-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="200cd-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 493

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "airPrintDestinations": [
    {
      "@odata.type": "microsoft.graph.airPrintDestination",
      "ipAddress": "Ip Address value",
      "resourcePath": "Resource Path value",
      "port": 4,
      "forceTls": true
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="200cd-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="200cd-178">Response</span></span>
<span data-ttu-id="200cd-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="200cd-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 672

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "id": "49fa957d-957d-49fa-7d95-fa497d95fa49",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "airPrintDestinations": [
    {
      "@odata.type": "microsoft.graph.airPrintDestination",
      "ipAddress": "Ip Address value",
      "resourcePath": "Resource Path value",
      "port": 4,
      "forceTls": true
    }
  ]
}
```





