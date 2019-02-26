---
title: Criar macOSDeviceFeaturesConfiguration
description: Criar um novo objeto macOSDeviceFeaturesConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5bccd64c5fc4b102340407ba1967a3b101c0b43e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148969"
---
# <a name="create-macosdevicefeaturesconfiguration"></a><span data-ttu-id="bb8fe-103">Criar macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="bb8fe-103">Create macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="bb8fe-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bb8fe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb8fe-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bb8fe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb8fe-106">Criar um novo objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bb8fe-106">Create a new [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb8fe-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bb8fe-107">Prerequisites</span></span>
<span data-ttu-id="bb8fe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="bb8fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bb8fe-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bb8fe-110">Permission type</span></span>|<span data-ttu-id="bb8fe-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bb8fe-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb8fe-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bb8fe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bb8fe-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb8fe-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bb8fe-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bb8fe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb8fe-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb8fe-115">Not supported.</span></span>|
|<span data-ttu-id="bb8fe-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bb8fe-116">Application</span></span>|<span data-ttu-id="bb8fe-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb8fe-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb8fe-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bb8fe-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="bb8fe-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bb8fe-119">Request headers</span></span>
|<span data-ttu-id="bb8fe-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bb8fe-120">Header</span></span>|<span data-ttu-id="bb8fe-121">Valor</span><span class="sxs-lookup"><span data-stu-id="bb8fe-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb8fe-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bb8fe-122">Authorization</span></span>|<span data-ttu-id="bb8fe-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bb8fe-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb8fe-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bb8fe-124">Accept</span></span>|<span data-ttu-id="bb8fe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bb8fe-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb8fe-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bb8fe-126">Request body</span></span>
<span data-ttu-id="bb8fe-127">No corpo da solicitação, forneça uma representação JSON do objeto macOSDeviceFeaturesConfiguration.</span><span class="sxs-lookup"><span data-stu-id="bb8fe-127">In the request body, supply a JSON representation for the macOSDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="bb8fe-128">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSDeviceFeaturesConfiguration.</span><span class="sxs-lookup"><span data-stu-id="bb8fe-128">The following table shows the properties that are required when you create the macOSDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="bb8fe-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bb8fe-129">Property</span></span>|<span data-ttu-id="bb8fe-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb8fe-130">Type</span></span>|<span data-ttu-id="bb8fe-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb8fe-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb8fe-132">id</span><span class="sxs-lookup"><span data-stu-id="bb8fe-132">id</span></span>|<span data-ttu-id="bb8fe-133">String</span><span class="sxs-lookup"><span data-stu-id="bb8fe-133">String</span></span>|<span data-ttu-id="bb8fe-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="bb8fe-134">Key of the entity.</span></span> <span data-ttu-id="bb8fe-135">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb8fe-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb8fe-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bb8fe-136">lastModifiedDateTime</span></span>|<span data-ttu-id="bb8fe-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb8fe-137">DateTimeOffset</span></span>|<span data-ttu-id="bb8fe-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="bb8fe-138">DateTime the object was last modified.</span></span> <span data-ttu-id="bb8fe-139">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb8fe-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb8fe-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bb8fe-140">roleScopeTagIds</span></span>|<span data-ttu-id="bb8fe-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb8fe-141">String collection</span></span>|<span data-ttu-id="bb8fe-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="bb8fe-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="bb8fe-143">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb8fe-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb8fe-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="bb8fe-144">supportsScopeTags</span></span>|<span data-ttu-id="bb8fe-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb8fe-145">Boolean</span></span>|<span data-ttu-id="bb8fe-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="bb8fe-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="bb8fe-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="bb8fe-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="bb8fe-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="bb8fe-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="bb8fe-149">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bb8fe-149">This property is read-only.</span></span> <span data-ttu-id="bb8fe-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb8fe-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb8fe-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bb8fe-151">createdDateTime</span></span>|<span data-ttu-id="bb8fe-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb8fe-152">DateTimeOffset</span></span>|<span data-ttu-id="bb8fe-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="bb8fe-153">DateTime the object was created.</span></span> <span data-ttu-id="bb8fe-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb8fe-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb8fe-155">description</span><span class="sxs-lookup"><span data-stu-id="bb8fe-155">description</span></span>|<span data-ttu-id="bb8fe-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb8fe-156">String</span></span>|<span data-ttu-id="bb8fe-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bb8fe-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bb8fe-158">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb8fe-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb8fe-159">displayName</span><span class="sxs-lookup"><span data-stu-id="bb8fe-159">displayName</span></span>|<span data-ttu-id="bb8fe-160">String</span><span class="sxs-lookup"><span data-stu-id="bb8fe-160">String</span></span>|<span data-ttu-id="bb8fe-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bb8fe-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bb8fe-162">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb8fe-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb8fe-163">version</span><span class="sxs-lookup"><span data-stu-id="bb8fe-163">version</span></span>|<span data-ttu-id="bb8fe-164">Int32</span><span class="sxs-lookup"><span data-stu-id="bb8fe-164">Int32</span></span>|<span data-ttu-id="bb8fe-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bb8fe-165">Version of the device configuration.</span></span> <span data-ttu-id="bb8fe-166">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb8fe-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb8fe-167">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="bb8fe-167">airPrintDestinations</span></span>|<span data-ttu-id="bb8fe-168">coleção [airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md)</span><span class="sxs-lookup"><span data-stu-id="bb8fe-168">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="bb8fe-169">Uma matriz de impressoras de impressão que sempre devem ser mostradas.</span><span class="sxs-lookup"><span data-stu-id="bb8fe-169">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="bb8fe-170">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="bb8fe-170">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="bb8fe-171">Herdado de [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="bb8fe-171">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|



## <a name="response"></a><span data-ttu-id="bb8fe-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb8fe-172">Response</span></span>
<span data-ttu-id="bb8fe-173">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bb8fe-173">If successful, this method returns a `201 Created` response code and a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb8fe-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bb8fe-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb8fe-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bb8fe-175">Request</span></span>
<span data-ttu-id="bb8fe-176">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bb8fe-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 500

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
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

### <a name="response"></a><span data-ttu-id="bb8fe-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb8fe-177">Response</span></span>
<span data-ttu-id="bb8fe-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bb8fe-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




