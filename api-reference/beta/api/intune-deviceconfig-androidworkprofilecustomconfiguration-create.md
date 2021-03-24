---
title: Criar androidWorkProfileCustomConfiguration
description: Crie um novo objeto androidWorkProfileCustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ab7d21e957c7a910e3eafd6e0738f7f8567c8299
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51128282"
---
# <a name="create-androidworkprofilecustomconfiguration"></a><span data-ttu-id="bc264-103">Criar androidWorkProfileCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="bc264-103">Create androidWorkProfileCustomConfiguration</span></span>

<span data-ttu-id="bc264-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc264-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bc264-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bc264-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc264-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bc264-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc264-107">Crie um novo [objeto androidWorkProfileCustomConfiguration.](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc264-107">Create a new [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bc264-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bc264-108">Prerequisites</span></span>
<span data-ttu-id="bc264-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc264-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc264-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bc264-111">Permission type</span></span>|<span data-ttu-id="bc264-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bc264-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc264-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bc264-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bc264-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc264-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bc264-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bc264-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc264-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc264-116">Not supported.</span></span>|
|<span data-ttu-id="bc264-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bc264-117">Application</span></span>|<span data-ttu-id="bc264-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc264-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc264-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bc264-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="bc264-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bc264-120">Request headers</span></span>
|<span data-ttu-id="bc264-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bc264-121">Header</span></span>|<span data-ttu-id="bc264-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bc264-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc264-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bc264-123">Authorization</span></span>|<span data-ttu-id="bc264-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bc264-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc264-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bc264-125">Accept</span></span>|<span data-ttu-id="bc264-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bc264-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc264-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bc264-127">Request body</span></span>
<span data-ttu-id="bc264-128">No corpo da solicitação, fornece uma representação JSON para o objeto androidWorkProfileCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="bc264-128">In the request body, supply a JSON representation for the androidWorkProfileCustomConfiguration object.</span></span>

<span data-ttu-id="bc264-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o androidWorkProfileCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="bc264-129">The following table shows the properties that are required when you create the androidWorkProfileCustomConfiguration.</span></span>

|<span data-ttu-id="bc264-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bc264-130">Property</span></span>|<span data-ttu-id="bc264-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc264-131">Type</span></span>|<span data-ttu-id="bc264-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc264-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc264-133">id</span><span class="sxs-lookup"><span data-stu-id="bc264-133">id</span></span>|<span data-ttu-id="bc264-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc264-134">String</span></span>|<span data-ttu-id="bc264-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="bc264-135">Key of the entity.</span></span> <span data-ttu-id="bc264-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc264-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bc264-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bc264-137">lastModifiedDateTime</span></span>|<span data-ttu-id="bc264-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc264-138">DateTimeOffset</span></span>|<span data-ttu-id="bc264-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="bc264-139">DateTime the object was last modified.</span></span> <span data-ttu-id="bc264-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc264-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bc264-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bc264-141">roleScopeTagIds</span></span>|<span data-ttu-id="bc264-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc264-142">String collection</span></span>|<span data-ttu-id="bc264-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="bc264-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="bc264-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc264-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bc264-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="bc264-145">supportsScopeTags</span></span>|<span data-ttu-id="bc264-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="bc264-146">Boolean</span></span>|<span data-ttu-id="bc264-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="bc264-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="bc264-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="bc264-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="bc264-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="bc264-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="bc264-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bc264-150">This property is read-only.</span></span> <span data-ttu-id="bc264-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc264-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bc264-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="bc264-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="bc264-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="bc264-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="bc264-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="bc264-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="bc264-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc264-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bc264-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="bc264-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="bc264-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="bc264-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="bc264-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="bc264-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="bc264-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc264-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bc264-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="bc264-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="bc264-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="bc264-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="bc264-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="bc264-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="bc264-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc264-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bc264-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bc264-164">createdDateTime</span></span>|<span data-ttu-id="bc264-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc264-165">DateTimeOffset</span></span>|<span data-ttu-id="bc264-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="bc264-166">DateTime the object was created.</span></span> <span data-ttu-id="bc264-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc264-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bc264-168">descrição</span><span class="sxs-lookup"><span data-stu-id="bc264-168">description</span></span>|<span data-ttu-id="bc264-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc264-169">String</span></span>|<span data-ttu-id="bc264-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bc264-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bc264-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc264-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bc264-172">displayName</span><span class="sxs-lookup"><span data-stu-id="bc264-172">displayName</span></span>|<span data-ttu-id="bc264-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc264-173">String</span></span>|<span data-ttu-id="bc264-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bc264-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bc264-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc264-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bc264-176">versão</span><span class="sxs-lookup"><span data-stu-id="bc264-176">version</span></span>|<span data-ttu-id="bc264-177">Int32</span><span class="sxs-lookup"><span data-stu-id="bc264-177">Int32</span></span>|<span data-ttu-id="bc264-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bc264-178">Version of the device configuration.</span></span> <span data-ttu-id="bc264-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc264-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bc264-180">omaSettings</span><span class="sxs-lookup"><span data-stu-id="bc264-180">omaSettings</span></span>|<span data-ttu-id="bc264-181">Coleção [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="bc264-181">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="bc264-182">Configurações OMA.</span><span class="sxs-lookup"><span data-stu-id="bc264-182">OMA settings.</span></span> <span data-ttu-id="bc264-183">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="bc264-183">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="bc264-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc264-184">Response</span></span>
<span data-ttu-id="bc264-185">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bc264-185">If successful, this method returns a `201 Created` response code and a [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc264-186">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bc264-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="bc264-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc264-187">Request</span></span>
<span data-ttu-id="bc264-188">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bc264-188">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1280

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSetting",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "isEncrypted": true
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="bc264-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc264-189">Response</span></span>
<span data-ttu-id="bc264-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bc264-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1452

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
  "id": "76c5d59b-d59b-76c5-9bd5-c5769bd5c576",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSetting",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "isEncrypted": true
    }
  ]
}
```




