---
title: Atualizar windows81TrustedRootCertificate
description: Atualiza as propriedades de um objeto windows81TrustedRootCertificate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 188a2c8f3e8e4f5cf168a406dce2fffab82bf581
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33918182"
---
# <a name="update-windows81trustedrootcertificate"></a><span data-ttu-id="b34e3-103">Atualizar windows81TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="b34e3-103">Update windows81TrustedRootCertificate</span></span>

> <span data-ttu-id="b34e3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b34e3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b34e3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b34e3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b34e3-106">Atualiza as propriedades de um objeto [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="b34e3-106">Update the properties of a [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b34e3-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b34e3-107">Prerequisites</span></span>
<span data-ttu-id="b34e3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b34e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b34e3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b34e3-110">Permission type</span></span>|<span data-ttu-id="b34e3-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b34e3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b34e3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b34e3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b34e3-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b34e3-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b34e3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b34e3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b34e3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b34e3-115">Not supported.</span></span>|
|<span data-ttu-id="b34e3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b34e3-116">Application</span></span>|<span data-ttu-id="b34e3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b34e3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b34e3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b34e3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/rootCertificate
```

## <a name="request-headers"></a><span data-ttu-id="b34e3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b34e3-119">Request headers</span></span>
|<span data-ttu-id="b34e3-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b34e3-120">Header</span></span>|<span data-ttu-id="b34e3-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b34e3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b34e3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b34e3-122">Authorization</span></span>|<span data-ttu-id="b34e3-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b34e3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b34e3-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b34e3-124">Accept</span></span>|<span data-ttu-id="b34e3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b34e3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b34e3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b34e3-126">Request body</span></span>
<span data-ttu-id="b34e3-127">No corpo da solicitação, forneça uma representação JSON do objeto [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="b34e3-127">In the request body, supply a JSON representation for the [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object.</span></span>

<span data-ttu-id="b34e3-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="b34e3-128">The following table shows the properties that are required when you create the [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md).</span></span>

|<span data-ttu-id="b34e3-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b34e3-129">Property</span></span>|<span data-ttu-id="b34e3-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b34e3-130">Type</span></span>|<span data-ttu-id="b34e3-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b34e3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b34e3-132">id</span><span class="sxs-lookup"><span data-stu-id="b34e3-132">id</span></span>|<span data-ttu-id="b34e3-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b34e3-133">String</span></span>|<span data-ttu-id="b34e3-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b34e3-134">Key of the entity.</span></span> <span data-ttu-id="b34e3-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b34e3-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b34e3-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b34e3-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b34e3-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b34e3-137">DateTimeOffset</span></span>|<span data-ttu-id="b34e3-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="b34e3-138">DateTime the object was last modified.</span></span> <span data-ttu-id="b34e3-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b34e3-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b34e3-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b34e3-140">roleScopeTagIds</span></span>|<span data-ttu-id="b34e3-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b34e3-141">String collection</span></span>|<span data-ttu-id="b34e3-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="b34e3-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b34e3-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b34e3-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b34e3-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b34e3-144">supportsScopeTags</span></span>|<span data-ttu-id="b34e3-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="b34e3-145">Boolean</span></span>|<span data-ttu-id="b34e3-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="b34e3-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b34e3-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="b34e3-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b34e3-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="b34e3-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b34e3-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b34e3-149">This property is read-only.</span></span> <span data-ttu-id="b34e3-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b34e3-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b34e3-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b34e3-151">createdDateTime</span></span>|<span data-ttu-id="b34e3-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b34e3-152">DateTimeOffset</span></span>|<span data-ttu-id="b34e3-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="b34e3-153">DateTime the object was created.</span></span> <span data-ttu-id="b34e3-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b34e3-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b34e3-155">description</span><span class="sxs-lookup"><span data-stu-id="b34e3-155">description</span></span>|<span data-ttu-id="b34e3-156">String</span><span class="sxs-lookup"><span data-stu-id="b34e3-156">String</span></span>|<span data-ttu-id="b34e3-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b34e3-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b34e3-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b34e3-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b34e3-159">displayName</span><span class="sxs-lookup"><span data-stu-id="b34e3-159">displayName</span></span>|<span data-ttu-id="b34e3-160">String</span><span class="sxs-lookup"><span data-stu-id="b34e3-160">String</span></span>|<span data-ttu-id="b34e3-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b34e3-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b34e3-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b34e3-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b34e3-163">versão</span><span class="sxs-lookup"><span data-stu-id="b34e3-163">version</span></span>|<span data-ttu-id="b34e3-164">Int32</span><span class="sxs-lookup"><span data-stu-id="b34e3-164">Int32</span></span>|<span data-ttu-id="b34e3-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b34e3-165">Version of the device configuration.</span></span> <span data-ttu-id="b34e3-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b34e3-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b34e3-167">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="b34e3-167">trustedRootCertificate</span></span>|<span data-ttu-id="b34e3-168">Binária</span><span class="sxs-lookup"><span data-stu-id="b34e3-168">Binary</span></span>|<span data-ttu-id="b34e3-169">Certificado raiz confiável</span><span class="sxs-lookup"><span data-stu-id="b34e3-169">Trusted Root Certificate</span></span>|
|<span data-ttu-id="b34e3-170">certFileName</span><span class="sxs-lookup"><span data-stu-id="b34e3-170">certFileName</span></span>|<span data-ttu-id="b34e3-171">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b34e3-171">String</span></span>|<span data-ttu-id="b34e3-172">Nome do arquivo a ser exibido na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="b34e3-172">File name to display in UI.</span></span>|
|<span data-ttu-id="b34e3-173">destinationStore</span><span class="sxs-lookup"><span data-stu-id="b34e3-173">destinationStore</span></span>|[<span data-ttu-id="b34e3-174">certificateDestinationStore</span><span class="sxs-lookup"><span data-stu-id="b34e3-174">certificateDestinationStore</span></span>](../resources/intune-deviceconfig-certificatedestinationstore.md)|<span data-ttu-id="b34e3-175">Local do repositório de destino para o certificado raiz confiável.</span><span class="sxs-lookup"><span data-stu-id="b34e3-175">Destination store location for the Trusted Root Certificate.</span></span> <span data-ttu-id="b34e3-176">Os valores possíveis são: `computerCertStoreRoot`, `computerCertStoreIntermediate`, `userCertStoreIntermediate`.</span><span class="sxs-lookup"><span data-stu-id="b34e3-176">Possible values are: `computerCertStoreRoot`, `computerCertStoreIntermediate`, `userCertStoreIntermediate`.</span></span>|



## <a name="response"></a><span data-ttu-id="b34e3-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="b34e3-177">Response</span></span>
<span data-ttu-id="b34e3-178">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b34e3-178">If successful, this method returns a `200 OK` response code and an updated [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b34e3-179">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b34e3-179">Example</span></span>

### <a name="request"></a><span data-ttu-id="b34e3-180">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b34e3-180">Request</span></span>
<span data-ttu-id="b34e3-181">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b34e3-181">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}
Content-type: application/json
Content-length: 425

{
  "@odata.type": "#microsoft.graph.windows81TrustedRootCertificate",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value",
  "destinationStore": "computerCertStoreIntermediate"
}
```

### <a name="response"></a><span data-ttu-id="b34e3-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="b34e3-182">Response</span></span>
<span data-ttu-id="b34e3-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b34e3-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 597

{
  "@odata.type": "#microsoft.graph.windows81TrustedRootCertificate",
  "id": "3fb588f9-88f9-3fb5-f988-b53ff988b53f",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value",
  "destinationStore": "computerCertStoreIntermediate"
}
```




