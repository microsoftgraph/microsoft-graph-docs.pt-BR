---
title: Atualizar windowsDomainJoinConfiguration
description: Atualize as propriedades de um objeto windowsDomainJoinConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 568d4c8fa440822e32a6c21770bb33cdeaa9ec18
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831651"
---
# <a name="update-windowsdomainjoinconfiguration"></a><span data-ttu-id="c40c1-103">Atualizar windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="c40c1-103">Update windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="c40c1-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c40c1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c40c1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c40c1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c40c1-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c40c1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c40c1-107">Atualize as propriedades de um objeto [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c40c1-107">Update the properties of a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c40c1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c40c1-108">Prerequisites</span></span>
<span data-ttu-id="c40c1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c40c1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c40c1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c40c1-111">Permission type</span></span>|<span data-ttu-id="c40c1-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c40c1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c40c1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c40c1-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c40c1-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="c40c1-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="c40c1-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c40c1-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="c40c1-116">&nbsp; &nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="c40c1-116">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="c40c1-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c40c1-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c40c1-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c40c1-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c40c1-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c40c1-119">Not supported.</span></span>|
|<span data-ttu-id="c40c1-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c40c1-120">Application</span></span>|<span data-ttu-id="c40c1-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c40c1-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c40c1-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c40c1-122">HTTP Request</span></span>

<span data-ttu-id="c40c1-123">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="c40c1-123">**Device configuration**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

<span data-ttu-id="c40c1-124">**Registro**</span><span class="sxs-lookup"><span data-stu-id="c40c1-124">**Enrollment**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile/domainJoinConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="c40c1-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c40c1-125">Request headers</span></span>
|<span data-ttu-id="c40c1-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c40c1-126">Header</span></span>|<span data-ttu-id="c40c1-127">Valor</span><span class="sxs-lookup"><span data-stu-id="c40c1-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c40c1-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="c40c1-128">Authorization</span></span>|<span data-ttu-id="c40c1-129">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c40c1-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c40c1-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c40c1-130">Accept</span></span>|<span data-ttu-id="c40c1-131">application/json</span><span class="sxs-lookup"><span data-stu-id="c40c1-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c40c1-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c40c1-132">Request body</span></span>
<span data-ttu-id="c40c1-133">No corpo da solicitação, fornece uma representação JSON para o objeto [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c40c1-133">In the request body, supply a JSON representation for the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>

<span data-ttu-id="c40c1-134">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c40c1-134">The following table shows the properties that are required when you create the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span></span>

|<span data-ttu-id="c40c1-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c40c1-135">Property</span></span>|<span data-ttu-id="c40c1-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="c40c1-136">Type</span></span>|<span data-ttu-id="c40c1-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="c40c1-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c40c1-138">id</span><span class="sxs-lookup"><span data-stu-id="c40c1-138">id</span></span>|<span data-ttu-id="c40c1-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c40c1-139">String</span></span>|<span data-ttu-id="c40c1-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c40c1-140">Key of the entity.</span></span> <span data-ttu-id="c40c1-141">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c40c1-141">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c40c1-142">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="c40c1-142">**Device configuration**</span></span>|
|<span data-ttu-id="c40c1-143">activeDirectoryDomainName</span><span class="sxs-lookup"><span data-stu-id="c40c1-143">activeDirectoryDomainName</span></span>|<span data-ttu-id="c40c1-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c40c1-144">String</span></span>|<span data-ttu-id="c40c1-145">Nome de domínio Active Directory para ingressar.</span><span class="sxs-lookup"><span data-stu-id="c40c1-145">Active Directory domain name to join.</span></span>|
|<span data-ttu-id="c40c1-146">computerNameStaticPrefix</span><span class="sxs-lookup"><span data-stu-id="c40c1-146">computerNameStaticPrefix</span></span>|<span data-ttu-id="c40c1-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c40c1-147">String</span></span>|<span data-ttu-id="c40c1-148">Fixo prefixo a ser usado para o nome do computador.</span><span class="sxs-lookup"><span data-stu-id="c40c1-148">Fixed prefix to be used for computer name.</span></span>|
|<span data-ttu-id="c40c1-149">computerNameSuffixRandomCharCount</span><span class="sxs-lookup"><span data-stu-id="c40c1-149">computerNameSuffixRandomCharCount</span></span>|<span data-ttu-id="c40c1-150">Int32</span><span class="sxs-lookup"><span data-stu-id="c40c1-150">Int32</span></span>|<span data-ttu-id="c40c1-151">Caracteres gerados dinamicamente usados como o sufixo de nome do computador.</span><span class="sxs-lookup"><span data-stu-id="c40c1-151">Dynamically generated characters used as suffix for computer name.</span></span> <span data-ttu-id="c40c1-152">Valores válidos 3 e 14</span><span class="sxs-lookup"><span data-stu-id="c40c1-152">Valid values 3 to 14</span></span>|
|<span data-ttu-id="c40c1-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c40c1-153">createdDateTime</span></span>|<span data-ttu-id="c40c1-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c40c1-154">DateTimeOffset</span></span>|<span data-ttu-id="c40c1-155">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="c40c1-155">DateTime the object was created.</span></span> <span data-ttu-id="c40c1-156">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c40c1-156">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c40c1-157">description</span><span class="sxs-lookup"><span data-stu-id="c40c1-157">description</span></span>|<span data-ttu-id="c40c1-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c40c1-158">String</span></span>|<span data-ttu-id="c40c1-159">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c40c1-159">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c40c1-160">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c40c1-160">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c40c1-161">displayName</span><span class="sxs-lookup"><span data-stu-id="c40c1-161">displayName</span></span>|<span data-ttu-id="c40c1-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c40c1-162">String</span></span>|<span data-ttu-id="c40c1-163">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c40c1-163">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c40c1-164">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c40c1-164">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c40c1-165">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c40c1-165">lastModifiedDateTime</span></span>|<span data-ttu-id="c40c1-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c40c1-166">DateTimeOffset</span></span>|<span data-ttu-id="c40c1-167">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="c40c1-167">DateTime the object was last modified.</span></span> <span data-ttu-id="c40c1-168">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c40c1-168">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c40c1-169">organizationalUnit</span><span class="sxs-lookup"><span data-stu-id="c40c1-169">organizationalUnit</span></span>|<span data-ttu-id="c40c1-170">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c40c1-170">String</span></span>|<span data-ttu-id="c40c1-171">Unidade organizacional (UO) onde a conta de computador será criada.</span><span class="sxs-lookup"><span data-stu-id="c40c1-171">Organizational unit (OU) where the computer account will be created.</span></span> <span data-ttu-id="c40c1-172">Se esse parâmetro for NULL, será usado o contêiner de objeto de computador bem conhecido como publicado no domínio.</span><span class="sxs-lookup"><span data-stu-id="c40c1-172">If this parameter is NULL, the well known computer object container will be used as published in the domain.</span></span>|
|<span data-ttu-id="c40c1-173">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c40c1-173">roleScopeTagIds</span></span>|<span data-ttu-id="c40c1-174">String collection</span><span class="sxs-lookup"><span data-stu-id="c40c1-174">String collection</span></span>|<span data-ttu-id="c40c1-175">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="c40c1-175">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c40c1-176">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c40c1-176">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c40c1-177">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c40c1-177">supportsScopeTags</span></span>|<span data-ttu-id="c40c1-178">Booliano</span><span class="sxs-lookup"><span data-stu-id="c40c1-178">Boolean</span></span>|<span data-ttu-id="c40c1-179">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="c40c1-179">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c40c1-180">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="c40c1-180">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c40c1-181">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="c40c1-181">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c40c1-182">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c40c1-182">This property is read-only.</span></span> <span data-ttu-id="c40c1-183">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c40c1-183">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c40c1-184">version</span><span class="sxs-lookup"><span data-stu-id="c40c1-184">version</span></span>|<span data-ttu-id="c40c1-185">Int32</span><span class="sxs-lookup"><span data-stu-id="c40c1-185">Int32</span></span>|<span data-ttu-id="c40c1-186">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c40c1-186">Version of the device configuration.</span></span> <span data-ttu-id="c40c1-187">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c40c1-187">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



<span data-ttu-id="c40c1-188">Observação: Solicitar as propriedades de corpo suporte depende do contexto da chamada.</span><span class="sxs-lookup"><span data-stu-id="c40c1-188">Note: Request body properties support depends on the context of the call.</span></span>  <span data-ttu-id="c40c1-189">Nem todas as propriedades são adequadas para todos os fluxos de trabalho.</span><span class="sxs-lookup"><span data-stu-id="c40c1-189">Not all properties are appropriate for all workflows.</span></span>

## <a name="response"></a><span data-ttu-id="c40c1-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="c40c1-190">Response</span></span>
<span data-ttu-id="c40c1-191">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c40c1-191">If successful, this method returns a `200 OK` response code and an updated [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c40c1-192">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c40c1-192">Example</span></span>
### <a name="request"></a><span data-ttu-id="c40c1-193">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c40c1-193">Request</span></span>
<span data-ttu-id="c40c1-194">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c40c1-194">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c40c1-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="c40c1-195">Response</span></span>
<span data-ttu-id="c40c1-196">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c40c1-196">Here is an example of the response.</span></span> <span data-ttu-id="c40c1-197">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="c40c1-197">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c40c1-198">Propriedades retornadas por chamadas reais variam de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="c40c1-198">Properties returned by actual calls vary according to the context.</span></span>
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



