---
title: Criar macOSDeviceFeaturesConfiguration
description: Criar um novo objeto macOSDeviceFeaturesConfiguration.
author: tfitzmac
ms.openlocfilehash: 8cc53a63223ecbe695c566bdb9e813ec1618657d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341780"
---
# <a name="create-macosdevicefeaturesconfiguration"></a><span data-ttu-id="89060-103">Criar macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="89060-103">Create macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="89060-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="89060-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="89060-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="89060-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="89060-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="89060-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="89060-107">Criar um novo objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="89060-107">Create a new [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="89060-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="89060-108">Prerequisites</span></span>
<span data-ttu-id="89060-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89060-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89060-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="89060-111">Permission type</span></span>|<span data-ttu-id="89060-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="89060-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89060-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="89060-113">Delegated (work or school account)</span></span>|<span data-ttu-id="89060-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89060-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="89060-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="89060-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89060-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="89060-116">Not supported.</span></span>|
|<span data-ttu-id="89060-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="89060-117">Application</span></span>|<span data-ttu-id="89060-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="89060-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="89060-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="89060-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="89060-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="89060-120">Request headers</span></span>
|<span data-ttu-id="89060-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="89060-121">Header</span></span>|<span data-ttu-id="89060-122">Valor</span><span class="sxs-lookup"><span data-stu-id="89060-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89060-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="89060-123">Authorization</span></span>|<span data-ttu-id="89060-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="89060-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89060-125">Accept</span><span class="sxs-lookup"><span data-stu-id="89060-125">Accept</span></span>|<span data-ttu-id="89060-126">application/json</span><span class="sxs-lookup"><span data-stu-id="89060-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89060-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="89060-127">Request body</span></span>
<span data-ttu-id="89060-128">No corpo da solicitação, forneça uma representação JSON do objeto macOSDeviceFeaturesConfiguration.</span><span class="sxs-lookup"><span data-stu-id="89060-128">In the request body, supply a JSON representation for the macOSDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="89060-129">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSDeviceFeaturesConfiguration.</span><span class="sxs-lookup"><span data-stu-id="89060-129">The following table shows the properties that are required when you create the macOSDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="89060-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="89060-130">Property</span></span>|<span data-ttu-id="89060-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="89060-131">Type</span></span>|<span data-ttu-id="89060-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="89060-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89060-133">id</span><span class="sxs-lookup"><span data-stu-id="89060-133">id</span></span>|<span data-ttu-id="89060-134">String</span><span class="sxs-lookup"><span data-stu-id="89060-134">String</span></span>|<span data-ttu-id="89060-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="89060-135">Key of the entity.</span></span> <span data-ttu-id="89060-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89060-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89060-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="89060-137">lastModifiedDateTime</span></span>|<span data-ttu-id="89060-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89060-138">DateTimeOffset</span></span>|<span data-ttu-id="89060-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="89060-139">DateTime the object was last modified.</span></span> <span data-ttu-id="89060-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89060-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89060-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="89060-141">roleScopeTagIds</span></span>|<span data-ttu-id="89060-142">String collection</span><span class="sxs-lookup"><span data-stu-id="89060-142">String collection</span></span>|<span data-ttu-id="89060-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="89060-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="89060-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89060-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89060-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="89060-145">supportsScopeTags</span></span>|<span data-ttu-id="89060-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="89060-146">Boolean</span></span>|<span data-ttu-id="89060-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="89060-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="89060-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="89060-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="89060-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="89060-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="89060-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="89060-150">This property is read-only.</span></span> <span data-ttu-id="89060-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89060-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89060-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="89060-152">createdDateTime</span></span>|<span data-ttu-id="89060-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89060-153">DateTimeOffset</span></span>|<span data-ttu-id="89060-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="89060-154">DateTime the object was created.</span></span> <span data-ttu-id="89060-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89060-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89060-156">description</span><span class="sxs-lookup"><span data-stu-id="89060-156">description</span></span>|<span data-ttu-id="89060-157">String</span><span class="sxs-lookup"><span data-stu-id="89060-157">String</span></span>|<span data-ttu-id="89060-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="89060-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="89060-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89060-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89060-160">displayName</span><span class="sxs-lookup"><span data-stu-id="89060-160">displayName</span></span>|<span data-ttu-id="89060-161">String</span><span class="sxs-lookup"><span data-stu-id="89060-161">String</span></span>|<span data-ttu-id="89060-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="89060-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="89060-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89060-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89060-164">version</span><span class="sxs-lookup"><span data-stu-id="89060-164">version</span></span>|<span data-ttu-id="89060-165">Int32</span><span class="sxs-lookup"><span data-stu-id="89060-165">Int32</span></span>|<span data-ttu-id="89060-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="89060-166">Version of the device configuration.</span></span> <span data-ttu-id="89060-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89060-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89060-168">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="89060-168">airPrintDestinations</span></span>|<span data-ttu-id="89060-169">coleção [airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md)</span><span class="sxs-lookup"><span data-stu-id="89060-169">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="89060-170">Uma matriz de impressoras AirPrint que sempre devem ser exibidos.</span><span class="sxs-lookup"><span data-stu-id="89060-170">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="89060-171">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="89060-171">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="89060-172">Herdado de [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="89060-172">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|



## <a name="response"></a><span data-ttu-id="89060-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="89060-173">Response</span></span>
<span data-ttu-id="89060-174">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="89060-174">If successful, this method returns a `201 Created` response code and a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89060-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="89060-175">Example</span></span>
### <a name="request"></a><span data-ttu-id="89060-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="89060-176">Request</span></span>
<span data-ttu-id="89060-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="89060-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="89060-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="89060-178">Response</span></span>
<span data-ttu-id="89060-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="89060-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





