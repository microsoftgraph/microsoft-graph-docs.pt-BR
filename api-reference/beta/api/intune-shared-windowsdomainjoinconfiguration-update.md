---
title: Atualizar windowsDomainJoinConfiguration
description: Atualize as propriedades de um objeto windowsDomainJoinConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ac8732ff9e9b6ee32a36205af919331372154236
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864757"
---
# <a name="update-windowsdomainjoinconfiguration"></a><span data-ttu-id="6af13-103">Atualizar windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="6af13-103">Update windowsDomainJoinConfiguration</span></span>

<span data-ttu-id="6af13-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6af13-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6af13-105">**Importante:** APIs na versão /beta do Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6af13-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6af13-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6af13-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6af13-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6af13-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6af13-108">Atualize as propriedades de um [objeto windowsDomainJoinConfiguration.](../resources/intune-shared-windowsdomainjoinconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6af13-108">Update the properties of a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6af13-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6af13-109">Prerequisites</span></span>
<span data-ttu-id="6af13-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6af13-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6af13-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6af13-112">Permission type</span></span>|<span data-ttu-id="6af13-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6af13-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6af13-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6af13-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="6af13-115">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="6af13-115">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="6af13-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6af13-116">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="6af13-117">&nbsp;&nbsp; **Inscrição**</span><span class="sxs-lookup"><span data-stu-id="6af13-117">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="6af13-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6af13-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6af13-119">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6af13-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6af13-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6af13-120">Not supported.</span></span>|
|<span data-ttu-id="6af13-121">Application</span><span class="sxs-lookup"><span data-stu-id="6af13-121">Application</span></span>||
| <span data-ttu-id="6af13-122">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="6af13-122">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="6af13-123">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6af13-123">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="6af13-124">&nbsp;&nbsp; **Inscrição**</span><span class="sxs-lookup"><span data-stu-id="6af13-124">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="6af13-125">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6af13-125">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6af13-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6af13-126">HTTP Request</span></span>

<span data-ttu-id="6af13-127">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="6af13-127">**Device configuration**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

<span data-ttu-id="6af13-128">**Inscrição**</span><span class="sxs-lookup"><span data-stu-id="6af13-128">**Enrollment**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile/domainJoinConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="6af13-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6af13-129">Request headers</span></span>
|<span data-ttu-id="6af13-130">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6af13-130">Header</span></span>|<span data-ttu-id="6af13-131">Valor</span><span class="sxs-lookup"><span data-stu-id="6af13-131">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6af13-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="6af13-132">Authorization</span></span>|<span data-ttu-id="6af13-133">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6af13-133">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6af13-134">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6af13-134">Accept</span></span>|<span data-ttu-id="6af13-135">application/json</span><span class="sxs-lookup"><span data-stu-id="6af13-135">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6af13-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6af13-136">Request body</span></span>
<span data-ttu-id="6af13-137">No corpo da solicitação, fornece uma representação JSON para o [objeto windowsDomainJoinConfiguration.](../resources/intune-shared-windowsdomainjoinconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6af13-137">In the request body, supply a JSON representation for the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>

<span data-ttu-id="6af13-138">A tabela a seguir mostra as propriedades que são necessárias ao criar [o windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6af13-138">The following table shows the properties that are required when you create the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span></span>

|<span data-ttu-id="6af13-139">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6af13-139">Property</span></span>|<span data-ttu-id="6af13-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="6af13-140">Type</span></span>|<span data-ttu-id="6af13-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="6af13-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6af13-142">id</span><span class="sxs-lookup"><span data-stu-id="6af13-142">id</span></span>|<span data-ttu-id="6af13-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6af13-143">String</span></span>|<span data-ttu-id="6af13-144">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6af13-144">Key of the entity.</span></span> <span data-ttu-id="6af13-145">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6af13-145">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6af13-146">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="6af13-146">**Device configuration**</span></span>|
|<span data-ttu-id="6af13-147">activeDirectoryDomainName</span><span class="sxs-lookup"><span data-stu-id="6af13-147">activeDirectoryDomainName</span></span>|<span data-ttu-id="6af13-148">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="6af13-148">String</span></span>|<span data-ttu-id="6af13-149">Nome de domínio do Active Directory para ingressar.</span><span class="sxs-lookup"><span data-stu-id="6af13-149">Active Directory domain name to join.</span></span>|
|<span data-ttu-id="6af13-150">computerNameStaticPrefix</span><span class="sxs-lookup"><span data-stu-id="6af13-150">computerNameStaticPrefix</span></span>|<span data-ttu-id="6af13-151">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="6af13-151">String</span></span>|<span data-ttu-id="6af13-152">Prefixo fixo a ser usado para nome do computador.</span><span class="sxs-lookup"><span data-stu-id="6af13-152">Fixed prefix to be used for computer name.</span></span>|
|<span data-ttu-id="6af13-153">computerNameSuffixRandomCharCount</span><span class="sxs-lookup"><span data-stu-id="6af13-153">computerNameSuffixRandomCharCount</span></span>|<span data-ttu-id="6af13-154">Int32</span><span class="sxs-lookup"><span data-stu-id="6af13-154">Int32</span></span>|<span data-ttu-id="6af13-155">Caracteres gerados dinamicamente usados como sufixo para o nome do computador.</span><span class="sxs-lookup"><span data-stu-id="6af13-155">Dynamically generated characters used as suffix for computer name.</span></span> <span data-ttu-id="6af13-156">Valores válidos de 3 a 14</span><span class="sxs-lookup"><span data-stu-id="6af13-156">Valid values 3 to 14</span></span>|
|<span data-ttu-id="6af13-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6af13-157">createdDateTime</span></span>|<span data-ttu-id="6af13-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6af13-158">DateTimeOffset</span></span>|<span data-ttu-id="6af13-159">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="6af13-159">DateTime the object was created.</span></span> <span data-ttu-id="6af13-160">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6af13-160">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6af13-161">description</span><span class="sxs-lookup"><span data-stu-id="6af13-161">description</span></span>|<span data-ttu-id="6af13-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6af13-162">String</span></span>|<span data-ttu-id="6af13-163">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6af13-163">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6af13-164">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6af13-164">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6af13-165">displayName</span><span class="sxs-lookup"><span data-stu-id="6af13-165">displayName</span></span>|<span data-ttu-id="6af13-166">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6af13-166">String</span></span>|<span data-ttu-id="6af13-167">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6af13-167">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6af13-168">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6af13-168">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6af13-169">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6af13-169">lastModifiedDateTime</span></span>|<span data-ttu-id="6af13-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6af13-170">DateTimeOffset</span></span>|<span data-ttu-id="6af13-171">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="6af13-171">DateTime the object was last modified.</span></span> <span data-ttu-id="6af13-172">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6af13-172">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6af13-173">organizationalUnit</span><span class="sxs-lookup"><span data-stu-id="6af13-173">organizationalUnit</span></span>|<span data-ttu-id="6af13-174">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="6af13-174">String</span></span>|<span data-ttu-id="6af13-175">Unidade organizacional (OU) onde a conta do computador será criada.</span><span class="sxs-lookup"><span data-stu-id="6af13-175">Organizational unit (OU) where the computer account will be created.</span></span> <span data-ttu-id="6af13-176">Se esse parâmetro for NULL, o contêiner de objeto de computador conhecido será usado como publicado no domínio.</span><span class="sxs-lookup"><span data-stu-id="6af13-176">If this parameter is NULL, the well known computer object container will be used as published in the domain.</span></span>|
|<span data-ttu-id="6af13-177">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6af13-177">roleScopeTagIds</span></span>|<span data-ttu-id="6af13-178">Coleção String</span><span class="sxs-lookup"><span data-stu-id="6af13-178">String collection</span></span>|<span data-ttu-id="6af13-179">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="6af13-179">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6af13-180">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6af13-180">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6af13-181">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6af13-181">supportsScopeTags</span></span>|<span data-ttu-id="6af13-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="6af13-182">Boolean</span></span>|<span data-ttu-id="6af13-183">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="6af13-183">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6af13-184">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="6af13-184">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6af13-185">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="6af13-185">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6af13-186">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6af13-186">This property is read-only.</span></span> <span data-ttu-id="6af13-187">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6af13-187">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6af13-188">versão</span><span class="sxs-lookup"><span data-stu-id="6af13-188">version</span></span>|<span data-ttu-id="6af13-189">Int32</span><span class="sxs-lookup"><span data-stu-id="6af13-189">Int32</span></span>|<span data-ttu-id="6af13-190">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6af13-190">Version of the device configuration.</span></span> <span data-ttu-id="6af13-191">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6af13-191">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|



<span data-ttu-id="6af13-192">Observação: o suporte às propriedades do corpo de solicitação depende do contexto da chamada.</span><span class="sxs-lookup"><span data-stu-id="6af13-192">Note: Request body properties support depends on the context of the call.</span></span>  <span data-ttu-id="6af13-193">Nem todas as propriedades são apropriadas para todos os fluxos de trabalho.</span><span class="sxs-lookup"><span data-stu-id="6af13-193">Not all properties are appropriate for all workflows.</span></span>

## <a name="response"></a><span data-ttu-id="6af13-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="6af13-194">Response</span></span>
<span data-ttu-id="6af13-195">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6af13-195">If successful, this method returns a `200 OK` response code and an updated [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6af13-196">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6af13-196">Example</span></span>
### <a name="request"></a><span data-ttu-id="6af13-197">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6af13-197">Request</span></span>
<span data-ttu-id="6af13-198">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6af13-198">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 344

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "computerNameStaticPrefix": "Computer Name Static Prefix value",
  "computerNameSuffixRandomCharCount": 1,
  "activeDirectoryDomainName": "Active Directory Domain Name value"
}
```

### <a name="response"></a><span data-ttu-id="6af13-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="6af13-199">Response</span></span>
<span data-ttu-id="6af13-200">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6af13-200">Here is an example of the response.</span></span> <span data-ttu-id="6af13-201">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="6af13-201">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="6af13-202">As propriedades retornadas por chamadas reais variam de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="6af13-202">Properties returned by actual calls vary according to the context.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 521

{
  "@odata.type": "#microsoft.graph.windowsDomainJoinConfiguration",
  "id": "40118d08-8d08-4011-088d-1140088d1140",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "computerNameStaticPrefix": "Computer Name Static Prefix value",
  "computerNameSuffixRandomCharCount": 1,
  "activeDirectoryDomainName": "Active Directory Domain Name value"
}
```










