---
title: Atualizar windowsDomainJoinConfiguration
description: Atualize as propriedades de um objeto windowsDomainJoinConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 66314179f65748abca432dcf4f41bab3c16ebd32
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410851"
---
# <a name="update-windowsdomainjoinconfiguration"></a><span data-ttu-id="c1463-103">Atualizar windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="c1463-103">Update windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="c1463-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="c1463-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c1463-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c1463-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c1463-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="c1463-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1463-107">Atualize as propriedades de um objeto [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c1463-107">Update the properties of a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c1463-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c1463-108">Prerequisites</span></span>
<span data-ttu-id="c1463-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1463-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1463-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c1463-111">Permission type</span></span>|<span data-ttu-id="c1463-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c1463-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1463-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c1463-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c1463-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="c1463-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="c1463-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1463-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="c1463-116">&nbsp; &nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="c1463-116">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="c1463-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1463-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c1463-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c1463-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1463-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c1463-119">Not supported.</span></span>|
|<span data-ttu-id="c1463-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c1463-120">Application</span></span>|<span data-ttu-id="c1463-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c1463-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1463-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c1463-122">HTTP Request</span></span>

<span data-ttu-id="c1463-123">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="c1463-123">**Device configuration**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

<span data-ttu-id="c1463-124">**Registro**</span><span class="sxs-lookup"><span data-stu-id="c1463-124">**Enrollment**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile/domainJoinConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="c1463-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c1463-125">Request headers</span></span>
|<span data-ttu-id="c1463-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c1463-126">Header</span></span>|<span data-ttu-id="c1463-127">Valor</span><span class="sxs-lookup"><span data-stu-id="c1463-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1463-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="c1463-128">Authorization</span></span>|<span data-ttu-id="c1463-129">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c1463-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1463-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c1463-130">Accept</span></span>|<span data-ttu-id="c1463-131">application/json</span><span class="sxs-lookup"><span data-stu-id="c1463-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1463-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c1463-132">Request body</span></span>
<span data-ttu-id="c1463-133">No corpo da solicitação, fornece uma representação JSON para o objeto [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c1463-133">In the request body, supply a JSON representation for the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>

<span data-ttu-id="c1463-134">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1463-134">The following table shows the properties that are required when you create the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span></span>

|<span data-ttu-id="c1463-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c1463-135">Property</span></span>|<span data-ttu-id="c1463-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="c1463-136">Type</span></span>|<span data-ttu-id="c1463-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1463-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1463-138">id</span><span class="sxs-lookup"><span data-stu-id="c1463-138">id</span></span>|<span data-ttu-id="c1463-139">String</span><span class="sxs-lookup"><span data-stu-id="c1463-139">String</span></span>|<span data-ttu-id="c1463-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c1463-140">Key of the entity.</span></span> <span data-ttu-id="c1463-141">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1463-141">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1463-142">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="c1463-142">**Device configuration**</span></span>|
|<span data-ttu-id="c1463-143">activeDirectoryDomainName</span><span class="sxs-lookup"><span data-stu-id="c1463-143">activeDirectoryDomainName</span></span>|<span data-ttu-id="c1463-144">String</span><span class="sxs-lookup"><span data-stu-id="c1463-144">String</span></span>|<span data-ttu-id="c1463-145">Nome de domínio Active Directory para ingressar.</span><span class="sxs-lookup"><span data-stu-id="c1463-145">Active Directory domain name to join.</span></span>|
|<span data-ttu-id="c1463-146">computerNameStaticPrefix</span><span class="sxs-lookup"><span data-stu-id="c1463-146">computerNameStaticPrefix</span></span>|<span data-ttu-id="c1463-147">String</span><span class="sxs-lookup"><span data-stu-id="c1463-147">String</span></span>|<span data-ttu-id="c1463-148">Fixo prefixo a ser usado para o nome do computador.</span><span class="sxs-lookup"><span data-stu-id="c1463-148">Fixed prefix to be used for computer name.</span></span>|
|<span data-ttu-id="c1463-149">computerNameSuffixRandomCharCount</span><span class="sxs-lookup"><span data-stu-id="c1463-149">computerNameSuffixRandomCharCount</span></span>|<span data-ttu-id="c1463-150">Int32</span><span class="sxs-lookup"><span data-stu-id="c1463-150">Int32</span></span>|<span data-ttu-id="c1463-151">Caracteres gerados dinamicamente usados como o sufixo de nome do computador.</span><span class="sxs-lookup"><span data-stu-id="c1463-151">Dynamically generated characters used as suffix for computer name.</span></span> <span data-ttu-id="c1463-152">Valores válidos 3 e 14</span><span class="sxs-lookup"><span data-stu-id="c1463-152">Valid values 3 to 14</span></span>|
|<span data-ttu-id="c1463-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c1463-153">createdDateTime</span></span>|<span data-ttu-id="c1463-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1463-154">DateTimeOffset</span></span>|<span data-ttu-id="c1463-155">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="c1463-155">DateTime the object was created.</span></span> <span data-ttu-id="c1463-156">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1463-156">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1463-157">description</span><span class="sxs-lookup"><span data-stu-id="c1463-157">description</span></span>|<span data-ttu-id="c1463-158">String</span><span class="sxs-lookup"><span data-stu-id="c1463-158">String</span></span>|<span data-ttu-id="c1463-159">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c1463-159">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c1463-160">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1463-160">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1463-161">displayName</span><span class="sxs-lookup"><span data-stu-id="c1463-161">displayName</span></span>|<span data-ttu-id="c1463-162">String</span><span class="sxs-lookup"><span data-stu-id="c1463-162">String</span></span>|<span data-ttu-id="c1463-163">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c1463-163">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c1463-164">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1463-164">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1463-165">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c1463-165">lastModifiedDateTime</span></span>|<span data-ttu-id="c1463-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1463-166">DateTimeOffset</span></span>|<span data-ttu-id="c1463-167">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="c1463-167">DateTime the object was last modified.</span></span> <span data-ttu-id="c1463-168">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1463-168">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1463-169">organizationalUnit</span><span class="sxs-lookup"><span data-stu-id="c1463-169">organizationalUnit</span></span>|<span data-ttu-id="c1463-170">String</span><span class="sxs-lookup"><span data-stu-id="c1463-170">String</span></span>|<span data-ttu-id="c1463-171">Unidade organizacional (UO) onde a conta de computador será criada.</span><span class="sxs-lookup"><span data-stu-id="c1463-171">Organizational unit (OU) where the computer account will be created.</span></span> <span data-ttu-id="c1463-172">Se esse parâmetro for NULL, será usado o contêiner de objeto de computador bem conhecido como publicado no domínio.</span><span class="sxs-lookup"><span data-stu-id="c1463-172">If this parameter is NULL, the well known computer object container will be used as published in the domain.</span></span>|
|<span data-ttu-id="c1463-173">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c1463-173">roleScopeTagIds</span></span>|<span data-ttu-id="c1463-174">String collection</span><span class="sxs-lookup"><span data-stu-id="c1463-174">String collection</span></span>|<span data-ttu-id="c1463-175">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="c1463-175">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c1463-176">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1463-176">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1463-177">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c1463-177">supportsScopeTags</span></span>|<span data-ttu-id="c1463-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1463-178">Boolean</span></span>|<span data-ttu-id="c1463-179">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="c1463-179">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c1463-180">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="c1463-180">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c1463-181">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="c1463-181">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c1463-182">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c1463-182">This property is read-only.</span></span> <span data-ttu-id="c1463-183">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1463-183">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1463-184">version</span><span class="sxs-lookup"><span data-stu-id="c1463-184">version</span></span>|<span data-ttu-id="c1463-185">Int32</span><span class="sxs-lookup"><span data-stu-id="c1463-185">Int32</span></span>|<span data-ttu-id="c1463-186">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c1463-186">Version of the device configuration.</span></span> <span data-ttu-id="c1463-187">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1463-187">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



<span data-ttu-id="c1463-188">Observação: Solicitar as propriedades de corpo suporte depende do contexto da chamada.</span><span class="sxs-lookup"><span data-stu-id="c1463-188">Note: Request body properties support depends on the context of the call.</span></span>  <span data-ttu-id="c1463-189">Nem todas as propriedades são adequadas para todos os fluxos de trabalho.</span><span class="sxs-lookup"><span data-stu-id="c1463-189">Not all properties are appropriate for all workflows.</span></span>

## <a name="response"></a><span data-ttu-id="c1463-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1463-190">Response</span></span>
<span data-ttu-id="c1463-191">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c1463-191">If successful, this method returns a `200 OK` response code and an updated [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1463-192">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c1463-192">Example</span></span>
### <a name="request"></a><span data-ttu-id="c1463-193">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c1463-193">Request</span></span>
<span data-ttu-id="c1463-194">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c1463-194">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c1463-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1463-195">Response</span></span>
<span data-ttu-id="c1463-196">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c1463-196">Here is an example of the response.</span></span> <span data-ttu-id="c1463-197">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="c1463-197">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c1463-198">Propriedades retornadas por chamadas reais variam de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="c1463-198">Properties returned by actual calls vary according to the context.</span></span>
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



