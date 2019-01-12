---
title: Criar macOSDeviceFeaturesConfiguration
description: Criar um novo objeto macOSDeviceFeaturesConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8d19dc422c59231aad723effb5ce25ada57631f2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924955"
---
# <a name="create-macosdevicefeaturesconfiguration"></a><span data-ttu-id="1e336-103">Criar macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="1e336-103">Create macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="1e336-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1e336-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1e336-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1e336-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1e336-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1e336-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1e336-107">Criar um novo objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1e336-107">Create a new [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1e336-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1e336-108">Prerequisites</span></span>
<span data-ttu-id="1e336-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e336-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e336-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1e336-111">Permission type</span></span>|<span data-ttu-id="1e336-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1e336-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e336-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1e336-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1e336-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e336-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1e336-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1e336-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e336-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e336-116">Not supported.</span></span>|
|<span data-ttu-id="1e336-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1e336-117">Application</span></span>|<span data-ttu-id="1e336-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e336-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e336-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1e336-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1e336-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1e336-120">Request headers</span></span>
|<span data-ttu-id="1e336-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1e336-121">Header</span></span>|<span data-ttu-id="1e336-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1e336-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e336-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1e336-123">Authorization</span></span>|<span data-ttu-id="1e336-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e336-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e336-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1e336-125">Accept</span></span>|<span data-ttu-id="1e336-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1e336-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e336-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1e336-127">Request body</span></span>
<span data-ttu-id="1e336-128">No corpo da solicitação, forneça uma representação JSON do objeto macOSDeviceFeaturesConfiguration.</span><span class="sxs-lookup"><span data-stu-id="1e336-128">In the request body, supply a JSON representation for the macOSDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="1e336-129">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSDeviceFeaturesConfiguration.</span><span class="sxs-lookup"><span data-stu-id="1e336-129">The following table shows the properties that are required when you create the macOSDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="1e336-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1e336-130">Property</span></span>|<span data-ttu-id="1e336-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e336-131">Type</span></span>|<span data-ttu-id="1e336-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e336-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e336-133">id</span><span class="sxs-lookup"><span data-stu-id="1e336-133">id</span></span>|<span data-ttu-id="1e336-134">String</span><span class="sxs-lookup"><span data-stu-id="1e336-134">String</span></span>|<span data-ttu-id="1e336-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1e336-135">Key of the entity.</span></span> <span data-ttu-id="1e336-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e336-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e336-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1e336-137">lastModifiedDateTime</span></span>|<span data-ttu-id="1e336-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e336-138">DateTimeOffset</span></span>|<span data-ttu-id="1e336-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="1e336-139">DateTime the object was last modified.</span></span> <span data-ttu-id="1e336-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e336-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e336-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1e336-141">roleScopeTagIds</span></span>|<span data-ttu-id="1e336-142">String collection</span><span class="sxs-lookup"><span data-stu-id="1e336-142">String collection</span></span>|<span data-ttu-id="1e336-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="1e336-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1e336-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e336-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e336-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1e336-145">supportsScopeTags</span></span>|<span data-ttu-id="1e336-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="1e336-146">Boolean</span></span>|<span data-ttu-id="1e336-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="1e336-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1e336-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="1e336-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1e336-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="1e336-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1e336-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1e336-150">This property is read-only.</span></span> <span data-ttu-id="1e336-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e336-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e336-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1e336-152">createdDateTime</span></span>|<span data-ttu-id="1e336-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e336-153">DateTimeOffset</span></span>|<span data-ttu-id="1e336-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="1e336-154">DateTime the object was created.</span></span> <span data-ttu-id="1e336-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e336-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e336-156">description</span><span class="sxs-lookup"><span data-stu-id="1e336-156">description</span></span>|<span data-ttu-id="1e336-157">String</span><span class="sxs-lookup"><span data-stu-id="1e336-157">String</span></span>|<span data-ttu-id="1e336-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1e336-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1e336-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e336-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e336-160">displayName</span><span class="sxs-lookup"><span data-stu-id="1e336-160">displayName</span></span>|<span data-ttu-id="1e336-161">String</span><span class="sxs-lookup"><span data-stu-id="1e336-161">String</span></span>|<span data-ttu-id="1e336-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1e336-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1e336-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e336-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e336-164">version</span><span class="sxs-lookup"><span data-stu-id="1e336-164">version</span></span>|<span data-ttu-id="1e336-165">Int32</span><span class="sxs-lookup"><span data-stu-id="1e336-165">Int32</span></span>|<span data-ttu-id="1e336-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1e336-166">Version of the device configuration.</span></span> <span data-ttu-id="1e336-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e336-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e336-168">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="1e336-168">airPrintDestinations</span></span>|<span data-ttu-id="1e336-169">coleção [airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md)</span><span class="sxs-lookup"><span data-stu-id="1e336-169">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="1e336-170">Uma matriz de impressoras AirPrint que sempre devem ser exibidos.</span><span class="sxs-lookup"><span data-stu-id="1e336-170">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="1e336-171">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="1e336-171">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="1e336-172">Herdado de [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="1e336-172">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|



## <a name="response"></a><span data-ttu-id="1e336-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e336-173">Response</span></span>
<span data-ttu-id="1e336-174">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1e336-174">If successful, this method returns a `201 Created` response code and a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e336-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1e336-175">Example</span></span>
### <a name="request"></a><span data-ttu-id="1e336-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1e336-176">Request</span></span>
<span data-ttu-id="1e336-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1e336-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 564

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
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

### <a name="response"></a><span data-ttu-id="1e336-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e336-178">Response</span></span>
<span data-ttu-id="1e336-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1e336-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





