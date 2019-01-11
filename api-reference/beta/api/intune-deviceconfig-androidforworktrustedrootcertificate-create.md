---
title: Criar androidForWorkTrustedRootCertificate
description: Crie um novo objeto de androidForWorkTrustedRootCertificate.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9becf2b7f9781977f29d5950d05ab64e6c58376e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869283"
---
# <a name="create-androidforworktrustedrootcertificate"></a><span data-ttu-id="8472c-103">Criar androidForWorkTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="8472c-103">Create androidForWorkTrustedRootCertificate</span></span>

> <span data-ttu-id="8472c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8472c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8472c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8472c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8472c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8472c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8472c-107">Crie um novo objeto de [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="8472c-107">Create a new [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8472c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8472c-108">Prerequisites</span></span>
<span data-ttu-id="8472c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8472c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8472c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8472c-111">Permission type</span></span>|<span data-ttu-id="8472c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8472c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8472c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8472c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8472c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8472c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8472c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8472c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8472c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8472c-116">Not supported.</span></span>|
|<span data-ttu-id="8472c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8472c-117">Application</span></span>|<span data-ttu-id="8472c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8472c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8472c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8472c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8472c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8472c-120">Request headers</span></span>
|<span data-ttu-id="8472c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8472c-121">Header</span></span>|<span data-ttu-id="8472c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8472c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8472c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8472c-123">Authorization</span></span>|<span data-ttu-id="8472c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8472c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8472c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8472c-125">Accept</span></span>|<span data-ttu-id="8472c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8472c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8472c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8472c-127">Request body</span></span>
<span data-ttu-id="8472c-128">No corpo da solicitação, fornece uma representação JSON para o objeto androidForWorkTrustedRootCertificate.</span><span class="sxs-lookup"><span data-stu-id="8472c-128">In the request body, supply a JSON representation for the androidForWorkTrustedRootCertificate object.</span></span>

<span data-ttu-id="8472c-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o androidForWorkTrustedRootCertificate.</span><span class="sxs-lookup"><span data-stu-id="8472c-129">The following table shows the properties that are required when you create the androidForWorkTrustedRootCertificate.</span></span>

|<span data-ttu-id="8472c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8472c-130">Property</span></span>|<span data-ttu-id="8472c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8472c-131">Type</span></span>|<span data-ttu-id="8472c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8472c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8472c-133">id</span><span class="sxs-lookup"><span data-stu-id="8472c-133">id</span></span>|<span data-ttu-id="8472c-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8472c-134">String</span></span>|<span data-ttu-id="8472c-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8472c-135">Key of the entity.</span></span> <span data-ttu-id="8472c-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8472c-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8472c-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8472c-137">lastModifiedDateTime</span></span>|<span data-ttu-id="8472c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8472c-138">DateTimeOffset</span></span>|<span data-ttu-id="8472c-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="8472c-139">DateTime the object was last modified.</span></span> <span data-ttu-id="8472c-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8472c-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8472c-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8472c-141">roleScopeTagIds</span></span>|<span data-ttu-id="8472c-142">String collection</span><span class="sxs-lookup"><span data-stu-id="8472c-142">String collection</span></span>|<span data-ttu-id="8472c-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="8472c-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8472c-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8472c-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8472c-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8472c-145">supportsScopeTags</span></span>|<span data-ttu-id="8472c-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="8472c-146">Boolean</span></span>|<span data-ttu-id="8472c-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="8472c-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8472c-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="8472c-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8472c-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="8472c-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8472c-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8472c-150">This property is read-only.</span></span> <span data-ttu-id="8472c-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8472c-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8472c-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8472c-152">createdDateTime</span></span>|<span data-ttu-id="8472c-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8472c-153">DateTimeOffset</span></span>|<span data-ttu-id="8472c-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="8472c-154">DateTime the object was created.</span></span> <span data-ttu-id="8472c-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8472c-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8472c-156">description</span><span class="sxs-lookup"><span data-stu-id="8472c-156">description</span></span>|<span data-ttu-id="8472c-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8472c-157">String</span></span>|<span data-ttu-id="8472c-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8472c-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8472c-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8472c-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8472c-160">displayName</span><span class="sxs-lookup"><span data-stu-id="8472c-160">displayName</span></span>|<span data-ttu-id="8472c-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8472c-161">String</span></span>|<span data-ttu-id="8472c-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8472c-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8472c-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8472c-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8472c-164">version</span><span class="sxs-lookup"><span data-stu-id="8472c-164">version</span></span>|<span data-ttu-id="8472c-165">Int32</span><span class="sxs-lookup"><span data-stu-id="8472c-165">Int32</span></span>|<span data-ttu-id="8472c-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8472c-166">Version of the device configuration.</span></span> <span data-ttu-id="8472c-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8472c-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8472c-168">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="8472c-168">trustedRootCertificate</span></span>|<span data-ttu-id="8472c-169">Binária</span><span class="sxs-lookup"><span data-stu-id="8472c-169">Binary</span></span>|<span data-ttu-id="8472c-170">Certificado raiz confiável</span><span class="sxs-lookup"><span data-stu-id="8472c-170">Trusted Root Certificate</span></span>|
|<span data-ttu-id="8472c-171">Nome_arquivo_cert</span><span class="sxs-lookup"><span data-stu-id="8472c-171">certFileName</span></span>|<span data-ttu-id="8472c-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8472c-172">String</span></span>|<span data-ttu-id="8472c-173">Nome de arquivo a ser exibido na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="8472c-173">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="8472c-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="8472c-174">Response</span></span>
<span data-ttu-id="8472c-175">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8472c-175">If successful, this method returns a `201 Created` response code and a [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8472c-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8472c-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="8472c-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8472c-177">Request</span></span>
<span data-ttu-id="8472c-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8472c-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 438

{
  "@odata.type": "#microsoft.graph.androidForWorkTrustedRootCertificate",
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

### <a name="response"></a><span data-ttu-id="8472c-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="8472c-179">Response</span></span>
<span data-ttu-id="8472c-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8472c-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 546

{
  "@odata.type": "#microsoft.graph.androidForWorkTrustedRootCertificate",
  "id": "2f78834c-834c-2f78-4c83-782f4c83782f",
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





