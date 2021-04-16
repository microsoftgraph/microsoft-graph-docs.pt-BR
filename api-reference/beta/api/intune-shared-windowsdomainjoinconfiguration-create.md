---
title: Criar windowsDomainJoinConfiguration
description: Crie um novo objeto windowsDomainJoinConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 55244869dd22c626d211a2b24e30e7befa28c6af
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866976"
---
# <a name="create-windowsdomainjoinconfiguration"></a><span data-ttu-id="7f847-103">Criar windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="7f847-103">Create windowsDomainJoinConfiguration</span></span>

<span data-ttu-id="7f847-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f847-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7f847-105">**Importante:** APIs na versão /beta do Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7f847-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7f847-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7f847-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7f847-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7f847-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f847-108">Crie um novo [objeto windowsDomainJoinConfiguration.](../resources/intune-shared-windowsdomainjoinconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7f847-108">Create a new [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7f847-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7f847-109">Prerequisites</span></span>
<span data-ttu-id="7f847-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f847-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f847-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7f847-112">Permission type</span></span>|<span data-ttu-id="7f847-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7f847-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f847-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7f847-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="7f847-115">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="7f847-115">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="7f847-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f847-116">DeviceManagementConfiguration.ReadWrite.All</span></span> |
|<span data-ttu-id="7f847-117">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7f847-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f847-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f847-118">Not supported.</span></span>|
|<span data-ttu-id="7f847-119">Application</span><span class="sxs-lookup"><span data-stu-id="7f847-119">Application</span></span>||
| <span data-ttu-id="7f847-120">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="7f847-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="7f847-121">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f847-121">DeviceManagementConfiguration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f847-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7f847-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7f847-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7f847-123">Request headers</span></span>

|<span data-ttu-id="7f847-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7f847-124">Header</span></span>|<span data-ttu-id="7f847-125">Valor</span><span class="sxs-lookup"><span data-stu-id="7f847-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f847-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="7f847-126">Authorization</span></span>|<span data-ttu-id="7f847-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7f847-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f847-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7f847-128">Accept</span></span>|<span data-ttu-id="7f847-129">application/json</span><span class="sxs-lookup"><span data-stu-id="7f847-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f847-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7f847-130">Request body</span></span>

<span data-ttu-id="7f847-131">No corpo da solicitação, fornece uma representação JSON para o objeto windowsDomainJoinConfiguration.</span><span class="sxs-lookup"><span data-stu-id="7f847-131">In the request body, supply a JSON representation for the windowsDomainJoinConfiguration object.</span></span>

<span data-ttu-id="7f847-132">A tabela a seguir mostra as propriedades que são necessárias ao criar o windowsDomainJoinConfiguration.</span><span class="sxs-lookup"><span data-stu-id="7f847-132">The following table shows the properties that are required when you create the windowsDomainJoinConfiguration.</span></span>

|<span data-ttu-id="7f847-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7f847-133">Property</span></span>|<span data-ttu-id="7f847-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f847-134">Type</span></span>|<span data-ttu-id="7f847-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f847-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f847-136">id</span><span class="sxs-lookup"><span data-stu-id="7f847-136">id</span></span>|<span data-ttu-id="7f847-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f847-137">String</span></span>|<span data-ttu-id="7f847-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7f847-138">Key of the entity.</span></span> <span data-ttu-id="7f847-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7f847-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f847-140">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="7f847-140">**Device configuration**</span></span>|
|<span data-ttu-id="7f847-141">activeDirectoryDomainName</span><span class="sxs-lookup"><span data-stu-id="7f847-141">activeDirectoryDomainName</span></span>|<span data-ttu-id="7f847-142">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="7f847-142">String</span></span>|<span data-ttu-id="7f847-143">Nome de domínio do Active Directory para ingressar.</span><span class="sxs-lookup"><span data-stu-id="7f847-143">Active Directory domain name to join.</span></span>|
|<span data-ttu-id="7f847-144">computerNameStaticPrefix</span><span class="sxs-lookup"><span data-stu-id="7f847-144">computerNameStaticPrefix</span></span>|<span data-ttu-id="7f847-145">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="7f847-145">String</span></span>|<span data-ttu-id="7f847-146">Prefixo fixo a ser usado para nome do computador.</span><span class="sxs-lookup"><span data-stu-id="7f847-146">Fixed prefix to be used for computer name.</span></span>|
|<span data-ttu-id="7f847-147">computerNameSuffixRandomCharCount</span><span class="sxs-lookup"><span data-stu-id="7f847-147">computerNameSuffixRandomCharCount</span></span>|<span data-ttu-id="7f847-148">Int32</span><span class="sxs-lookup"><span data-stu-id="7f847-148">Int32</span></span>|<span data-ttu-id="7f847-149">Caracteres gerados dinamicamente usados como sufixo para o nome do computador.</span><span class="sxs-lookup"><span data-stu-id="7f847-149">Dynamically generated characters used as suffix for computer name.</span></span> <span data-ttu-id="7f847-150">Valores válidos de 3 a 14</span><span class="sxs-lookup"><span data-stu-id="7f847-150">Valid values 3 to 14</span></span>|
|<span data-ttu-id="7f847-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7f847-151">createdDateTime</span></span>|<span data-ttu-id="7f847-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f847-152">DateTimeOffset</span></span>|<span data-ttu-id="7f847-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="7f847-153">DateTime the object was created.</span></span> <span data-ttu-id="7f847-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7f847-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f847-155">description</span><span class="sxs-lookup"><span data-stu-id="7f847-155">description</span></span>|<span data-ttu-id="7f847-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f847-156">String</span></span>|<span data-ttu-id="7f847-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7f847-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7f847-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7f847-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f847-159">displayName</span><span class="sxs-lookup"><span data-stu-id="7f847-159">displayName</span></span>|<span data-ttu-id="7f847-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f847-160">String</span></span>|<span data-ttu-id="7f847-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7f847-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7f847-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7f847-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f847-163">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7f847-163">lastModifiedDateTime</span></span>|<span data-ttu-id="7f847-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f847-164">DateTimeOffset</span></span>|<span data-ttu-id="7f847-165">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="7f847-165">DateTime the object was last modified.</span></span> <span data-ttu-id="7f847-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7f847-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f847-167">organizationalUnit</span><span class="sxs-lookup"><span data-stu-id="7f847-167">organizationalUnit</span></span>|<span data-ttu-id="7f847-168">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="7f847-168">String</span></span>|<span data-ttu-id="7f847-169">Unidade organizacional (OU) onde a conta do computador será criada.</span><span class="sxs-lookup"><span data-stu-id="7f847-169">Organizational unit (OU) where the computer account will be created.</span></span> <span data-ttu-id="7f847-170">Se esse parâmetro for NULL, o contêiner de objeto de computador conhecido será usado como publicado no domínio.</span><span class="sxs-lookup"><span data-stu-id="7f847-170">If this parameter is NULL, the well known computer object container will be used as published in the domain.</span></span>|
|<span data-ttu-id="7f847-171">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7f847-171">roleScopeTagIds</span></span>|<span data-ttu-id="7f847-172">Coleção String</span><span class="sxs-lookup"><span data-stu-id="7f847-172">String collection</span></span>|<span data-ttu-id="7f847-173">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="7f847-173">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7f847-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7f847-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f847-175">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="7f847-175">supportsScopeTags</span></span>|<span data-ttu-id="7f847-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f847-176">Boolean</span></span>|<span data-ttu-id="7f847-177">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="7f847-177">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7f847-178">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="7f847-178">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7f847-179">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="7f847-179">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7f847-180">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7f847-180">This property is read-only.</span></span> <span data-ttu-id="7f847-181">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7f847-181">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f847-182">versão</span><span class="sxs-lookup"><span data-stu-id="7f847-182">version</span></span>|<span data-ttu-id="7f847-183">Int32</span><span class="sxs-lookup"><span data-stu-id="7f847-183">Int32</span></span>|<span data-ttu-id="7f847-184">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7f847-184">Version of the device configuration.</span></span> <span data-ttu-id="7f847-185">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7f847-185">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="7f847-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f847-186">Response</span></span>

<span data-ttu-id="7f847-187">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7f847-187">If successful, this method returns a `201 Created` response code and a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f847-188">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7f847-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f847-189">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f847-189">Request</span></span>

<span data-ttu-id="7f847-190">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7f847-190">Here is an example of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="7f847-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f847-191">Response</span></span>

<span data-ttu-id="7f847-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7f847-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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










