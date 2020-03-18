---
title: Criar windowsDomainJoinConfiguration
description: Criar um novo objeto windowsDomainJoinConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a083f270d43cf5863fb97345af830865434ad0c3
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800477"
---
# <a name="create-windowsdomainjoinconfiguration"></a><span data-ttu-id="83aa5-103">Criar windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="83aa5-103">Create windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="83aa5-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="83aa5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="83aa5-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="83aa5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="83aa5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="83aa5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83aa5-107">Criar um novo objeto [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="83aa5-107">Create a new [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="83aa5-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="83aa5-108">Prerequisites</span></span>
<span data-ttu-id="83aa5-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83aa5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83aa5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="83aa5-111">Permission type</span></span>|<span data-ttu-id="83aa5-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="83aa5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83aa5-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="83aa5-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="83aa5-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="83aa5-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="83aa5-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83aa5-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
|<span data-ttu-id="83aa5-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="83aa5-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83aa5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="83aa5-117">Not supported.</span></span>|
|<span data-ttu-id="83aa5-118">Application</span><span class="sxs-lookup"><span data-stu-id="83aa5-118">Application</span></span>||
| <span data-ttu-id="83aa5-119">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="83aa5-119">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="83aa5-120">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83aa5-120">DeviceManagementConfiguration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="83aa5-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="83aa5-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="83aa5-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="83aa5-122">Request headers</span></span>

|<span data-ttu-id="83aa5-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="83aa5-123">Header</span></span>|<span data-ttu-id="83aa5-124">Valor</span><span class="sxs-lookup"><span data-stu-id="83aa5-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83aa5-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="83aa5-125">Authorization</span></span>|<span data-ttu-id="83aa5-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="83aa5-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83aa5-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="83aa5-127">Accept</span></span>|<span data-ttu-id="83aa5-128">application/json</span><span class="sxs-lookup"><span data-stu-id="83aa5-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83aa5-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="83aa5-129">Request body</span></span>

<span data-ttu-id="83aa5-130">No corpo da solicitação, forneça uma representação JSON do objeto windowsDomainJoinConfiguration.</span><span class="sxs-lookup"><span data-stu-id="83aa5-130">In the request body, supply a JSON representation for the windowsDomainJoinConfiguration object.</span></span>

<span data-ttu-id="83aa5-131">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsDomainJoinConfiguration.</span><span class="sxs-lookup"><span data-stu-id="83aa5-131">The following table shows the properties that are required when you create the windowsDomainJoinConfiguration.</span></span>

|<span data-ttu-id="83aa5-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="83aa5-132">Property</span></span>|<span data-ttu-id="83aa5-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="83aa5-133">Type</span></span>|<span data-ttu-id="83aa5-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="83aa5-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83aa5-135">id</span><span class="sxs-lookup"><span data-stu-id="83aa5-135">id</span></span>|<span data-ttu-id="83aa5-136">String</span><span class="sxs-lookup"><span data-stu-id="83aa5-136">String</span></span>|<span data-ttu-id="83aa5-137">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="83aa5-137">Key of the entity.</span></span> <span data-ttu-id="83aa5-138">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83aa5-138">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83aa5-139">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="83aa5-139">**Device configuration**</span></span>|
|<span data-ttu-id="83aa5-140">activeDirectoryDomainName</span><span class="sxs-lookup"><span data-stu-id="83aa5-140">activeDirectoryDomainName</span></span>|<span data-ttu-id="83aa5-141">String</span><span class="sxs-lookup"><span data-stu-id="83aa5-141">String</span></span>|<span data-ttu-id="83aa5-142">Nome de domínio do Active Directory para ingressar.</span><span class="sxs-lookup"><span data-stu-id="83aa5-142">Active Directory domain name to join.</span></span>|
|<span data-ttu-id="83aa5-143">computerNameStaticPrefix</span><span class="sxs-lookup"><span data-stu-id="83aa5-143">computerNameStaticPrefix</span></span>|<span data-ttu-id="83aa5-144">String</span><span class="sxs-lookup"><span data-stu-id="83aa5-144">String</span></span>|<span data-ttu-id="83aa5-145">Prefixo fixo a ser usado para o nome do computador.</span><span class="sxs-lookup"><span data-stu-id="83aa5-145">Fixed prefix to be used for computer name.</span></span>|
|<span data-ttu-id="83aa5-146">computerNameSuffixRandomCharCount</span><span class="sxs-lookup"><span data-stu-id="83aa5-146">computerNameSuffixRandomCharCount</span></span>|<span data-ttu-id="83aa5-147">Int32</span><span class="sxs-lookup"><span data-stu-id="83aa5-147">Int32</span></span>|<span data-ttu-id="83aa5-148">Caracteres gerados dinamicamente usados como sufixo para o nome do computador.</span><span class="sxs-lookup"><span data-stu-id="83aa5-148">Dynamically generated characters used as suffix for computer name.</span></span> <span data-ttu-id="83aa5-149">Valores válidos de 3 a 14</span><span class="sxs-lookup"><span data-stu-id="83aa5-149">Valid values 3 to 14</span></span>|
|<span data-ttu-id="83aa5-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="83aa5-150">createdDateTime</span></span>|<span data-ttu-id="83aa5-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83aa5-151">DateTimeOffset</span></span>|<span data-ttu-id="83aa5-152">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="83aa5-152">DateTime the object was created.</span></span> <span data-ttu-id="83aa5-153">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83aa5-153">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83aa5-154">description</span><span class="sxs-lookup"><span data-stu-id="83aa5-154">description</span></span>|<span data-ttu-id="83aa5-155">String</span><span class="sxs-lookup"><span data-stu-id="83aa5-155">String</span></span>|<span data-ttu-id="83aa5-156">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="83aa5-156">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="83aa5-157">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83aa5-157">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83aa5-158">displayName</span><span class="sxs-lookup"><span data-stu-id="83aa5-158">displayName</span></span>|<span data-ttu-id="83aa5-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="83aa5-159">String</span></span>|<span data-ttu-id="83aa5-160">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="83aa5-160">Admin provided name of the device configuration.</span></span> <span data-ttu-id="83aa5-161">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83aa5-161">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83aa5-162">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="83aa5-162">lastModifiedDateTime</span></span>|<span data-ttu-id="83aa5-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83aa5-163">DateTimeOffset</span></span>|<span data-ttu-id="83aa5-164">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="83aa5-164">DateTime the object was last modified.</span></span> <span data-ttu-id="83aa5-165">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83aa5-165">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83aa5-166">organizationalUnit</span><span class="sxs-lookup"><span data-stu-id="83aa5-166">organizationalUnit</span></span>|<span data-ttu-id="83aa5-167">String</span><span class="sxs-lookup"><span data-stu-id="83aa5-167">String</span></span>|<span data-ttu-id="83aa5-168">Unidade organizacional (UO) em que a conta de computador será criada.</span><span class="sxs-lookup"><span data-stu-id="83aa5-168">Organizational unit (OU) where the computer account will be created.</span></span> <span data-ttu-id="83aa5-169">Se esse parâmetro for NULL, o contêiner do objeto de computador conhecido será usado como publicado no domínio.</span><span class="sxs-lookup"><span data-stu-id="83aa5-169">If this parameter is NULL, the well known computer object container will be used as published in the domain.</span></span>|
|<span data-ttu-id="83aa5-170">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="83aa5-170">roleScopeTagIds</span></span>|<span data-ttu-id="83aa5-171">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="83aa5-171">String collection</span></span>|<span data-ttu-id="83aa5-172">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="83aa5-172">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="83aa5-173">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83aa5-173">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83aa5-174">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="83aa5-174">supportsScopeTags</span></span>|<span data-ttu-id="83aa5-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="83aa5-175">Boolean</span></span>|<span data-ttu-id="83aa5-176">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="83aa5-176">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="83aa5-177">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="83aa5-177">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="83aa5-178">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="83aa5-178">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="83aa5-179">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="83aa5-179">This property is read-only.</span></span> <span data-ttu-id="83aa5-180">Herdado de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83aa5-180">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83aa5-181">versão</span><span class="sxs-lookup"><span data-stu-id="83aa5-181">version</span></span>|<span data-ttu-id="83aa5-182">Int32</span><span class="sxs-lookup"><span data-stu-id="83aa5-182">Int32</span></span>|<span data-ttu-id="83aa5-183">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="83aa5-183">Version of the device configuration.</span></span> <span data-ttu-id="83aa5-184">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83aa5-184">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="83aa5-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="83aa5-185">Response</span></span>

<span data-ttu-id="83aa5-186">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="83aa5-186">If successful, this method returns a `201 Created` response code and a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83aa5-187">Exemplo</span><span class="sxs-lookup"><span data-stu-id="83aa5-187">Example</span></span>

### <a name="request"></a><span data-ttu-id="83aa5-188">Solicitação</span><span class="sxs-lookup"><span data-stu-id="83aa5-188">Request</span></span>

<span data-ttu-id="83aa5-189">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="83aa5-189">Here is an example of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="83aa5-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="83aa5-190">Response</span></span>

<span data-ttu-id="83aa5-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="83aa5-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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










