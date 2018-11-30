---
title: Atualizar windowsDomainJoinConfiguration
description: Atualize as propriedades de um objeto windowsDomainJoinConfiguration.
ms.openlocfilehash: 78e082aa7baba3e1e1483800d6971a2c376e2234
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037957"
---
# <a name="update-windowsdomainjoinconfiguration"></a><span data-ttu-id="0a0a3-103">Atualizar windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="0a0a3-103">Update windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="0a0a3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0a0a3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0a0a3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0a0a3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0a0a3-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0a0a3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0a0a3-107">Atualize as propriedades de um objeto [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="0a0a3-107">Update the properties of a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0a0a3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0a0a3-108">Prerequisites</span></span>
<span data-ttu-id="0a0a3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a0a3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a0a3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0a0a3-111">Permission type</span></span>|<span data-ttu-id="0a0a3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0a0a3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a0a3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0a0a3-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="0a0a3-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="0a0a3-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="0a0a3-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a0a3-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="0a0a3-116">&nbsp; &nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="0a0a3-116">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="0a0a3-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a0a3-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0a0a3-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0a0a3-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a0a3-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0a0a3-119">Not supported.</span></span>|
|<span data-ttu-id="0a0a3-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0a0a3-120">Application</span></span>|<span data-ttu-id="0a0a3-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0a0a3-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a0a3-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0a0a3-122">HTTP Request</span></span>

<span data-ttu-id="0a0a3-123">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="0a0a3-123">**Device configuration**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

<span data-ttu-id="0a0a3-124">**Registro**</span><span class="sxs-lookup"><span data-stu-id="0a0a3-124">**Enrollment**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile/domainJoinConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="0a0a3-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0a0a3-125">Request headers</span></span>
|<span data-ttu-id="0a0a3-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0a0a3-126">Header</span></span>|<span data-ttu-id="0a0a3-127">Valor</span><span class="sxs-lookup"><span data-stu-id="0a0a3-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a0a3-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="0a0a3-128">Authorization</span></span>|<span data-ttu-id="0a0a3-129">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0a0a3-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a0a3-130">Accept</span><span class="sxs-lookup"><span data-stu-id="0a0a3-130">Accept</span></span>|<span data-ttu-id="0a0a3-131">application/json</span><span class="sxs-lookup"><span data-stu-id="0a0a3-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a0a3-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0a0a3-132">Request body</span></span>
<span data-ttu-id="0a0a3-133">No corpo da solicitação, fornece uma representação JSON para o objeto [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="0a0a3-133">In the request body, supply a JSON representation for the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>

<span data-ttu-id="0a0a3-134">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0a0a3-134">The following table shows the properties that are required when you create the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span></span>

|<span data-ttu-id="0a0a3-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0a0a3-135">Property</span></span>|<span data-ttu-id="0a0a3-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="0a0a3-136">Type</span></span>|<span data-ttu-id="0a0a3-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a0a3-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a0a3-138">id</span><span class="sxs-lookup"><span data-stu-id="0a0a3-138">id</span></span>|<span data-ttu-id="0a0a3-139">String</span><span class="sxs-lookup"><span data-stu-id="0a0a3-139">String</span></span>|<span data-ttu-id="0a0a3-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0a0a3-140">Key of the entity.</span></span> <span data-ttu-id="0a0a3-141">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0a0a3-141">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a0a3-142">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="0a0a3-142">**Device configuration**</span></span>|
|<span data-ttu-id="0a0a3-143">activeDirectoryDomainName</span><span class="sxs-lookup"><span data-stu-id="0a0a3-143">activeDirectoryDomainName</span></span>|<span data-ttu-id="0a0a3-144">String</span><span class="sxs-lookup"><span data-stu-id="0a0a3-144">String</span></span>|<span data-ttu-id="0a0a3-145">Nome de domínio Active Directory para ingressar.</span><span class="sxs-lookup"><span data-stu-id="0a0a3-145">Active Directory domain name to join.</span></span>|
|<span data-ttu-id="0a0a3-146">computerNameStaticPrefix</span><span class="sxs-lookup"><span data-stu-id="0a0a3-146">computerNameStaticPrefix</span></span>|<span data-ttu-id="0a0a3-147">String</span><span class="sxs-lookup"><span data-stu-id="0a0a3-147">String</span></span>|<span data-ttu-id="0a0a3-148">Fixo prefixo a ser usado para o nome do computador.</span><span class="sxs-lookup"><span data-stu-id="0a0a3-148">Fixed prefix to be used for computer name.</span></span>|
|<span data-ttu-id="0a0a3-149">computerNameSuffixRandomCharCount</span><span class="sxs-lookup"><span data-stu-id="0a0a3-149">computerNameSuffixRandomCharCount</span></span>|<span data-ttu-id="0a0a3-150">Int32</span><span class="sxs-lookup"><span data-stu-id="0a0a3-150">Int32</span></span>|<span data-ttu-id="0a0a3-151">Caracteres gerados dinamicamente usados como o sufixo de nome do computador.</span><span class="sxs-lookup"><span data-stu-id="0a0a3-151">Dynamically generated characters used as suffix for computer name.</span></span> <span data-ttu-id="0a0a3-152">Valores válidos 3 e 14</span><span class="sxs-lookup"><span data-stu-id="0a0a3-152">Valid values 3 to 14</span></span>|
|<span data-ttu-id="0a0a3-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0a0a3-153">createdDateTime</span></span>|<span data-ttu-id="0a0a3-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a0a3-154">DateTimeOffset</span></span>|<span data-ttu-id="0a0a3-155">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="0a0a3-155">DateTime the object was created.</span></span> <span data-ttu-id="0a0a3-156">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0a0a3-156">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a0a3-157">description</span><span class="sxs-lookup"><span data-stu-id="0a0a3-157">description</span></span>|<span data-ttu-id="0a0a3-158">String</span><span class="sxs-lookup"><span data-stu-id="0a0a3-158">String</span></span>|<span data-ttu-id="0a0a3-159">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0a0a3-159">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0a0a3-160">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0a0a3-160">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a0a3-161">displayName</span><span class="sxs-lookup"><span data-stu-id="0a0a3-161">displayName</span></span>|<span data-ttu-id="0a0a3-162">String</span><span class="sxs-lookup"><span data-stu-id="0a0a3-162">String</span></span>|<span data-ttu-id="0a0a3-163">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0a0a3-163">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0a0a3-164">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0a0a3-164">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a0a3-165">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0a0a3-165">lastModifiedDateTime</span></span>|<span data-ttu-id="0a0a3-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a0a3-166">DateTimeOffset</span></span>|<span data-ttu-id="0a0a3-167">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="0a0a3-167">DateTime the object was last modified.</span></span> <span data-ttu-id="0a0a3-168">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0a0a3-168">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a0a3-169">organizationalUnit</span><span class="sxs-lookup"><span data-stu-id="0a0a3-169">organizationalUnit</span></span>|<span data-ttu-id="0a0a3-170">String</span><span class="sxs-lookup"><span data-stu-id="0a0a3-170">String</span></span>|<span data-ttu-id="0a0a3-171">Unidade organizacional (UO) onde a conta de computador será criada.</span><span class="sxs-lookup"><span data-stu-id="0a0a3-171">Organizational unit (OU) where the computer account will be created.</span></span> <span data-ttu-id="0a0a3-172">Se esse parâmetro for NULL, será usado o contêiner de objeto de computador bem conhecido como publicado no domínio.</span><span class="sxs-lookup"><span data-stu-id="0a0a3-172">If this parameter is NULL, the well known computer object container will be used as published in the domain.</span></span>|
|<span data-ttu-id="0a0a3-173">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0a0a3-173">roleScopeTagIds</span></span>|<span data-ttu-id="0a0a3-174">String collection</span><span class="sxs-lookup"><span data-stu-id="0a0a3-174">String collection</span></span>|<span data-ttu-id="0a0a3-175">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="0a0a3-175">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0a0a3-176">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0a0a3-176">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a0a3-177">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0a0a3-177">supportsScopeTags</span></span>|<span data-ttu-id="0a0a3-178">Booliano</span><span class="sxs-lookup"><span data-stu-id="0a0a3-178">Boolean</span></span>|<span data-ttu-id="0a0a3-179">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="0a0a3-179">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0a0a3-180">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="0a0a3-180">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0a0a3-181">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="0a0a3-181">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0a0a3-182">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0a0a3-182">This property is read-only.</span></span> <span data-ttu-id="0a0a3-183">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0a0a3-183">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a0a3-184">version</span><span class="sxs-lookup"><span data-stu-id="0a0a3-184">version</span></span>|<span data-ttu-id="0a0a3-185">Int32</span><span class="sxs-lookup"><span data-stu-id="0a0a3-185">Int32</span></span>|<span data-ttu-id="0a0a3-186">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0a0a3-186">Version of the device configuration.</span></span> <span data-ttu-id="0a0a3-187">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0a0a3-187">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



<span data-ttu-id="0a0a3-188">Observação: Solicitar as propriedades de corpo suporte depende do contexto da chamada.</span><span class="sxs-lookup"><span data-stu-id="0a0a3-188">Note: Request body properties support depends on the context of the call.</span></span>  <span data-ttu-id="0a0a3-189">Nem todas as propriedades são adequadas para todos os fluxos de trabalho.</span><span class="sxs-lookup"><span data-stu-id="0a0a3-189">Not all properties are appropriate for all workflows.</span></span>

## <a name="response"></a><span data-ttu-id="0a0a3-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a0a3-190">Response</span></span>
<span data-ttu-id="0a0a3-191">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0a0a3-191">If successful, this method returns a `200 OK` response code and an updated [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a0a3-192">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0a0a3-192">Example</span></span>
### <a name="request"></a><span data-ttu-id="0a0a3-193">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0a0a3-193">Request</span></span>
<span data-ttu-id="0a0a3-194">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0a0a3-194">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0a0a3-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a0a3-195">Response</span></span>
<span data-ttu-id="0a0a3-196">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0a0a3-196">Here is an example of the response.</span></span> <span data-ttu-id="0a0a3-197">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="0a0a3-197">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="0a0a3-198">Propriedades retornadas por chamadas reais variam de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="0a0a3-198">Properties returned by actual calls vary according to the context.</span></span>
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



