---
title: Criar macOSDeviceFeaturesConfiguration
description: Criar um novo objeto macOSDeviceFeaturesConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 65b535959a5c8b58bd945870395e83f18ce6d171
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30979358"
---
# <a name="create-macosdevicefeaturesconfiguration"></a><span data-ttu-id="f8545-103">Criar macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="f8545-103">Create macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="f8545-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f8545-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8545-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f8545-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8545-106">Criar um novo objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f8545-106">Create a new [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f8545-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f8545-107">Prerequisites</span></span>
<span data-ttu-id="f8545-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8545-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8545-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f8545-110">Permission type</span></span>|<span data-ttu-id="f8545-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f8545-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8545-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f8545-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f8545-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8545-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f8545-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f8545-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8545-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8545-115">Not supported.</span></span>|
|<span data-ttu-id="f8545-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f8545-116">Application</span></span>|<span data-ttu-id="f8545-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8545-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8545-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f8545-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f8545-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f8545-119">Request headers</span></span>
|<span data-ttu-id="f8545-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f8545-120">Header</span></span>|<span data-ttu-id="f8545-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f8545-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8545-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f8545-122">Authorization</span></span>|<span data-ttu-id="f8545-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f8545-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8545-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f8545-124">Accept</span></span>|<span data-ttu-id="f8545-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f8545-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8545-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f8545-126">Request body</span></span>
<span data-ttu-id="f8545-127">No corpo da solicitação, forneça uma representação JSON do objeto macOSDeviceFeaturesConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f8545-127">In the request body, supply a JSON representation for the macOSDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="f8545-128">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSDeviceFeaturesConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f8545-128">The following table shows the properties that are required when you create the macOSDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="f8545-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f8545-129">Property</span></span>|<span data-ttu-id="f8545-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f8545-130">Type</span></span>|<span data-ttu-id="f8545-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8545-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8545-132">id</span><span class="sxs-lookup"><span data-stu-id="f8545-132">id</span></span>|<span data-ttu-id="f8545-133">String</span><span class="sxs-lookup"><span data-stu-id="f8545-133">String</span></span>|<span data-ttu-id="f8545-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f8545-134">Key of the entity.</span></span> <span data-ttu-id="f8545-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8545-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8545-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f8545-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f8545-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8545-137">DateTimeOffset</span></span>|<span data-ttu-id="f8545-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="f8545-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f8545-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8545-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8545-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f8545-140">roleScopeTagIds</span></span>|<span data-ttu-id="f8545-141">Coleção String</span><span class="sxs-lookup"><span data-stu-id="f8545-141">String collection</span></span>|<span data-ttu-id="f8545-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="f8545-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f8545-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8545-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8545-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f8545-144">supportsScopeTags</span></span>|<span data-ttu-id="f8545-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8545-145">Boolean</span></span>|<span data-ttu-id="f8545-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="f8545-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f8545-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="f8545-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f8545-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="f8545-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f8545-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f8545-149">This property is read-only.</span></span> <span data-ttu-id="f8545-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8545-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8545-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f8545-151">createdDateTime</span></span>|<span data-ttu-id="f8545-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8545-152">DateTimeOffset</span></span>|<span data-ttu-id="f8545-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="f8545-153">DateTime the object was created.</span></span> <span data-ttu-id="f8545-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8545-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8545-155">descrição</span><span class="sxs-lookup"><span data-stu-id="f8545-155">description</span></span>|<span data-ttu-id="f8545-156">String</span><span class="sxs-lookup"><span data-stu-id="f8545-156">String</span></span>|<span data-ttu-id="f8545-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f8545-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f8545-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8545-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8545-159">displayName</span><span class="sxs-lookup"><span data-stu-id="f8545-159">displayName</span></span>|<span data-ttu-id="f8545-160">String</span><span class="sxs-lookup"><span data-stu-id="f8545-160">String</span></span>|<span data-ttu-id="f8545-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f8545-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f8545-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8545-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8545-163">versão</span><span class="sxs-lookup"><span data-stu-id="f8545-163">version</span></span>|<span data-ttu-id="f8545-164">Int32</span><span class="sxs-lookup"><span data-stu-id="f8545-164">Int32</span></span>|<span data-ttu-id="f8545-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f8545-165">Version of the device configuration.</span></span> <span data-ttu-id="f8545-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8545-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8545-167">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="f8545-167">airPrintDestinations</span></span>|<span data-ttu-id="f8545-168">coleção [airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md)</span><span class="sxs-lookup"><span data-stu-id="f8545-168">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="f8545-169">Uma matriz de impressoras de impressão que sempre devem ser mostradas.</span><span class="sxs-lookup"><span data-stu-id="f8545-169">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="f8545-170">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="f8545-170">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="f8545-171">Herdado de [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="f8545-171">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|



## <a name="response"></a><span data-ttu-id="f8545-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8545-172">Response</span></span>
<span data-ttu-id="f8545-173">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f8545-173">If successful, this method returns a `201 Created` response code and a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8545-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f8545-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="f8545-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f8545-175">Request</span></span>
<span data-ttu-id="f8545-176">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f8545-176">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f8545-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8545-177">Response</span></span>
<span data-ttu-id="f8545-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f8545-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




