---
title: Atualizar windowsDomainJoinConfiguration
description: Atualiza as propriedades de um objeto windowsDomainJoinConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c75d0ff64e8e2b6c4467dda79938809c49753409
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457934"
---
# <a name="update-windowsdomainjoinconfiguration"></a><span data-ttu-id="5ed9e-103">Atualizar windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="5ed9e-103">Update windowsDomainJoinConfiguration</span></span>

<span data-ttu-id="5ed9e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5ed9e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5ed9e-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5ed9e-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5ed9e-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5ed9e-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5ed9e-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5ed9e-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ed9e-108">Atualiza as propriedades de um objeto [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="5ed9e-108">Update the properties of a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5ed9e-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5ed9e-109">Prerequisites</span></span>
<span data-ttu-id="5ed9e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ed9e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ed9e-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ed9e-112">Permission type</span></span>|<span data-ttu-id="5ed9e-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5ed9e-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ed9e-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ed9e-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="5ed9e-115">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="5ed9e-115">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="5ed9e-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ed9e-116">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="5ed9e-117">&nbsp;&nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="5ed9e-117">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="5ed9e-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ed9e-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5ed9e-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ed9e-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ed9e-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ed9e-120">Not supported.</span></span>|
|<span data-ttu-id="5ed9e-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ed9e-121">Application</span></span>||
| <span data-ttu-id="5ed9e-122">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="5ed9e-122">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="5ed9e-123">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ed9e-123">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="5ed9e-124">&nbsp;&nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="5ed9e-124">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="5ed9e-125">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ed9e-125">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ed9e-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ed9e-126">HTTP Request</span></span>

<span data-ttu-id="5ed9e-127">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="5ed9e-127">**Device configuration**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

<span data-ttu-id="5ed9e-128">**Enrollmentid**</span><span class="sxs-lookup"><span data-stu-id="5ed9e-128">**Enrollment**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile/domainJoinConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="5ed9e-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ed9e-129">Request headers</span></span>
|<span data-ttu-id="5ed9e-130">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5ed9e-130">Header</span></span>|<span data-ttu-id="5ed9e-131">Valor</span><span class="sxs-lookup"><span data-stu-id="5ed9e-131">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ed9e-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ed9e-132">Authorization</span></span>|<span data-ttu-id="5ed9e-133">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ed9e-133">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ed9e-134">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5ed9e-134">Accept</span></span>|<span data-ttu-id="5ed9e-135">application/json</span><span class="sxs-lookup"><span data-stu-id="5ed9e-135">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ed9e-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ed9e-136">Request body</span></span>
<span data-ttu-id="5ed9e-137">No corpo da solicitação, forneça uma representação JSON do objeto [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="5ed9e-137">In the request body, supply a JSON representation for the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>

<span data-ttu-id="5ed9e-138">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5ed9e-138">The following table shows the properties that are required when you create the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span></span>

|<span data-ttu-id="5ed9e-139">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5ed9e-139">Property</span></span>|<span data-ttu-id="5ed9e-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ed9e-140">Type</span></span>|<span data-ttu-id="5ed9e-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ed9e-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ed9e-142">id</span><span class="sxs-lookup"><span data-stu-id="5ed9e-142">id</span></span>|<span data-ttu-id="5ed9e-143">String</span><span class="sxs-lookup"><span data-stu-id="5ed9e-143">String</span></span>|<span data-ttu-id="5ed9e-144">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5ed9e-144">Key of the entity.</span></span> <span data-ttu-id="5ed9e-145">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ed9e-145">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ed9e-146">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="5ed9e-146">**Device configuration**</span></span>|
|<span data-ttu-id="5ed9e-147">activeDirectoryDomainName</span><span class="sxs-lookup"><span data-stu-id="5ed9e-147">activeDirectoryDomainName</span></span>|<span data-ttu-id="5ed9e-148">String</span><span class="sxs-lookup"><span data-stu-id="5ed9e-148">String</span></span>|<span data-ttu-id="5ed9e-149">Nome de domínio do Active Directory para ingressar.</span><span class="sxs-lookup"><span data-stu-id="5ed9e-149">Active Directory domain name to join.</span></span>|
|<span data-ttu-id="5ed9e-150">computerNameStaticPrefix</span><span class="sxs-lookup"><span data-stu-id="5ed9e-150">computerNameStaticPrefix</span></span>|<span data-ttu-id="5ed9e-151">String</span><span class="sxs-lookup"><span data-stu-id="5ed9e-151">String</span></span>|<span data-ttu-id="5ed9e-152">Prefixo fixo a ser usado para o nome do computador.</span><span class="sxs-lookup"><span data-stu-id="5ed9e-152">Fixed prefix to be used for computer name.</span></span>|
|<span data-ttu-id="5ed9e-153">computerNameSuffixRandomCharCount</span><span class="sxs-lookup"><span data-stu-id="5ed9e-153">computerNameSuffixRandomCharCount</span></span>|<span data-ttu-id="5ed9e-154">Int32</span><span class="sxs-lookup"><span data-stu-id="5ed9e-154">Int32</span></span>|<span data-ttu-id="5ed9e-155">Caracteres gerados dinamicamente usados como sufixo para o nome do computador.</span><span class="sxs-lookup"><span data-stu-id="5ed9e-155">Dynamically generated characters used as suffix for computer name.</span></span> <span data-ttu-id="5ed9e-156">Valores válidos de 3 a 14</span><span class="sxs-lookup"><span data-stu-id="5ed9e-156">Valid values 3 to 14</span></span>|
|<span data-ttu-id="5ed9e-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5ed9e-157">createdDateTime</span></span>|<span data-ttu-id="5ed9e-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ed9e-158">DateTimeOffset</span></span>|<span data-ttu-id="5ed9e-159">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="5ed9e-159">DateTime the object was created.</span></span> <span data-ttu-id="5ed9e-160">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ed9e-160">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ed9e-161">description</span><span class="sxs-lookup"><span data-stu-id="5ed9e-161">description</span></span>|<span data-ttu-id="5ed9e-162">String</span><span class="sxs-lookup"><span data-stu-id="5ed9e-162">String</span></span>|<span data-ttu-id="5ed9e-163">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5ed9e-163">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5ed9e-164">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ed9e-164">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ed9e-165">displayName</span><span class="sxs-lookup"><span data-stu-id="5ed9e-165">displayName</span></span>|<span data-ttu-id="5ed9e-166">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ed9e-166">String</span></span>|<span data-ttu-id="5ed9e-167">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5ed9e-167">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5ed9e-168">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ed9e-168">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ed9e-169">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5ed9e-169">lastModifiedDateTime</span></span>|<span data-ttu-id="5ed9e-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ed9e-170">DateTimeOffset</span></span>|<span data-ttu-id="5ed9e-171">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="5ed9e-171">DateTime the object was last modified.</span></span> <span data-ttu-id="5ed9e-172">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ed9e-172">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ed9e-173">organizationalUnit</span><span class="sxs-lookup"><span data-stu-id="5ed9e-173">organizationalUnit</span></span>|<span data-ttu-id="5ed9e-174">String</span><span class="sxs-lookup"><span data-stu-id="5ed9e-174">String</span></span>|<span data-ttu-id="5ed9e-175">Unidade organizacional (UO) em que a conta de computador será criada.</span><span class="sxs-lookup"><span data-stu-id="5ed9e-175">Organizational unit (OU) where the computer account will be created.</span></span> <span data-ttu-id="5ed9e-176">Se esse parâmetro for NULL, o contêiner do objeto de computador conhecido será usado como publicado no domínio.</span><span class="sxs-lookup"><span data-stu-id="5ed9e-176">If this parameter is NULL, the well known computer object container will be used as published in the domain.</span></span>|
|<span data-ttu-id="5ed9e-177">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5ed9e-177">roleScopeTagIds</span></span>|<span data-ttu-id="5ed9e-178">String collection</span><span class="sxs-lookup"><span data-stu-id="5ed9e-178">String collection</span></span>|<span data-ttu-id="5ed9e-179">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="5ed9e-179">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5ed9e-180">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ed9e-180">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ed9e-181">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="5ed9e-181">supportsScopeTags</span></span>|<span data-ttu-id="5ed9e-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ed9e-182">Boolean</span></span>|<span data-ttu-id="5ed9e-183">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="5ed9e-183">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5ed9e-184">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="5ed9e-184">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5ed9e-185">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="5ed9e-185">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5ed9e-186">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5ed9e-186">This property is read-only.</span></span> <span data-ttu-id="5ed9e-187">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ed9e-187">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ed9e-188">versão</span><span class="sxs-lookup"><span data-stu-id="5ed9e-188">version</span></span>|<span data-ttu-id="5ed9e-189">Int32</span><span class="sxs-lookup"><span data-stu-id="5ed9e-189">Int32</span></span>|<span data-ttu-id="5ed9e-190">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5ed9e-190">Version of the device configuration.</span></span> <span data-ttu-id="5ed9e-191">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ed9e-191">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|



<span data-ttu-id="5ed9e-192">Observação: o suporte às propriedades do corpo da solicitação depende do contexto da chamada.</span><span class="sxs-lookup"><span data-stu-id="5ed9e-192">Note: Request body properties support depends on the context of the call.</span></span>  <span data-ttu-id="5ed9e-193">Nem todas as propriedades são apropriadas para todos os fluxos de trabalho.</span><span class="sxs-lookup"><span data-stu-id="5ed9e-193">Not all properties are appropriate for all workflows.</span></span>

## <a name="response"></a><span data-ttu-id="5ed9e-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ed9e-194">Response</span></span>
<span data-ttu-id="5ed9e-195">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ed9e-195">If successful, this method returns a `200 OK` response code and an updated [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ed9e-196">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5ed9e-196">Example</span></span>
### <a name="request"></a><span data-ttu-id="5ed9e-197">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ed9e-197">Request</span></span>
<span data-ttu-id="5ed9e-198">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ed9e-198">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5ed9e-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ed9e-199">Response</span></span>
<span data-ttu-id="5ed9e-200">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ed9e-200">Here is an example of the response.</span></span> <span data-ttu-id="5ed9e-201">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="5ed9e-201">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="5ed9e-202">As propriedades retornadas por chamadas reais variam de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="5ed9e-202">Properties returned by actual calls vary according to the context.</span></span>
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











