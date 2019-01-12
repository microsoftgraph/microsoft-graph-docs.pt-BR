---
title: Atualizar iosTrustedRootCertificate
description: Atualize as propriedades de um objeto iosTrustedRootCertificate.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8050d9809541703f0ad3f659f22c4eddc880879d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931934"
---
# <a name="update-iostrustedrootcertificate"></a><span data-ttu-id="d3b1f-103">Atualizar iosTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="d3b1f-103">Update iosTrustedRootCertificate</span></span>

> <span data-ttu-id="d3b1f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d3b1f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d3b1f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d3b1f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d3b1f-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d3b1f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d3b1f-107">Atualize as propriedades de um objeto [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="d3b1f-107">Update the properties of a [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d3b1f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d3b1f-108">Prerequisites</span></span>
<span data-ttu-id="d3b1f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3b1f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3b1f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3b1f-111">Permission type</span></span>|<span data-ttu-id="d3b1f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d3b1f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3b1f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3b1f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d3b1f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3b1f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d3b1f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3b1f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3b1f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3b1f-116">Not supported.</span></span>|
|<span data-ttu-id="d3b1f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3b1f-117">Application</span></span>|<span data-ttu-id="d3b1f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3b1f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3b1f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3b1f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEnterpriseWiFiConfiguration/rootCertificatesForServerValidation/{iosTrustedRootCertificateId}
```

## <a name="request-headers"></a><span data-ttu-id="d3b1f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3b1f-120">Request headers</span></span>
|<span data-ttu-id="d3b1f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d3b1f-121">Header</span></span>|<span data-ttu-id="d3b1f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d3b1f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3b1f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3b1f-123">Authorization</span></span>|<span data-ttu-id="d3b1f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3b1f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3b1f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d3b1f-125">Accept</span></span>|<span data-ttu-id="d3b1f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d3b1f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3b1f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3b1f-127">Request body</span></span>
<span data-ttu-id="d3b1f-128">No corpo da solicitação, fornece uma representação JSON para o objeto [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="d3b1f-128">In the request body, supply a JSON representation for the [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) object.</span></span>

<span data-ttu-id="d3b1f-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="d3b1f-129">The following table shows the properties that are required when you create the [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md).</span></span>

|<span data-ttu-id="d3b1f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d3b1f-130">Property</span></span>|<span data-ttu-id="d3b1f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3b1f-131">Type</span></span>|<span data-ttu-id="d3b1f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3b1f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3b1f-133">id</span><span class="sxs-lookup"><span data-stu-id="d3b1f-133">id</span></span>|<span data-ttu-id="d3b1f-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d3b1f-134">String</span></span>|<span data-ttu-id="d3b1f-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d3b1f-135">Key of the entity.</span></span> <span data-ttu-id="d3b1f-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d3b1f-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3b1f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d3b1f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d3b1f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3b1f-138">DateTimeOffset</span></span>|<span data-ttu-id="d3b1f-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="d3b1f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d3b1f-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d3b1f-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3b1f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d3b1f-141">roleScopeTagIds</span></span>|<span data-ttu-id="d3b1f-142">String collection</span><span class="sxs-lookup"><span data-stu-id="d3b1f-142">String collection</span></span>|<span data-ttu-id="d3b1f-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="d3b1f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d3b1f-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d3b1f-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3b1f-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d3b1f-145">supportsScopeTags</span></span>|<span data-ttu-id="d3b1f-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="d3b1f-146">Boolean</span></span>|<span data-ttu-id="d3b1f-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="d3b1f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d3b1f-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="d3b1f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d3b1f-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="d3b1f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d3b1f-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d3b1f-150">This property is read-only.</span></span> <span data-ttu-id="d3b1f-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d3b1f-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3b1f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d3b1f-152">createdDateTime</span></span>|<span data-ttu-id="d3b1f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3b1f-153">DateTimeOffset</span></span>|<span data-ttu-id="d3b1f-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="d3b1f-154">DateTime the object was created.</span></span> <span data-ttu-id="d3b1f-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d3b1f-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3b1f-156">description</span><span class="sxs-lookup"><span data-stu-id="d3b1f-156">description</span></span>|<span data-ttu-id="d3b1f-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d3b1f-157">String</span></span>|<span data-ttu-id="d3b1f-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d3b1f-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d3b1f-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d3b1f-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3b1f-160">displayName</span><span class="sxs-lookup"><span data-stu-id="d3b1f-160">displayName</span></span>|<span data-ttu-id="d3b1f-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d3b1f-161">String</span></span>|<span data-ttu-id="d3b1f-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d3b1f-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d3b1f-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d3b1f-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3b1f-164">version</span><span class="sxs-lookup"><span data-stu-id="d3b1f-164">version</span></span>|<span data-ttu-id="d3b1f-165">Int32</span><span class="sxs-lookup"><span data-stu-id="d3b1f-165">Int32</span></span>|<span data-ttu-id="d3b1f-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d3b1f-166">Version of the device configuration.</span></span> <span data-ttu-id="d3b1f-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d3b1f-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3b1f-168">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="d3b1f-168">trustedRootCertificate</span></span>|<span data-ttu-id="d3b1f-169">Binária</span><span class="sxs-lookup"><span data-stu-id="d3b1f-169">Binary</span></span>|<span data-ttu-id="d3b1f-170">Certificado raiz confiável.</span><span class="sxs-lookup"><span data-stu-id="d3b1f-170">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="d3b1f-171">Nome_arquivo_cert</span><span class="sxs-lookup"><span data-stu-id="d3b1f-171">certFileName</span></span>|<span data-ttu-id="d3b1f-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d3b1f-172">String</span></span>|<span data-ttu-id="d3b1f-173">Nome de arquivo a ser exibido na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="d3b1f-173">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="d3b1f-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3b1f-174">Response</span></span>
<span data-ttu-id="d3b1f-175">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d3b1f-175">If successful, this method returns a `200 OK` response code and an updated [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3b1f-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d3b1f-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="d3b1f-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3b1f-177">Request</span></span>
<span data-ttu-id="d3b1f-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3b1f-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate
Content-type: application/json
Content-length: 363

{
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

### <a name="response"></a><span data-ttu-id="d3b1f-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3b1f-179">Response</span></span>
<span data-ttu-id="d3b1f-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d3b1f-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





