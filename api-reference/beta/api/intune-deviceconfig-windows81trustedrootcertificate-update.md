---
title: Atualizar windows81TrustedRootCertificate
description: Atualize as propriedades de um objeto windows81TrustedRootCertificate.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 685e9ecb2b36b5db9062927f9ceb2f5603003317
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400554"
---
# <a name="update-windows81trustedrootcertificate"></a><span data-ttu-id="03dbf-103">Atualizar windows81TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="03dbf-103">Update windows81TrustedRootCertificate</span></span>

> <span data-ttu-id="03dbf-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="03dbf-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="03dbf-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="03dbf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="03dbf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="03dbf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03dbf-107">Atualize as propriedades de um objeto [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="03dbf-107">Update the properties of a [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="03dbf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="03dbf-108">Prerequisites</span></span>
<span data-ttu-id="03dbf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="03dbf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="03dbf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="03dbf-111">Permission type</span></span>|<span data-ttu-id="03dbf-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="03dbf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03dbf-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="03dbf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="03dbf-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03dbf-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="03dbf-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="03dbf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03dbf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="03dbf-116">Not supported.</span></span>|
|<span data-ttu-id="03dbf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="03dbf-117">Application</span></span>|<span data-ttu-id="03dbf-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="03dbf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="03dbf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="03dbf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/rootCertificate
```

## <a name="request-headers"></a><span data-ttu-id="03dbf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="03dbf-120">Request headers</span></span>
|<span data-ttu-id="03dbf-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="03dbf-121">Header</span></span>|<span data-ttu-id="03dbf-122">Valor</span><span class="sxs-lookup"><span data-stu-id="03dbf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03dbf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="03dbf-123">Authorization</span></span>|<span data-ttu-id="03dbf-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="03dbf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03dbf-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="03dbf-125">Accept</span></span>|<span data-ttu-id="03dbf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="03dbf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03dbf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="03dbf-127">Request body</span></span>
<span data-ttu-id="03dbf-128">No corpo da solicitação, fornece uma representação JSON para o objeto [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="03dbf-128">In the request body, supply a JSON representation for the [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object.</span></span>

<span data-ttu-id="03dbf-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="03dbf-129">The following table shows the properties that are required when you create the [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md).</span></span>

|<span data-ttu-id="03dbf-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="03dbf-130">Property</span></span>|<span data-ttu-id="03dbf-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="03dbf-131">Type</span></span>|<span data-ttu-id="03dbf-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="03dbf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03dbf-133">id</span><span class="sxs-lookup"><span data-stu-id="03dbf-133">id</span></span>|<span data-ttu-id="03dbf-134">String</span><span class="sxs-lookup"><span data-stu-id="03dbf-134">String</span></span>|<span data-ttu-id="03dbf-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="03dbf-135">Key of the entity.</span></span> <span data-ttu-id="03dbf-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03dbf-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03dbf-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="03dbf-137">lastModifiedDateTime</span></span>|<span data-ttu-id="03dbf-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03dbf-138">DateTimeOffset</span></span>|<span data-ttu-id="03dbf-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="03dbf-139">DateTime the object was last modified.</span></span> <span data-ttu-id="03dbf-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03dbf-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03dbf-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="03dbf-141">roleScopeTagIds</span></span>|<span data-ttu-id="03dbf-142">String collection</span><span class="sxs-lookup"><span data-stu-id="03dbf-142">String collection</span></span>|<span data-ttu-id="03dbf-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="03dbf-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="03dbf-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03dbf-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03dbf-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="03dbf-145">supportsScopeTags</span></span>|<span data-ttu-id="03dbf-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="03dbf-146">Boolean</span></span>|<span data-ttu-id="03dbf-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="03dbf-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="03dbf-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="03dbf-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="03dbf-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="03dbf-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="03dbf-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="03dbf-150">This property is read-only.</span></span> <span data-ttu-id="03dbf-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03dbf-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03dbf-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="03dbf-152">createdDateTime</span></span>|<span data-ttu-id="03dbf-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03dbf-153">DateTimeOffset</span></span>|<span data-ttu-id="03dbf-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="03dbf-154">DateTime the object was created.</span></span> <span data-ttu-id="03dbf-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03dbf-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03dbf-156">description</span><span class="sxs-lookup"><span data-stu-id="03dbf-156">description</span></span>|<span data-ttu-id="03dbf-157">String</span><span class="sxs-lookup"><span data-stu-id="03dbf-157">String</span></span>|<span data-ttu-id="03dbf-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="03dbf-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="03dbf-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03dbf-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03dbf-160">displayName</span><span class="sxs-lookup"><span data-stu-id="03dbf-160">displayName</span></span>|<span data-ttu-id="03dbf-161">String</span><span class="sxs-lookup"><span data-stu-id="03dbf-161">String</span></span>|<span data-ttu-id="03dbf-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="03dbf-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="03dbf-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03dbf-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03dbf-164">version</span><span class="sxs-lookup"><span data-stu-id="03dbf-164">version</span></span>|<span data-ttu-id="03dbf-165">Int32</span><span class="sxs-lookup"><span data-stu-id="03dbf-165">Int32</span></span>|<span data-ttu-id="03dbf-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="03dbf-166">Version of the device configuration.</span></span> <span data-ttu-id="03dbf-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03dbf-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03dbf-168">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="03dbf-168">trustedRootCertificate</span></span>|<span data-ttu-id="03dbf-169">Binária</span><span class="sxs-lookup"><span data-stu-id="03dbf-169">Binary</span></span>|<span data-ttu-id="03dbf-170">Certificado raiz confiável</span><span class="sxs-lookup"><span data-stu-id="03dbf-170">Trusted Root Certificate</span></span>|
|<span data-ttu-id="03dbf-171">Nome_arquivo_cert</span><span class="sxs-lookup"><span data-stu-id="03dbf-171">certFileName</span></span>|<span data-ttu-id="03dbf-172">String</span><span class="sxs-lookup"><span data-stu-id="03dbf-172">String</span></span>|<span data-ttu-id="03dbf-173">Nome de arquivo a ser exibido na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="03dbf-173">File name to display in UI.</span></span>|
|<span data-ttu-id="03dbf-174">destinationStore</span><span class="sxs-lookup"><span data-stu-id="03dbf-174">destinationStore</span></span>|[<span data-ttu-id="03dbf-175">certificateDestinationStore</span><span class="sxs-lookup"><span data-stu-id="03dbf-175">certificateDestinationStore</span></span>](../resources/intune-deviceconfig-certificatedestinationstore.md)|<span data-ttu-id="03dbf-176">Local do repositório de destino para o certificado de raiz confiável.</span><span class="sxs-lookup"><span data-stu-id="03dbf-176">Destination store location for the Trusted Root Certificate.</span></span> <span data-ttu-id="03dbf-177">Os valores possíveis são: `computerCertStoreRoot`, `computerCertStoreIntermediate`, `userCertStoreIntermediate`.</span><span class="sxs-lookup"><span data-stu-id="03dbf-177">Possible values are: `computerCertStoreRoot`, `computerCertStoreIntermediate`, `userCertStoreIntermediate`.</span></span>|



## <a name="response"></a><span data-ttu-id="03dbf-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="03dbf-178">Response</span></span>
<span data-ttu-id="03dbf-179">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="03dbf-179">If successful, this method returns a `200 OK` response code and an updated [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03dbf-180">Exemplo</span><span class="sxs-lookup"><span data-stu-id="03dbf-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="03dbf-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="03dbf-181">Request</span></span>
<span data-ttu-id="03dbf-182">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="03dbf-182">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="03dbf-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="03dbf-183">Response</span></span>
<span data-ttu-id="03dbf-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="03dbf-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




