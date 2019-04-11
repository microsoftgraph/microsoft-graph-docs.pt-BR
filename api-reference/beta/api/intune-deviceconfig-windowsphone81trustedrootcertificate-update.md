---
title: Atualizar windowsPhone81TrustedRootCertificate
description: Atualiza as propriedades de um objeto windowsPhone81TrustedRootCertificate.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e0acc47bd427a61e9009db8ecb7cb16f65f0f2d8
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31803518"
---
# <a name="update-windowsphone81trustedrootcertificate"></a><span data-ttu-id="20f2c-103">Atualizar windowsPhone81TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="20f2c-103">Update windowsPhone81TrustedRootCertificate</span></span>

> <span data-ttu-id="20f2c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="20f2c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="20f2c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="20f2c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20f2c-106">Atualiza as propriedades de um objeto [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="20f2c-106">Update the properties of a [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="20f2c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="20f2c-107">Prerequisites</span></span>
<span data-ttu-id="20f2c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20f2c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20f2c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20f2c-110">Permission type</span></span>|<span data-ttu-id="20f2c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="20f2c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20f2c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20f2c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="20f2c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20f2c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="20f2c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20f2c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20f2c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20f2c-115">Not supported.</span></span>|
|<span data-ttu-id="20f2c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20f2c-116">Application</span></span>|<span data-ttu-id="20f2c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20f2c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="20f2c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20f2c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/rootCertificate
```

## <a name="request-headers"></a><span data-ttu-id="20f2c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20f2c-119">Request headers</span></span>
|<span data-ttu-id="20f2c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="20f2c-120">Header</span></span>|<span data-ttu-id="20f2c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="20f2c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20f2c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="20f2c-122">Authorization</span></span>|<span data-ttu-id="20f2c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20f2c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20f2c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="20f2c-124">Accept</span></span>|<span data-ttu-id="20f2c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="20f2c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20f2c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20f2c-126">Request body</span></span>
<span data-ttu-id="20f2c-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="20f2c-127">In the request body, supply a JSON representation for the [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) object.</span></span>

<span data-ttu-id="20f2c-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="20f2c-128">The following table shows the properties that are required when you create the [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md).</span></span>

|<span data-ttu-id="20f2c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="20f2c-129">Property</span></span>|<span data-ttu-id="20f2c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="20f2c-130">Type</span></span>|<span data-ttu-id="20f2c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="20f2c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20f2c-132">id</span><span class="sxs-lookup"><span data-stu-id="20f2c-132">id</span></span>|<span data-ttu-id="20f2c-133">String</span><span class="sxs-lookup"><span data-stu-id="20f2c-133">String</span></span>|<span data-ttu-id="20f2c-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="20f2c-134">Key of the entity.</span></span> <span data-ttu-id="20f2c-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="20f2c-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20f2c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="20f2c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="20f2c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20f2c-137">DateTimeOffset</span></span>|<span data-ttu-id="20f2c-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="20f2c-138">DateTime the object was last modified.</span></span> <span data-ttu-id="20f2c-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="20f2c-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20f2c-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="20f2c-140">roleScopeTagIds</span></span>|<span data-ttu-id="20f2c-141">Coleção String</span><span class="sxs-lookup"><span data-stu-id="20f2c-141">String collection</span></span>|<span data-ttu-id="20f2c-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="20f2c-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="20f2c-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="20f2c-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20f2c-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="20f2c-144">supportsScopeTags</span></span>|<span data-ttu-id="20f2c-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="20f2c-145">Boolean</span></span>|<span data-ttu-id="20f2c-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="20f2c-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="20f2c-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="20f2c-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="20f2c-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="20f2c-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="20f2c-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="20f2c-149">This property is read-only.</span></span> <span data-ttu-id="20f2c-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="20f2c-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20f2c-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="20f2c-151">createdDateTime</span></span>|<span data-ttu-id="20f2c-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20f2c-152">DateTimeOffset</span></span>|<span data-ttu-id="20f2c-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="20f2c-153">DateTime the object was created.</span></span> <span data-ttu-id="20f2c-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="20f2c-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20f2c-155">description</span><span class="sxs-lookup"><span data-stu-id="20f2c-155">description</span></span>|<span data-ttu-id="20f2c-156">String</span><span class="sxs-lookup"><span data-stu-id="20f2c-156">String</span></span>|<span data-ttu-id="20f2c-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="20f2c-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="20f2c-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="20f2c-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20f2c-159">displayName</span><span class="sxs-lookup"><span data-stu-id="20f2c-159">displayName</span></span>|<span data-ttu-id="20f2c-160">String</span><span class="sxs-lookup"><span data-stu-id="20f2c-160">String</span></span>|<span data-ttu-id="20f2c-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="20f2c-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="20f2c-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="20f2c-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20f2c-163">versão</span><span class="sxs-lookup"><span data-stu-id="20f2c-163">version</span></span>|<span data-ttu-id="20f2c-164">Int32</span><span class="sxs-lookup"><span data-stu-id="20f2c-164">Int32</span></span>|<span data-ttu-id="20f2c-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="20f2c-165">Version of the device configuration.</span></span> <span data-ttu-id="20f2c-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="20f2c-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20f2c-167">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="20f2c-167">trustedRootCertificate</span></span>|<span data-ttu-id="20f2c-168">Binary</span><span class="sxs-lookup"><span data-stu-id="20f2c-168">Binary</span></span>|<span data-ttu-id="20f2c-169">Certificado raiz confiável</span><span class="sxs-lookup"><span data-stu-id="20f2c-169">Trusted Root Certificate</span></span>|
|<span data-ttu-id="20f2c-170">certFileName</span><span class="sxs-lookup"><span data-stu-id="20f2c-170">certFileName</span></span>|<span data-ttu-id="20f2c-171">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="20f2c-171">String</span></span>|<span data-ttu-id="20f2c-172">Nome do arquivo a ser exibido na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="20f2c-172">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="20f2c-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="20f2c-173">Response</span></span>
<span data-ttu-id="20f2c-174">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20f2c-174">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20f2c-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="20f2c-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="20f2c-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20f2c-176">Request</span></span>
<span data-ttu-id="20f2c-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="20f2c-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/rootCertificate
Content-type: application/json
Content-length: 374

{
  "@odata.type": "#microsoft.graph.windowsPhone81TrustedRootCertificate",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value"
}
```

### <a name="response"></a><span data-ttu-id="20f2c-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="20f2c-178">Response</span></span>
<span data-ttu-id="20f2c-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="20f2c-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 546

{
  "@odata.type": "#microsoft.graph.windowsPhone81TrustedRootCertificate",
  "id": "6316bf01-bf01-6316-01bf-166301bf1663",
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
  "certFileName": "Cert File Name value"
}
```





