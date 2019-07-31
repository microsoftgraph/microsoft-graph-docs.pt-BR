---
title: Criar windowsDomainJoinConfiguration
description: Criar um novo objeto windowsDomainJoinConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c2da99bc698993c57b67cbb009486953e6807c1b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35993540"
---
# <a name="create-windowsdomainjoinconfiguration"></a><span data-ttu-id="f930d-103">Criar windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="f930d-103">Create windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="f930d-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f930d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f930d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f930d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f930d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f930d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f930d-107">Criar um novo objeto [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f930d-107">Create a new [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f930d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f930d-108">Prerequisites</span></span>
<span data-ttu-id="f930d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f930d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f930d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f930d-111">Permission type</span></span>|<span data-ttu-id="f930d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f930d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f930d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f930d-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f930d-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="f930d-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="f930d-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f930d-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
|<span data-ttu-id="f930d-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f930d-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f930d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f930d-117">Not supported.</span></span>|
|<span data-ttu-id="f930d-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f930d-118">Application</span></span>|<span data-ttu-id="f930d-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f930d-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f930d-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f930d-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f930d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f930d-121">Request headers</span></span>

|<span data-ttu-id="f930d-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f930d-122">Header</span></span>|<span data-ttu-id="f930d-123">Valor</span><span class="sxs-lookup"><span data-stu-id="f930d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f930d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f930d-124">Authorization</span></span>|<span data-ttu-id="f930d-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f930d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f930d-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f930d-126">Accept</span></span>|<span data-ttu-id="f930d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f930d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f930d-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f930d-128">Request body</span></span>

<span data-ttu-id="f930d-129">No corpo da solicitação, forneça uma representação JSON do objeto windowsDomainJoinConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f930d-129">In the request body, supply a JSON representation for the windowsDomainJoinConfiguration object.</span></span>

<span data-ttu-id="f930d-130">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsDomainJoinConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f930d-130">The following table shows the properties that are required when you create the windowsDomainJoinConfiguration.</span></span>

|<span data-ttu-id="f930d-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f930d-131">Property</span></span>|<span data-ttu-id="f930d-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="f930d-132">Type</span></span>|<span data-ttu-id="f930d-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="f930d-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f930d-134">id</span><span class="sxs-lookup"><span data-stu-id="f930d-134">id</span></span>|<span data-ttu-id="f930d-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f930d-135">String</span></span>|<span data-ttu-id="f930d-136">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f930d-136">Key of the entity.</span></span> <span data-ttu-id="f930d-137">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f930d-137">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f930d-138">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="f930d-138">**Device configuration**</span></span>|
|<span data-ttu-id="f930d-139">activeDirectoryDomainName</span><span class="sxs-lookup"><span data-stu-id="f930d-139">activeDirectoryDomainName</span></span>|<span data-ttu-id="f930d-140">String</span><span class="sxs-lookup"><span data-stu-id="f930d-140">String</span></span>|<span data-ttu-id="f930d-141">Nome de domínio do Active Directory para ingressar.</span><span class="sxs-lookup"><span data-stu-id="f930d-141">Active Directory domain name to join.</span></span>|
|<span data-ttu-id="f930d-142">computerNameStaticPrefix</span><span class="sxs-lookup"><span data-stu-id="f930d-142">computerNameStaticPrefix</span></span>|<span data-ttu-id="f930d-143">String</span><span class="sxs-lookup"><span data-stu-id="f930d-143">String</span></span>|<span data-ttu-id="f930d-144">Prefixo fixo a ser usado para o nome do computador.</span><span class="sxs-lookup"><span data-stu-id="f930d-144">Fixed prefix to be used for computer name.</span></span>|
|<span data-ttu-id="f930d-145">computerNameSuffixRandomCharCount</span><span class="sxs-lookup"><span data-stu-id="f930d-145">computerNameSuffixRandomCharCount</span></span>|<span data-ttu-id="f930d-146">Int32</span><span class="sxs-lookup"><span data-stu-id="f930d-146">Int32</span></span>|<span data-ttu-id="f930d-147">Caracteres gerados dinamicamente usados como sufixo para o nome do computador.</span><span class="sxs-lookup"><span data-stu-id="f930d-147">Dynamically generated characters used as suffix for computer name.</span></span> <span data-ttu-id="f930d-148">Valores válidos de 3 a 14</span><span class="sxs-lookup"><span data-stu-id="f930d-148">Valid values 3 to 14</span></span>|
|<span data-ttu-id="f930d-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f930d-149">createdDateTime</span></span>|<span data-ttu-id="f930d-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f930d-150">DateTimeOffset</span></span>|<span data-ttu-id="f930d-151">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="f930d-151">DateTime the object was created.</span></span> <span data-ttu-id="f930d-152">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f930d-152">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f930d-153">descrição</span><span class="sxs-lookup"><span data-stu-id="f930d-153">description</span></span>|<span data-ttu-id="f930d-154">String</span><span class="sxs-lookup"><span data-stu-id="f930d-154">String</span></span>|<span data-ttu-id="f930d-155">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f930d-155">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f930d-156">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f930d-156">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f930d-157">displayName</span><span class="sxs-lookup"><span data-stu-id="f930d-157">displayName</span></span>|<span data-ttu-id="f930d-158">String</span><span class="sxs-lookup"><span data-stu-id="f930d-158">String</span></span>|<span data-ttu-id="f930d-159">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f930d-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f930d-160">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f930d-160">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f930d-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f930d-161">lastModifiedDateTime</span></span>|<span data-ttu-id="f930d-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f930d-162">DateTimeOffset</span></span>|<span data-ttu-id="f930d-163">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="f930d-163">DateTime the object was last modified.</span></span> <span data-ttu-id="f930d-164">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f930d-164">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f930d-165">organizationalUnit</span><span class="sxs-lookup"><span data-stu-id="f930d-165">organizationalUnit</span></span>|<span data-ttu-id="f930d-166">String</span><span class="sxs-lookup"><span data-stu-id="f930d-166">String</span></span>|<span data-ttu-id="f930d-167">Unidade organizacional (UO) em que a conta de computador será criada.</span><span class="sxs-lookup"><span data-stu-id="f930d-167">Organizational unit (OU) where the computer account will be created.</span></span> <span data-ttu-id="f930d-168">Se esse parâmetro for NULL, o contêiner do objeto de computador conhecido será usado como publicado no domínio.</span><span class="sxs-lookup"><span data-stu-id="f930d-168">If this parameter is NULL, the well known computer object container will be used as published in the domain.</span></span>|
|<span data-ttu-id="f930d-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f930d-169">roleScopeTagIds</span></span>|<span data-ttu-id="f930d-170">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f930d-170">String collection</span></span>|<span data-ttu-id="f930d-171">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="f930d-171">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f930d-172">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f930d-172">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f930d-173">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f930d-173">supportsScopeTags</span></span>|<span data-ttu-id="f930d-174">Booliano</span><span class="sxs-lookup"><span data-stu-id="f930d-174">Boolean</span></span>|<span data-ttu-id="f930d-175">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="f930d-175">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f930d-176">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="f930d-176">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f930d-177">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="f930d-177">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f930d-178">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f930d-178">This property is read-only.</span></span> <span data-ttu-id="f930d-179">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f930d-179">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f930d-180">versão</span><span class="sxs-lookup"><span data-stu-id="f930d-180">version</span></span>|<span data-ttu-id="f930d-181">Int32</span><span class="sxs-lookup"><span data-stu-id="f930d-181">Int32</span></span>|<span data-ttu-id="f930d-182">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f930d-182">Version of the device configuration.</span></span> <span data-ttu-id="f930d-183">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f930d-183">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="f930d-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="f930d-184">Response</span></span>

<span data-ttu-id="f930d-185">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f930d-185">If successful, this method returns a `201 Created` response code and a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f930d-186">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f930d-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="f930d-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f930d-187">Request</span></span>

<span data-ttu-id="f930d-188">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f930d-188">Here is an example of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="f930d-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="f930d-189">Response</span></span>

<span data-ttu-id="f930d-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f930d-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



