---
title: Atualizar windowsPhone81TrustedRootCertificate
description: Atualiza as propriedades de um objeto windowsPhone81TrustedRootCertificate.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7d93593ac66ea1eddc3902496884188f673fc2fe
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157971"
---
# <a name="update-windowsphone81trustedrootcertificate"></a><span data-ttu-id="69929-103">Atualizar windowsPhone81TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="69929-103">Update windowsPhone81TrustedRootCertificate</span></span>

> <span data-ttu-id="69929-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="69929-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69929-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="69929-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69929-106">Atualiza as propriedades de um objeto [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="69929-106">Update the properties of a [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="69929-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="69929-107">Prerequisites</span></span>
<span data-ttu-id="69929-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="69929-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="69929-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="69929-110">Permission type</span></span>|<span data-ttu-id="69929-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="69929-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69929-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="69929-112">Delegated (work or school account)</span></span>|<span data-ttu-id="69929-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69929-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="69929-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="69929-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69929-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="69929-115">Not supported.</span></span>|
|<span data-ttu-id="69929-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="69929-116">Application</span></span>|<span data-ttu-id="69929-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="69929-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="69929-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="69929-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/rootCertificate
```

## <a name="request-headers"></a><span data-ttu-id="69929-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="69929-119">Request headers</span></span>
|<span data-ttu-id="69929-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="69929-120">Header</span></span>|<span data-ttu-id="69929-121">Valor</span><span class="sxs-lookup"><span data-stu-id="69929-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69929-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="69929-122">Authorization</span></span>|<span data-ttu-id="69929-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="69929-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69929-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="69929-124">Accept</span></span>|<span data-ttu-id="69929-125">application/json</span><span class="sxs-lookup"><span data-stu-id="69929-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69929-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="69929-126">Request body</span></span>
<span data-ttu-id="69929-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="69929-127">In the request body, supply a JSON representation for the [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) object.</span></span>

<span data-ttu-id="69929-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="69929-128">The following table shows the properties that are required when you create the [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md).</span></span>

|<span data-ttu-id="69929-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="69929-129">Property</span></span>|<span data-ttu-id="69929-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="69929-130">Type</span></span>|<span data-ttu-id="69929-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="69929-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69929-132">id</span><span class="sxs-lookup"><span data-stu-id="69929-132">id</span></span>|<span data-ttu-id="69929-133">String</span><span class="sxs-lookup"><span data-stu-id="69929-133">String</span></span>|<span data-ttu-id="69929-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="69929-134">Key of the entity.</span></span> <span data-ttu-id="69929-135">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="69929-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69929-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="69929-136">lastModifiedDateTime</span></span>|<span data-ttu-id="69929-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69929-137">DateTimeOffset</span></span>|<span data-ttu-id="69929-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="69929-138">DateTime the object was last modified.</span></span> <span data-ttu-id="69929-139">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="69929-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69929-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="69929-140">roleScopeTagIds</span></span>|<span data-ttu-id="69929-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="69929-141">String collection</span></span>|<span data-ttu-id="69929-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="69929-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="69929-143">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="69929-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69929-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="69929-144">supportsScopeTags</span></span>|<span data-ttu-id="69929-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="69929-145">Boolean</span></span>|<span data-ttu-id="69929-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="69929-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="69929-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="69929-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="69929-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="69929-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="69929-149">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="69929-149">This property is read-only.</span></span> <span data-ttu-id="69929-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="69929-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69929-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="69929-151">createdDateTime</span></span>|<span data-ttu-id="69929-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69929-152">DateTimeOffset</span></span>|<span data-ttu-id="69929-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="69929-153">DateTime the object was created.</span></span> <span data-ttu-id="69929-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="69929-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69929-155">description</span><span class="sxs-lookup"><span data-stu-id="69929-155">description</span></span>|<span data-ttu-id="69929-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69929-156">String</span></span>|<span data-ttu-id="69929-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="69929-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="69929-158">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="69929-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69929-159">displayName</span><span class="sxs-lookup"><span data-stu-id="69929-159">displayName</span></span>|<span data-ttu-id="69929-160">String</span><span class="sxs-lookup"><span data-stu-id="69929-160">String</span></span>|<span data-ttu-id="69929-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="69929-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="69929-162">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="69929-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69929-163">version</span><span class="sxs-lookup"><span data-stu-id="69929-163">version</span></span>|<span data-ttu-id="69929-164">Int32</span><span class="sxs-lookup"><span data-stu-id="69929-164">Int32</span></span>|<span data-ttu-id="69929-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="69929-165">Version of the device configuration.</span></span> <span data-ttu-id="69929-166">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="69929-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69929-167">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="69929-167">trustedRootCertificate</span></span>|<span data-ttu-id="69929-168">Binária</span><span class="sxs-lookup"><span data-stu-id="69929-168">Binary</span></span>|<span data-ttu-id="69929-169">Certificado raiz confiável</span><span class="sxs-lookup"><span data-stu-id="69929-169">Trusted Root Certificate</span></span>|
|<span data-ttu-id="69929-170">certFileName</span><span class="sxs-lookup"><span data-stu-id="69929-170">certFileName</span></span>|<span data-ttu-id="69929-171">String</span><span class="sxs-lookup"><span data-stu-id="69929-171">String</span></span>|<span data-ttu-id="69929-172">Nome do arquivo a ser exibido na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="69929-172">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="69929-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="69929-173">Response</span></span>
<span data-ttu-id="69929-174">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="69929-174">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69929-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="69929-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="69929-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="69929-176">Request</span></span>
<span data-ttu-id="69929-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="69929-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="69929-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="69929-178">Response</span></span>
<span data-ttu-id="69929-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="69929-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




