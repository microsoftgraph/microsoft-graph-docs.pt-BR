---
title: Criar macOSTrustedRootCertificate
description: Criar um novo objeto macOSTrustedRootCertificate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a85a7666b2ab445e65fee9e84de7e40ff7eec933
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34963153"
---
# <a name="create-macostrustedrootcertificate"></a><span data-ttu-id="b6acb-103">Criar macOSTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="b6acb-103">Create macOSTrustedRootCertificate</span></span>

> <span data-ttu-id="b6acb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b6acb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6acb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b6acb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6acb-106">Criar um novo objeto [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="b6acb-106">Create a new [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6acb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b6acb-107">Prerequisites</span></span>
<span data-ttu-id="b6acb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6acb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6acb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6acb-110">Permission type</span></span>|<span data-ttu-id="b6acb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b6acb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6acb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6acb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b6acb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6acb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b6acb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6acb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6acb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6acb-115">Not supported.</span></span>|
|<span data-ttu-id="b6acb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6acb-116">Application</span></span>|<span data-ttu-id="b6acb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6acb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6acb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6acb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b6acb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6acb-119">Request headers</span></span>
|<span data-ttu-id="b6acb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b6acb-120">Header</span></span>|<span data-ttu-id="b6acb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b6acb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6acb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6acb-122">Authorization</span></span>|<span data-ttu-id="b6acb-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6acb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6acb-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b6acb-124">Accept</span></span>|<span data-ttu-id="b6acb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b6acb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6acb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6acb-126">Request body</span></span>
<span data-ttu-id="b6acb-127">No corpo da solicitação, forneça uma representação JSON do objeto macOSTrustedRootCertificate.</span><span class="sxs-lookup"><span data-stu-id="b6acb-127">In the request body, supply a JSON representation for the macOSTrustedRootCertificate object.</span></span>

<span data-ttu-id="b6acb-128">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSTrustedRootCertificate.</span><span class="sxs-lookup"><span data-stu-id="b6acb-128">The following table shows the properties that are required when you create the macOSTrustedRootCertificate.</span></span>

|<span data-ttu-id="b6acb-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b6acb-129">Property</span></span>|<span data-ttu-id="b6acb-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6acb-130">Type</span></span>|<span data-ttu-id="b6acb-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6acb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6acb-132">id</span><span class="sxs-lookup"><span data-stu-id="b6acb-132">id</span></span>|<span data-ttu-id="b6acb-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6acb-133">String</span></span>|<span data-ttu-id="b6acb-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b6acb-134">Key of the entity.</span></span> <span data-ttu-id="b6acb-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b6acb-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6acb-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b6acb-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b6acb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6acb-137">DateTimeOffset</span></span>|<span data-ttu-id="b6acb-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="b6acb-138">DateTime the object was last modified.</span></span> <span data-ttu-id="b6acb-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b6acb-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6acb-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b6acb-140">roleScopeTagIds</span></span>|<span data-ttu-id="b6acb-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6acb-141">String collection</span></span>|<span data-ttu-id="b6acb-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="b6acb-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b6acb-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b6acb-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6acb-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b6acb-144">supportsScopeTags</span></span>|<span data-ttu-id="b6acb-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="b6acb-145">Boolean</span></span>|<span data-ttu-id="b6acb-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="b6acb-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b6acb-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="b6acb-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b6acb-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="b6acb-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b6acb-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b6acb-149">This property is read-only.</span></span> <span data-ttu-id="b6acb-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b6acb-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6acb-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b6acb-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b6acb-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b6acb-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b6acb-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="b6acb-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b6acb-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b6acb-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6acb-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b6acb-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b6acb-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b6acb-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b6acb-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="b6acb-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b6acb-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b6acb-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6acb-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b6acb-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b6acb-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b6acb-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b6acb-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="b6acb-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b6acb-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b6acb-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6acb-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b6acb-163">createdDateTime</span></span>|<span data-ttu-id="b6acb-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6acb-164">DateTimeOffset</span></span>|<span data-ttu-id="b6acb-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="b6acb-165">DateTime the object was created.</span></span> <span data-ttu-id="b6acb-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b6acb-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6acb-167">descrição</span><span class="sxs-lookup"><span data-stu-id="b6acb-167">description</span></span>|<span data-ttu-id="b6acb-168">String</span><span class="sxs-lookup"><span data-stu-id="b6acb-168">String</span></span>|<span data-ttu-id="b6acb-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b6acb-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b6acb-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b6acb-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6acb-171">displayName</span><span class="sxs-lookup"><span data-stu-id="b6acb-171">displayName</span></span>|<span data-ttu-id="b6acb-172">String</span><span class="sxs-lookup"><span data-stu-id="b6acb-172">String</span></span>|<span data-ttu-id="b6acb-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b6acb-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b6acb-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b6acb-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6acb-175">versão</span><span class="sxs-lookup"><span data-stu-id="b6acb-175">version</span></span>|<span data-ttu-id="b6acb-176">Int32</span><span class="sxs-lookup"><span data-stu-id="b6acb-176">Int32</span></span>|<span data-ttu-id="b6acb-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b6acb-177">Version of the device configuration.</span></span> <span data-ttu-id="b6acb-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b6acb-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6acb-179">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="b6acb-179">trustedRootCertificate</span></span>|<span data-ttu-id="b6acb-180">Binária</span><span class="sxs-lookup"><span data-stu-id="b6acb-180">Binary</span></span>|<span data-ttu-id="b6acb-181">Certificado raiz confiável.</span><span class="sxs-lookup"><span data-stu-id="b6acb-181">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="b6acb-182">certFileName</span><span class="sxs-lookup"><span data-stu-id="b6acb-182">certFileName</span></span>|<span data-ttu-id="b6acb-183">String</span><span class="sxs-lookup"><span data-stu-id="b6acb-183">String</span></span>|<span data-ttu-id="b6acb-184">Nome do arquivo a ser exibido na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="b6acb-184">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="b6acb-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6acb-185">Response</span></span>
<span data-ttu-id="b6acb-186">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6acb-186">If successful, this method returns a `201 Created` response code and a [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6acb-187">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6acb-187">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6acb-188">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6acb-188">Request</span></span>
<span data-ttu-id="b6acb-189">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6acb-189">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1138

{
  "@odata.type": "#microsoft.graph.macOSTrustedRootCertificate",
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
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value"
}
```

### <a name="response"></a><span data-ttu-id="b6acb-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6acb-190">Response</span></span>
<span data-ttu-id="b6acb-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b6acb-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1310

{
  "@odata.type": "#microsoft.graph.macOSTrustedRootCertificate",
  "id": "c5fac954-c954-c5fa-54c9-fac554c9fac5",
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
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value"
}
```





