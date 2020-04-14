---
title: Criar windowsDomainJoinConfiguration
description: Criar um novo objeto windowsDomainJoinConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 97d760b9e5dd34038a70cea14294fa4a27e55a3b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43447354"
---
# <a name="create-windowsdomainjoinconfiguration"></a><span data-ttu-id="0636c-103">Criar windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="0636c-103">Create windowsDomainJoinConfiguration</span></span>

<span data-ttu-id="0636c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0636c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0636c-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0636c-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0636c-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0636c-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0636c-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0636c-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0636c-108">Criar um novo objeto [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="0636c-108">Create a new [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0636c-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0636c-109">Prerequisites</span></span>
<span data-ttu-id="0636c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0636c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0636c-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0636c-112">Permission type</span></span>|<span data-ttu-id="0636c-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0636c-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0636c-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0636c-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="0636c-115">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="0636c-115">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="0636c-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0636c-116">DeviceManagementConfiguration.ReadWrite.All</span></span> |
|<span data-ttu-id="0636c-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0636c-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0636c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0636c-118">Not supported.</span></span>|
|<span data-ttu-id="0636c-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0636c-119">Application</span></span>||
| <span data-ttu-id="0636c-120">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="0636c-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="0636c-121">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0636c-121">DeviceManagementConfiguration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0636c-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0636c-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0636c-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0636c-123">Request headers</span></span>

|<span data-ttu-id="0636c-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0636c-124">Header</span></span>|<span data-ttu-id="0636c-125">Valor</span><span class="sxs-lookup"><span data-stu-id="0636c-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0636c-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="0636c-126">Authorization</span></span>|<span data-ttu-id="0636c-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0636c-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0636c-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0636c-128">Accept</span></span>|<span data-ttu-id="0636c-129">application/json</span><span class="sxs-lookup"><span data-stu-id="0636c-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0636c-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0636c-130">Request body</span></span>

<span data-ttu-id="0636c-131">No corpo da solicitação, forneça uma representação JSON do objeto windowsDomainJoinConfiguration.</span><span class="sxs-lookup"><span data-stu-id="0636c-131">In the request body, supply a JSON representation for the windowsDomainJoinConfiguration object.</span></span>

<span data-ttu-id="0636c-132">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsDomainJoinConfiguration.</span><span class="sxs-lookup"><span data-stu-id="0636c-132">The following table shows the properties that are required when you create the windowsDomainJoinConfiguration.</span></span>

|<span data-ttu-id="0636c-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0636c-133">Property</span></span>|<span data-ttu-id="0636c-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="0636c-134">Type</span></span>|<span data-ttu-id="0636c-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="0636c-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0636c-136">id</span><span class="sxs-lookup"><span data-stu-id="0636c-136">id</span></span>|<span data-ttu-id="0636c-137">String</span><span class="sxs-lookup"><span data-stu-id="0636c-137">String</span></span>|<span data-ttu-id="0636c-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0636c-138">Key of the entity.</span></span> <span data-ttu-id="0636c-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0636c-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0636c-140">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="0636c-140">**Device configuration**</span></span>|
|<span data-ttu-id="0636c-141">activeDirectoryDomainName</span><span class="sxs-lookup"><span data-stu-id="0636c-141">activeDirectoryDomainName</span></span>|<span data-ttu-id="0636c-142">String</span><span class="sxs-lookup"><span data-stu-id="0636c-142">String</span></span>|<span data-ttu-id="0636c-143">Nome de domínio do Active Directory para ingressar.</span><span class="sxs-lookup"><span data-stu-id="0636c-143">Active Directory domain name to join.</span></span>|
|<span data-ttu-id="0636c-144">computerNameStaticPrefix</span><span class="sxs-lookup"><span data-stu-id="0636c-144">computerNameStaticPrefix</span></span>|<span data-ttu-id="0636c-145">String</span><span class="sxs-lookup"><span data-stu-id="0636c-145">String</span></span>|<span data-ttu-id="0636c-146">Prefixo fixo a ser usado para o nome do computador.</span><span class="sxs-lookup"><span data-stu-id="0636c-146">Fixed prefix to be used for computer name.</span></span>|
|<span data-ttu-id="0636c-147">computerNameSuffixRandomCharCount</span><span class="sxs-lookup"><span data-stu-id="0636c-147">computerNameSuffixRandomCharCount</span></span>|<span data-ttu-id="0636c-148">Int32</span><span class="sxs-lookup"><span data-stu-id="0636c-148">Int32</span></span>|<span data-ttu-id="0636c-149">Caracteres gerados dinamicamente usados como sufixo para o nome do computador.</span><span class="sxs-lookup"><span data-stu-id="0636c-149">Dynamically generated characters used as suffix for computer name.</span></span> <span data-ttu-id="0636c-150">Valores válidos de 3 a 14</span><span class="sxs-lookup"><span data-stu-id="0636c-150">Valid values 3 to 14</span></span>|
|<span data-ttu-id="0636c-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0636c-151">createdDateTime</span></span>|<span data-ttu-id="0636c-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0636c-152">DateTimeOffset</span></span>|<span data-ttu-id="0636c-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="0636c-153">DateTime the object was created.</span></span> <span data-ttu-id="0636c-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0636c-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0636c-155">description</span><span class="sxs-lookup"><span data-stu-id="0636c-155">description</span></span>|<span data-ttu-id="0636c-156">String</span><span class="sxs-lookup"><span data-stu-id="0636c-156">String</span></span>|<span data-ttu-id="0636c-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0636c-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0636c-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0636c-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0636c-159">displayName</span><span class="sxs-lookup"><span data-stu-id="0636c-159">displayName</span></span>|<span data-ttu-id="0636c-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0636c-160">String</span></span>|<span data-ttu-id="0636c-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0636c-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0636c-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0636c-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0636c-163">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0636c-163">lastModifiedDateTime</span></span>|<span data-ttu-id="0636c-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0636c-164">DateTimeOffset</span></span>|<span data-ttu-id="0636c-165">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="0636c-165">DateTime the object was last modified.</span></span> <span data-ttu-id="0636c-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0636c-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0636c-167">organizationalUnit</span><span class="sxs-lookup"><span data-stu-id="0636c-167">organizationalUnit</span></span>|<span data-ttu-id="0636c-168">String</span><span class="sxs-lookup"><span data-stu-id="0636c-168">String</span></span>|<span data-ttu-id="0636c-169">Unidade organizacional (UO) em que a conta de computador será criada.</span><span class="sxs-lookup"><span data-stu-id="0636c-169">Organizational unit (OU) where the computer account will be created.</span></span> <span data-ttu-id="0636c-170">Se esse parâmetro for NULL, o contêiner do objeto de computador conhecido será usado como publicado no domínio.</span><span class="sxs-lookup"><span data-stu-id="0636c-170">If this parameter is NULL, the well known computer object container will be used as published in the domain.</span></span>|
|<span data-ttu-id="0636c-171">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0636c-171">roleScopeTagIds</span></span>|<span data-ttu-id="0636c-172">Coleção String</span><span class="sxs-lookup"><span data-stu-id="0636c-172">String collection</span></span>|<span data-ttu-id="0636c-173">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="0636c-173">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0636c-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0636c-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0636c-175">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0636c-175">supportsScopeTags</span></span>|<span data-ttu-id="0636c-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="0636c-176">Boolean</span></span>|<span data-ttu-id="0636c-177">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="0636c-177">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0636c-178">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="0636c-178">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0636c-179">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="0636c-179">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0636c-180">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0636c-180">This property is read-only.</span></span> <span data-ttu-id="0636c-181">Herdado de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0636c-181">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0636c-182">versão</span><span class="sxs-lookup"><span data-stu-id="0636c-182">version</span></span>|<span data-ttu-id="0636c-183">Int32</span><span class="sxs-lookup"><span data-stu-id="0636c-183">Int32</span></span>|<span data-ttu-id="0636c-184">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0636c-184">Version of the device configuration.</span></span> <span data-ttu-id="0636c-185">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0636c-185">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="0636c-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="0636c-186">Response</span></span>

<span data-ttu-id="0636c-187">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0636c-187">If successful, this method returns a `201 Created` response code and a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0636c-188">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0636c-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="0636c-189">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0636c-189">Request</span></span>

<span data-ttu-id="0636c-190">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0636c-190">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 559

{
  "@odata.type": "#microsoft.graph.windowsDomainJoinConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "computerNameStaticPrefix": "Computer Name Static Prefix value",
  "computerNameSuffixRandomCharCount": 1,
  "activeDirectoryDomainName": "Active Directory Domain Name value",
  "organizationalUnit": "Organizational Unit value"
}
```

### <a name="response"></a><span data-ttu-id="0636c-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="0636c-191">Response</span></span>

<span data-ttu-id="0636c-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0636c-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 667

{
  "@odata.type": "#microsoft.graph.windowsDomainJoinConfiguration",
  "id": "40118d08-8d08-4011-088d-1140088d1140",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "computerNameStaticPrefix": "Computer Name Static Prefix value",
  "computerNameSuffixRandomCharCount": 1,
  "activeDirectoryDomainName": "Active Directory Domain Name value",
  "organizationalUnit": "Organizational Unit value"
}
```









