---
title: Criar windowsDomainJoinConfiguration
description: Crie um novo objeto de windowsDomainJoinConfiguration.
ms.openlocfilehash: 8069dfac727ee24d96f72875a4cec19fa42b8baa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040459"
---
# <a name="create-windowsdomainjoinconfiguration"></a><span data-ttu-id="61525-103">Criar windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="61525-103">Create windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="61525-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="61525-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="61525-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="61525-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="61525-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="61525-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="61525-107">Crie um novo objeto de [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="61525-107">Create a new [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="61525-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="61525-108">Prerequisites</span></span>
<span data-ttu-id="61525-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61525-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61525-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="61525-111">Permission type</span></span>|<span data-ttu-id="61525-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="61525-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61525-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="61525-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="61525-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="61525-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="61525-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61525-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
|<span data-ttu-id="61525-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="61525-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61525-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61525-117">Not supported.</span></span>|
|<span data-ttu-id="61525-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="61525-118">Application</span></span>|<span data-ttu-id="61525-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61525-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="61525-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="61525-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="61525-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="61525-121">Request headers</span></span>

|<span data-ttu-id="61525-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="61525-122">Header</span></span>|<span data-ttu-id="61525-123">Valor</span><span class="sxs-lookup"><span data-stu-id="61525-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61525-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="61525-124">Authorization</span></span>|<span data-ttu-id="61525-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="61525-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="61525-126">Accept</span><span class="sxs-lookup"><span data-stu-id="61525-126">Accept</span></span>|<span data-ttu-id="61525-127">application/json</span><span class="sxs-lookup"><span data-stu-id="61525-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61525-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="61525-128">Request body</span></span>

<span data-ttu-id="61525-129">No corpo da solicitação, fornece uma representação JSON para o objeto windowsDomainJoinConfiguration.</span><span class="sxs-lookup"><span data-stu-id="61525-129">In the request body, supply a JSON representation for the windowsDomainJoinConfiguration object.</span></span>

<span data-ttu-id="61525-130">A tabela a seguir mostra as propriedades que são necessárias quando você cria o windowsDomainJoinConfiguration.</span><span class="sxs-lookup"><span data-stu-id="61525-130">The following table shows the properties that are required when you create the windowsDomainJoinConfiguration.</span></span>

|<span data-ttu-id="61525-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="61525-131">Property</span></span>|<span data-ttu-id="61525-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="61525-132">Type</span></span>|<span data-ttu-id="61525-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="61525-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61525-134">id</span><span class="sxs-lookup"><span data-stu-id="61525-134">id</span></span>|<span data-ttu-id="61525-135">String</span><span class="sxs-lookup"><span data-stu-id="61525-135">String</span></span>|<span data-ttu-id="61525-136">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="61525-136">Key of the entity.</span></span> <span data-ttu-id="61525-137">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="61525-137">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="61525-138">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="61525-138">**Device configuration**</span></span>|
|<span data-ttu-id="61525-139">activeDirectoryDomainName</span><span class="sxs-lookup"><span data-stu-id="61525-139">activeDirectoryDomainName</span></span>|<span data-ttu-id="61525-140">String</span><span class="sxs-lookup"><span data-stu-id="61525-140">String</span></span>|<span data-ttu-id="61525-141">Nome de domínio Active Directory para ingressar.</span><span class="sxs-lookup"><span data-stu-id="61525-141">Active Directory domain name to join.</span></span>|
|<span data-ttu-id="61525-142">computerNameStaticPrefix</span><span class="sxs-lookup"><span data-stu-id="61525-142">computerNameStaticPrefix</span></span>|<span data-ttu-id="61525-143">String</span><span class="sxs-lookup"><span data-stu-id="61525-143">String</span></span>|<span data-ttu-id="61525-144">Fixo prefixo a ser usado para o nome do computador.</span><span class="sxs-lookup"><span data-stu-id="61525-144">Fixed prefix to be used for computer name.</span></span>|
|<span data-ttu-id="61525-145">computerNameSuffixRandomCharCount</span><span class="sxs-lookup"><span data-stu-id="61525-145">computerNameSuffixRandomCharCount</span></span>|<span data-ttu-id="61525-146">Int32</span><span class="sxs-lookup"><span data-stu-id="61525-146">Int32</span></span>|<span data-ttu-id="61525-147">Caracteres gerados dinamicamente usados como o sufixo de nome do computador.</span><span class="sxs-lookup"><span data-stu-id="61525-147">Dynamically generated characters used as suffix for computer name.</span></span> <span data-ttu-id="61525-148">Valores válidos 3 e 14</span><span class="sxs-lookup"><span data-stu-id="61525-148">Valid values 3 to 14</span></span>|
|<span data-ttu-id="61525-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="61525-149">createdDateTime</span></span>|<span data-ttu-id="61525-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61525-150">DateTimeOffset</span></span>|<span data-ttu-id="61525-151">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="61525-151">DateTime the object was created.</span></span> <span data-ttu-id="61525-152">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="61525-152">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="61525-153">description</span><span class="sxs-lookup"><span data-stu-id="61525-153">description</span></span>|<span data-ttu-id="61525-154">String</span><span class="sxs-lookup"><span data-stu-id="61525-154">String</span></span>|<span data-ttu-id="61525-155">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="61525-155">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="61525-156">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="61525-156">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="61525-157">displayName</span><span class="sxs-lookup"><span data-stu-id="61525-157">displayName</span></span>|<span data-ttu-id="61525-158">String</span><span class="sxs-lookup"><span data-stu-id="61525-158">String</span></span>|<span data-ttu-id="61525-159">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="61525-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="61525-160">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="61525-160">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="61525-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="61525-161">lastModifiedDateTime</span></span>|<span data-ttu-id="61525-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61525-162">DateTimeOffset</span></span>|<span data-ttu-id="61525-163">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="61525-163">DateTime the object was last modified.</span></span> <span data-ttu-id="61525-164">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="61525-164">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="61525-165">organizationalUnit</span><span class="sxs-lookup"><span data-stu-id="61525-165">organizationalUnit</span></span>|<span data-ttu-id="61525-166">String</span><span class="sxs-lookup"><span data-stu-id="61525-166">String</span></span>|<span data-ttu-id="61525-167">Unidade organizacional (UO) onde a conta de computador será criada.</span><span class="sxs-lookup"><span data-stu-id="61525-167">Organizational unit (OU) where the computer account will be created.</span></span> <span data-ttu-id="61525-168">Se esse parâmetro for NULL, será usado o contêiner de objeto de computador bem conhecido como publicado no domínio.</span><span class="sxs-lookup"><span data-stu-id="61525-168">If this parameter is NULL, the well known computer object container will be used as published in the domain.</span></span>|
|<span data-ttu-id="61525-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="61525-169">roleScopeTagIds</span></span>|<span data-ttu-id="61525-170">String collection</span><span class="sxs-lookup"><span data-stu-id="61525-170">String collection</span></span>|<span data-ttu-id="61525-171">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="61525-171">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="61525-172">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="61525-172">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="61525-173">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="61525-173">supportsScopeTags</span></span>|<span data-ttu-id="61525-174">Booliano</span><span class="sxs-lookup"><span data-stu-id="61525-174">Boolean</span></span>|<span data-ttu-id="61525-175">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="61525-175">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="61525-176">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="61525-176">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="61525-177">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="61525-177">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="61525-178">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="61525-178">This property is read-only.</span></span> <span data-ttu-id="61525-179">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="61525-179">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="61525-180">version</span><span class="sxs-lookup"><span data-stu-id="61525-180">version</span></span>|<span data-ttu-id="61525-181">Int32</span><span class="sxs-lookup"><span data-stu-id="61525-181">Int32</span></span>|<span data-ttu-id="61525-182">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="61525-182">Version of the device configuration.</span></span> <span data-ttu-id="61525-183">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="61525-183">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="61525-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="61525-184">Response</span></span>

<span data-ttu-id="61525-185">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="61525-185">If successful, this method returns a `201 Created` response code and a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61525-186">Exemplo</span><span class="sxs-lookup"><span data-stu-id="61525-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="61525-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61525-187">Request</span></span>

<span data-ttu-id="61525-188">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="61525-188">Here is an example of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="61525-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="61525-189">Response</span></span>

<span data-ttu-id="61525-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="61525-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



