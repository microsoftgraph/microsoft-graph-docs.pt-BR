---
title: Criar androidForWorkTrustedRootCertificate
description: Criar um novo objeto androidForWorkTrustedRootCertificate.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bb4396882de59295afd601b63393634f1ec7af01
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160302"
---
# <a name="create-androidforworktrustedrootcertificate"></a><span data-ttu-id="1d0c6-103">Criar androidForWorkTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="1d0c6-103">Create androidForWorkTrustedRootCertificate</span></span>

> <span data-ttu-id="1d0c6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1d0c6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d0c6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1d0c6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d0c6-106">Criar um novo objeto [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="1d0c6-106">Create a new [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1d0c6-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1d0c6-107">Prerequisites</span></span>
<span data-ttu-id="1d0c6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1d0c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1d0c6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1d0c6-110">Permission type</span></span>|<span data-ttu-id="1d0c6-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1d0c6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d0c6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1d0c6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1d0c6-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d0c6-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1d0c6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1d0c6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d0c6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d0c6-115">Not supported.</span></span>|
|<span data-ttu-id="1d0c6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1d0c6-116">Application</span></span>|<span data-ttu-id="1d0c6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d0c6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d0c6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1d0c6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1d0c6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1d0c6-119">Request headers</span></span>
|<span data-ttu-id="1d0c6-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1d0c6-120">Header</span></span>|<span data-ttu-id="1d0c6-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1d0c6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d0c6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1d0c6-122">Authorization</span></span>|<span data-ttu-id="1d0c6-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1d0c6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d0c6-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1d0c6-124">Accept</span></span>|<span data-ttu-id="1d0c6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1d0c6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d0c6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1d0c6-126">Request body</span></span>
<span data-ttu-id="1d0c6-127">No corpo da solicitação, forneça uma representação JSON do objeto androidForWorkTrustedRootCertificate.</span><span class="sxs-lookup"><span data-stu-id="1d0c6-127">In the request body, supply a JSON representation for the androidForWorkTrustedRootCertificate object.</span></span>

<span data-ttu-id="1d0c6-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidForWorkTrustedRootCertificate.</span><span class="sxs-lookup"><span data-stu-id="1d0c6-128">The following table shows the properties that are required when you create the androidForWorkTrustedRootCertificate.</span></span>

|<span data-ttu-id="1d0c6-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d0c6-129">Property</span></span>|<span data-ttu-id="1d0c6-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d0c6-130">Type</span></span>|<span data-ttu-id="1d0c6-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d0c6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d0c6-132">id</span><span class="sxs-lookup"><span data-stu-id="1d0c6-132">id</span></span>|<span data-ttu-id="1d0c6-133">String</span><span class="sxs-lookup"><span data-stu-id="1d0c6-133">String</span></span>|<span data-ttu-id="1d0c6-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1d0c6-134">Key of the entity.</span></span> <span data-ttu-id="1d0c6-135">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1d0c6-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d0c6-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1d0c6-136">lastModifiedDateTime</span></span>|<span data-ttu-id="1d0c6-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d0c6-137">DateTimeOffset</span></span>|<span data-ttu-id="1d0c6-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="1d0c6-138">DateTime the object was last modified.</span></span> <span data-ttu-id="1d0c6-139">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1d0c6-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d0c6-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1d0c6-140">roleScopeTagIds</span></span>|<span data-ttu-id="1d0c6-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1d0c6-141">String collection</span></span>|<span data-ttu-id="1d0c6-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="1d0c6-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1d0c6-143">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1d0c6-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d0c6-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1d0c6-144">supportsScopeTags</span></span>|<span data-ttu-id="1d0c6-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d0c6-145">Boolean</span></span>|<span data-ttu-id="1d0c6-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="1d0c6-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1d0c6-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="1d0c6-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1d0c6-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="1d0c6-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1d0c6-149">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1d0c6-149">This property is read-only.</span></span> <span data-ttu-id="1d0c6-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1d0c6-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d0c6-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1d0c6-151">createdDateTime</span></span>|<span data-ttu-id="1d0c6-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d0c6-152">DateTimeOffset</span></span>|<span data-ttu-id="1d0c6-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="1d0c6-153">DateTime the object was created.</span></span> <span data-ttu-id="1d0c6-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1d0c6-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d0c6-155">description</span><span class="sxs-lookup"><span data-stu-id="1d0c6-155">description</span></span>|<span data-ttu-id="1d0c6-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1d0c6-156">String</span></span>|<span data-ttu-id="1d0c6-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1d0c6-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1d0c6-158">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1d0c6-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d0c6-159">displayName</span><span class="sxs-lookup"><span data-stu-id="1d0c6-159">displayName</span></span>|<span data-ttu-id="1d0c6-160">String</span><span class="sxs-lookup"><span data-stu-id="1d0c6-160">String</span></span>|<span data-ttu-id="1d0c6-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1d0c6-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1d0c6-162">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1d0c6-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d0c6-163">version</span><span class="sxs-lookup"><span data-stu-id="1d0c6-163">version</span></span>|<span data-ttu-id="1d0c6-164">Int32</span><span class="sxs-lookup"><span data-stu-id="1d0c6-164">Int32</span></span>|<span data-ttu-id="1d0c6-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1d0c6-165">Version of the device configuration.</span></span> <span data-ttu-id="1d0c6-166">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1d0c6-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d0c6-167">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="1d0c6-167">trustedRootCertificate</span></span>|<span data-ttu-id="1d0c6-168">Binária</span><span class="sxs-lookup"><span data-stu-id="1d0c6-168">Binary</span></span>|<span data-ttu-id="1d0c6-169">Certificado raiz confiável</span><span class="sxs-lookup"><span data-stu-id="1d0c6-169">Trusted Root Certificate</span></span>|
|<span data-ttu-id="1d0c6-170">certFileName</span><span class="sxs-lookup"><span data-stu-id="1d0c6-170">certFileName</span></span>|<span data-ttu-id="1d0c6-171">String</span><span class="sxs-lookup"><span data-stu-id="1d0c6-171">String</span></span>|<span data-ttu-id="1d0c6-172">Nome do arquivo a ser exibido na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="1d0c6-172">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="1d0c6-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d0c6-173">Response</span></span>
<span data-ttu-id="1d0c6-174">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1d0c6-174">If successful, this method returns a `201 Created` response code and a [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d0c6-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1d0c6-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="1d0c6-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1d0c6-176">Request</span></span>
<span data-ttu-id="1d0c6-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1d0c6-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 374

{
  "@odata.type": "#microsoft.graph.androidForWorkTrustedRootCertificate",
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

### <a name="response"></a><span data-ttu-id="1d0c6-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d0c6-178">Response</span></span>
<span data-ttu-id="1d0c6-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1d0c6-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




