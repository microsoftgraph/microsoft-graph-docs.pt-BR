---
title: Criar iosTrustedRootCertificate
description: Crie um novo objeto de iosTrustedRootCertificate.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6216dcccf2cde30506ee32dbbf612156c2fe3bce
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823412"
---
# <a name="create-iostrustedrootcertificate"></a><span data-ttu-id="66058-103">Criar iosTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="66058-103">Create iosTrustedRootCertificate</span></span>

> <span data-ttu-id="66058-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="66058-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="66058-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="66058-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="66058-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="66058-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="66058-107">Crie um novo objeto de [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="66058-107">Create a new [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="66058-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="66058-108">Prerequisites</span></span>
<span data-ttu-id="66058-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66058-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66058-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="66058-111">Permission type</span></span>|<span data-ttu-id="66058-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="66058-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66058-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="66058-113">Delegated (work or school account)</span></span>|<span data-ttu-id="66058-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66058-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="66058-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="66058-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66058-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66058-116">Not supported.</span></span>|
|<span data-ttu-id="66058-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="66058-117">Application</span></span>|<span data-ttu-id="66058-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66058-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="66058-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="66058-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEnterpriseWiFiConfiguration/rootCertificatesForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="66058-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="66058-120">Request headers</span></span>
|<span data-ttu-id="66058-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="66058-121">Header</span></span>|<span data-ttu-id="66058-122">Valor</span><span class="sxs-lookup"><span data-stu-id="66058-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66058-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="66058-123">Authorization</span></span>|<span data-ttu-id="66058-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="66058-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66058-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="66058-125">Accept</span></span>|<span data-ttu-id="66058-126">application/json</span><span class="sxs-lookup"><span data-stu-id="66058-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66058-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="66058-127">Request body</span></span>
<span data-ttu-id="66058-128">No corpo da solicitação, fornece uma representação JSON para o objeto iosTrustedRootCertificate.</span><span class="sxs-lookup"><span data-stu-id="66058-128">In the request body, supply a JSON representation for the iosTrustedRootCertificate object.</span></span>

<span data-ttu-id="66058-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o iosTrustedRootCertificate.</span><span class="sxs-lookup"><span data-stu-id="66058-129">The following table shows the properties that are required when you create the iosTrustedRootCertificate.</span></span>

|<span data-ttu-id="66058-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="66058-130">Property</span></span>|<span data-ttu-id="66058-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="66058-131">Type</span></span>|<span data-ttu-id="66058-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="66058-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66058-133">id</span><span class="sxs-lookup"><span data-stu-id="66058-133">id</span></span>|<span data-ttu-id="66058-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="66058-134">String</span></span>|<span data-ttu-id="66058-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="66058-135">Key of the entity.</span></span> <span data-ttu-id="66058-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="66058-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66058-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="66058-137">lastModifiedDateTime</span></span>|<span data-ttu-id="66058-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66058-138">DateTimeOffset</span></span>|<span data-ttu-id="66058-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="66058-139">DateTime the object was last modified.</span></span> <span data-ttu-id="66058-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="66058-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66058-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="66058-141">roleScopeTagIds</span></span>|<span data-ttu-id="66058-142">String collection</span><span class="sxs-lookup"><span data-stu-id="66058-142">String collection</span></span>|<span data-ttu-id="66058-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="66058-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="66058-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="66058-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66058-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="66058-145">supportsScopeTags</span></span>|<span data-ttu-id="66058-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="66058-146">Boolean</span></span>|<span data-ttu-id="66058-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="66058-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="66058-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="66058-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="66058-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="66058-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="66058-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66058-150">This property is read-only.</span></span> <span data-ttu-id="66058-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="66058-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66058-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="66058-152">createdDateTime</span></span>|<span data-ttu-id="66058-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66058-153">DateTimeOffset</span></span>|<span data-ttu-id="66058-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="66058-154">DateTime the object was created.</span></span> <span data-ttu-id="66058-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="66058-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66058-156">description</span><span class="sxs-lookup"><span data-stu-id="66058-156">description</span></span>|<span data-ttu-id="66058-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="66058-157">String</span></span>|<span data-ttu-id="66058-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="66058-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="66058-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="66058-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66058-160">displayName</span><span class="sxs-lookup"><span data-stu-id="66058-160">displayName</span></span>|<span data-ttu-id="66058-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="66058-161">String</span></span>|<span data-ttu-id="66058-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="66058-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="66058-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="66058-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66058-164">version</span><span class="sxs-lookup"><span data-stu-id="66058-164">version</span></span>|<span data-ttu-id="66058-165">Int32</span><span class="sxs-lookup"><span data-stu-id="66058-165">Int32</span></span>|<span data-ttu-id="66058-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="66058-166">Version of the device configuration.</span></span> <span data-ttu-id="66058-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="66058-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66058-168">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="66058-168">trustedRootCertificate</span></span>|<span data-ttu-id="66058-169">Binária</span><span class="sxs-lookup"><span data-stu-id="66058-169">Binary</span></span>|<span data-ttu-id="66058-170">Certificado raiz confiável.</span><span class="sxs-lookup"><span data-stu-id="66058-170">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="66058-171">Nome_arquivo_cert</span><span class="sxs-lookup"><span data-stu-id="66058-171">certFileName</span></span>|<span data-ttu-id="66058-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="66058-172">String</span></span>|<span data-ttu-id="66058-173">Nome de arquivo a ser exibido na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="66058-173">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="66058-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="66058-174">Response</span></span>
<span data-ttu-id="66058-175">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="66058-175">If successful, this method returns a `201 Created` response code and a [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66058-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="66058-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="66058-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="66058-177">Request</span></span>
<span data-ttu-id="66058-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="66058-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEnterpriseWiFiConfiguration/rootCertificatesForServerValidation
Content-type: application/json
Content-length: 427

{
  "@odata.type": "#microsoft.graph.iosTrustedRootCertificate",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="66058-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="66058-179">Response</span></span>
<span data-ttu-id="66058-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="66058-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 535

{
  "@odata.type": "#microsoft.graph.iosTrustedRootCertificate",
  "id": "9bc72bb8-2bb8-9bc7-b82b-c79bb82bc79b",
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





