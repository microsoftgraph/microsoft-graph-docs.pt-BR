---
title: Atualizar windowsDomainJoinConfiguration
description: Atualiza as propriedades de um objeto windowsDomainJoinConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cadf31d0d7ada9b8e94ea17f326e102d8404c00e
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939343"
---
# <a name="update-windowsdomainjoinconfiguration"></a><span data-ttu-id="f83d2-103">Atualizar windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="f83d2-103">Update windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="f83d2-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f83d2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f83d2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f83d2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f83d2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f83d2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f83d2-107">Atualiza as propriedades de um objeto [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f83d2-107">Update the properties of a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f83d2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f83d2-108">Prerequisites</span></span>
<span data-ttu-id="f83d2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f83d2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f83d2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f83d2-111">Permission type</span></span>|<span data-ttu-id="f83d2-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f83d2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f83d2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f83d2-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f83d2-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="f83d2-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="f83d2-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f83d2-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="f83d2-116">&nbsp;&nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="f83d2-116">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="f83d2-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f83d2-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f83d2-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f83d2-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f83d2-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f83d2-119">Not supported.</span></span>|
|<span data-ttu-id="f83d2-120">Application</span><span class="sxs-lookup"><span data-stu-id="f83d2-120">Application</span></span>||
| <span data-ttu-id="f83d2-121">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="f83d2-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="f83d2-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f83d2-122">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="f83d2-123">&nbsp;&nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="f83d2-123">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="f83d2-124">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f83d2-124">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f83d2-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f83d2-125">HTTP Request</span></span>

<span data-ttu-id="f83d2-126">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="f83d2-126">**Device configuration**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

<span data-ttu-id="f83d2-127">**Enrollmentid**</span><span class="sxs-lookup"><span data-stu-id="f83d2-127">**Enrollment**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile/domainJoinConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="f83d2-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f83d2-128">Request headers</span></span>
|<span data-ttu-id="f83d2-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f83d2-129">Header</span></span>|<span data-ttu-id="f83d2-130">Valor</span><span class="sxs-lookup"><span data-stu-id="f83d2-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f83d2-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="f83d2-131">Authorization</span></span>|<span data-ttu-id="f83d2-132">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f83d2-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f83d2-133">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f83d2-133">Accept</span></span>|<span data-ttu-id="f83d2-134">application/json</span><span class="sxs-lookup"><span data-stu-id="f83d2-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f83d2-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f83d2-135">Request body</span></span>
<span data-ttu-id="f83d2-136">No corpo da solicitação, forneça uma representação JSON do objeto [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f83d2-136">In the request body, supply a JSON representation for the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>

<span data-ttu-id="f83d2-137">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f83d2-137">The following table shows the properties that are required when you create the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span></span>

|<span data-ttu-id="f83d2-138">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f83d2-138">Property</span></span>|<span data-ttu-id="f83d2-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="f83d2-139">Type</span></span>|<span data-ttu-id="f83d2-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="f83d2-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f83d2-141">id</span><span class="sxs-lookup"><span data-stu-id="f83d2-141">id</span></span>|<span data-ttu-id="f83d2-142">String</span><span class="sxs-lookup"><span data-stu-id="f83d2-142">String</span></span>|<span data-ttu-id="f83d2-143">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f83d2-143">Key of the entity.</span></span> <span data-ttu-id="f83d2-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f83d2-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f83d2-145">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="f83d2-145">**Device configuration**</span></span>|
|<span data-ttu-id="f83d2-146">activeDirectoryDomainName</span><span class="sxs-lookup"><span data-stu-id="f83d2-146">activeDirectoryDomainName</span></span>|<span data-ttu-id="f83d2-147">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="f83d2-147">String</span></span>|<span data-ttu-id="f83d2-148">Nome de domínio do Active Directory para ingressar.</span><span class="sxs-lookup"><span data-stu-id="f83d2-148">Active Directory domain name to join.</span></span>|
|<span data-ttu-id="f83d2-149">computerNameStaticPrefix</span><span class="sxs-lookup"><span data-stu-id="f83d2-149">computerNameStaticPrefix</span></span>|<span data-ttu-id="f83d2-150">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="f83d2-150">String</span></span>|<span data-ttu-id="f83d2-151">Prefixo fixo a ser usado para o nome do computador.</span><span class="sxs-lookup"><span data-stu-id="f83d2-151">Fixed prefix to be used for computer name.</span></span>|
|<span data-ttu-id="f83d2-152">computerNameSuffixRandomCharCount</span><span class="sxs-lookup"><span data-stu-id="f83d2-152">computerNameSuffixRandomCharCount</span></span>|<span data-ttu-id="f83d2-153">Int32</span><span class="sxs-lookup"><span data-stu-id="f83d2-153">Int32</span></span>|<span data-ttu-id="f83d2-154">Caracteres gerados dinamicamente usados como sufixo para o nome do computador.</span><span class="sxs-lookup"><span data-stu-id="f83d2-154">Dynamically generated characters used as suffix for computer name.</span></span> <span data-ttu-id="f83d2-155">Valores válidos de 3 a 14</span><span class="sxs-lookup"><span data-stu-id="f83d2-155">Valid values 3 to 14</span></span>|
|<span data-ttu-id="f83d2-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f83d2-156">createdDateTime</span></span>|<span data-ttu-id="f83d2-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f83d2-157">DateTimeOffset</span></span>|<span data-ttu-id="f83d2-158">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="f83d2-158">DateTime the object was created.</span></span> <span data-ttu-id="f83d2-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f83d2-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f83d2-160">description</span><span class="sxs-lookup"><span data-stu-id="f83d2-160">description</span></span>|<span data-ttu-id="f83d2-161">String</span><span class="sxs-lookup"><span data-stu-id="f83d2-161">String</span></span>|<span data-ttu-id="f83d2-162">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f83d2-162">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f83d2-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f83d2-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f83d2-164">displayName</span><span class="sxs-lookup"><span data-stu-id="f83d2-164">displayName</span></span>|<span data-ttu-id="f83d2-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f83d2-165">String</span></span>|<span data-ttu-id="f83d2-166">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f83d2-166">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f83d2-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f83d2-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f83d2-168">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f83d2-168">lastModifiedDateTime</span></span>|<span data-ttu-id="f83d2-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f83d2-169">DateTimeOffset</span></span>|<span data-ttu-id="f83d2-170">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="f83d2-170">DateTime the object was last modified.</span></span> <span data-ttu-id="f83d2-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f83d2-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f83d2-172">organizationalUnit</span><span class="sxs-lookup"><span data-stu-id="f83d2-172">organizationalUnit</span></span>|<span data-ttu-id="f83d2-173">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="f83d2-173">String</span></span>|<span data-ttu-id="f83d2-174">Unidade organizacional (UO) em que a conta de computador será criada.</span><span class="sxs-lookup"><span data-stu-id="f83d2-174">Organizational unit (OU) where the computer account will be created.</span></span> <span data-ttu-id="f83d2-175">Se esse parâmetro for NULL, o contêiner do objeto de computador conhecido será usado como publicado no domínio.</span><span class="sxs-lookup"><span data-stu-id="f83d2-175">If this parameter is NULL, the well known computer object container will be used as published in the domain.</span></span>|
|<span data-ttu-id="f83d2-176">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f83d2-176">roleScopeTagIds</span></span>|<span data-ttu-id="f83d2-177">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f83d2-177">String collection</span></span>|<span data-ttu-id="f83d2-178">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="f83d2-178">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f83d2-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f83d2-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f83d2-180">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f83d2-180">supportsScopeTags</span></span>|<span data-ttu-id="f83d2-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="f83d2-181">Boolean</span></span>|<span data-ttu-id="f83d2-182">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="f83d2-182">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f83d2-183">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="f83d2-183">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f83d2-184">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="f83d2-184">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f83d2-185">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f83d2-185">This property is read-only.</span></span> <span data-ttu-id="f83d2-186">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f83d2-186">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f83d2-187">versão</span><span class="sxs-lookup"><span data-stu-id="f83d2-187">version</span></span>|<span data-ttu-id="f83d2-188">Int32</span><span class="sxs-lookup"><span data-stu-id="f83d2-188">Int32</span></span>|<span data-ttu-id="f83d2-189">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f83d2-189">Version of the device configuration.</span></span> <span data-ttu-id="f83d2-190">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f83d2-190">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|



<span data-ttu-id="f83d2-191">Observação: o suporte às propriedades do corpo da solicitação depende do contexto da chamada.</span><span class="sxs-lookup"><span data-stu-id="f83d2-191">Note: Request body properties support depends on the context of the call.</span></span>  <span data-ttu-id="f83d2-192">Nem todas as propriedades são apropriadas para todos os fluxos de trabalho.</span><span class="sxs-lookup"><span data-stu-id="f83d2-192">Not all properties are appropriate for all workflows.</span></span>

## <a name="response"></a><span data-ttu-id="f83d2-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="f83d2-193">Response</span></span>
<span data-ttu-id="f83d2-194">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f83d2-194">If successful, this method returns a `200 OK` response code and an updated [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f83d2-195">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f83d2-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="f83d2-196">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f83d2-196">Request</span></span>
<span data-ttu-id="f83d2-197">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f83d2-197">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f83d2-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="f83d2-198">Response</span></span>
<span data-ttu-id="f83d2-199">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f83d2-199">Here is an example of the response.</span></span> <span data-ttu-id="f83d2-200">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="f83d2-200">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f83d2-201">As propriedades retornadas por chamadas reais variam de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="f83d2-201">Properties returned by actual calls vary according to the context.</span></span>
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











