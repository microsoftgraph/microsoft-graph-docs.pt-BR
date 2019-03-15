---
title: Atualizar windowsDomainJoinConfiguration
description: Atualiza as propriedades de um objeto windowsDomainJoinConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2e0700a630d3009520b290da269b213623bdf48a
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571659"
---
# <a name="update-windowsdomainjoinconfiguration"></a><span data-ttu-id="f9f8d-103">Atualizar windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="f9f8d-103">Update windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="f9f8d-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f9f8d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f9f8d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f9f8d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f9f8d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f9f8d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9f8d-107">Atualiza as propriedades de um objeto [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f9f8d-107">Update the properties of a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f9f8d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f9f8d-108">Prerequisites</span></span>
<span data-ttu-id="f9f8d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f9f8d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f9f8d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f9f8d-111">Permission type</span></span>|<span data-ttu-id="f9f8d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f9f8d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9f8d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f9f8d-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f9f8d-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="f9f8d-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="f9f8d-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9f8d-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="f9f8d-116">&nbsp;&nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="f9f8d-116">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="f9f8d-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9f8d-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f9f8d-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f9f8d-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9f8d-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9f8d-119">Not supported.</span></span>|
|<span data-ttu-id="f9f8d-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f9f8d-120">Application</span></span>|<span data-ttu-id="f9f8d-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9f8d-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9f8d-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f9f8d-122">HTTP Request</span></span>

<span data-ttu-id="f9f8d-123">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="f9f8d-123">**Device configuration**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

<span data-ttu-id="f9f8d-124">**Enrollmentid**</span><span class="sxs-lookup"><span data-stu-id="f9f8d-124">**Enrollment**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile/domainJoinConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="f9f8d-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f9f8d-125">Request headers</span></span>
|<span data-ttu-id="f9f8d-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f9f8d-126">Header</span></span>|<span data-ttu-id="f9f8d-127">Valor</span><span class="sxs-lookup"><span data-stu-id="f9f8d-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9f8d-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="f9f8d-128">Authorization</span></span>|<span data-ttu-id="f9f8d-129">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f9f8d-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9f8d-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f9f8d-130">Accept</span></span>|<span data-ttu-id="f9f8d-131">application/json</span><span class="sxs-lookup"><span data-stu-id="f9f8d-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9f8d-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f9f8d-132">Request body</span></span>
<span data-ttu-id="f9f8d-133">No corpo da solicitação, forneça uma representação JSON do objeto [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f9f8d-133">In the request body, supply a JSON representation for the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>

<span data-ttu-id="f9f8d-134">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f9f8d-134">The following table shows the properties that are required when you create the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span></span>

|<span data-ttu-id="f9f8d-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f9f8d-135">Property</span></span>|<span data-ttu-id="f9f8d-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9f8d-136">Type</span></span>|<span data-ttu-id="f9f8d-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9f8d-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9f8d-138">id</span><span class="sxs-lookup"><span data-stu-id="f9f8d-138">id</span></span>|<span data-ttu-id="f9f8d-139">String</span><span class="sxs-lookup"><span data-stu-id="f9f8d-139">String</span></span>|<span data-ttu-id="f9f8d-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f9f8d-140">Key of the entity.</span></span> <span data-ttu-id="f9f8d-141">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9f8d-141">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9f8d-142">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="f9f8d-142">**Device configuration**</span></span>|
|<span data-ttu-id="f9f8d-143">activeDirectoryDomainName</span><span class="sxs-lookup"><span data-stu-id="f9f8d-143">activeDirectoryDomainName</span></span>|<span data-ttu-id="f9f8d-144">String</span><span class="sxs-lookup"><span data-stu-id="f9f8d-144">String</span></span>|<span data-ttu-id="f9f8d-145">Nome de domínio do Active Directory para ingressar.</span><span class="sxs-lookup"><span data-stu-id="f9f8d-145">Active Directory domain name to join.</span></span>|
|<span data-ttu-id="f9f8d-146">computerNameStaticPrefix</span><span class="sxs-lookup"><span data-stu-id="f9f8d-146">computerNameStaticPrefix</span></span>|<span data-ttu-id="f9f8d-147">String</span><span class="sxs-lookup"><span data-stu-id="f9f8d-147">String</span></span>|<span data-ttu-id="f9f8d-148">Prefixo fixo a ser usado para o nome do computador.</span><span class="sxs-lookup"><span data-stu-id="f9f8d-148">Fixed prefix to be used for computer name.</span></span>|
|<span data-ttu-id="f9f8d-149">computerNameSuffixRandomCharCount</span><span class="sxs-lookup"><span data-stu-id="f9f8d-149">computerNameSuffixRandomCharCount</span></span>|<span data-ttu-id="f9f8d-150">Int32</span><span class="sxs-lookup"><span data-stu-id="f9f8d-150">Int32</span></span>|<span data-ttu-id="f9f8d-151">Caracteres gerados dinamicamente usados como sufixo para o nome do computador.</span><span class="sxs-lookup"><span data-stu-id="f9f8d-151">Dynamically generated characters used as suffix for computer name.</span></span> <span data-ttu-id="f9f8d-152">Valores válidos de 3 a 14</span><span class="sxs-lookup"><span data-stu-id="f9f8d-152">Valid values 3 to 14</span></span>|
|<span data-ttu-id="f9f8d-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f9f8d-153">createdDateTime</span></span>|<span data-ttu-id="f9f8d-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9f8d-154">DateTimeOffset</span></span>|<span data-ttu-id="f9f8d-155">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="f9f8d-155">DateTime the object was created.</span></span> <span data-ttu-id="f9f8d-156">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9f8d-156">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9f8d-157">descrição</span><span class="sxs-lookup"><span data-stu-id="f9f8d-157">description</span></span>|<span data-ttu-id="f9f8d-158">String</span><span class="sxs-lookup"><span data-stu-id="f9f8d-158">String</span></span>|<span data-ttu-id="f9f8d-159">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9f8d-159">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f9f8d-160">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9f8d-160">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9f8d-161">displayName</span><span class="sxs-lookup"><span data-stu-id="f9f8d-161">displayName</span></span>|<span data-ttu-id="f9f8d-162">String</span><span class="sxs-lookup"><span data-stu-id="f9f8d-162">String</span></span>|<span data-ttu-id="f9f8d-163">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9f8d-163">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f9f8d-164">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9f8d-164">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9f8d-165">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f9f8d-165">lastModifiedDateTime</span></span>|<span data-ttu-id="f9f8d-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9f8d-166">DateTimeOffset</span></span>|<span data-ttu-id="f9f8d-167">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="f9f8d-167">DateTime the object was last modified.</span></span> <span data-ttu-id="f9f8d-168">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9f8d-168">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9f8d-169">organizationalUnit</span><span class="sxs-lookup"><span data-stu-id="f9f8d-169">organizationalUnit</span></span>|<span data-ttu-id="f9f8d-170">String</span><span class="sxs-lookup"><span data-stu-id="f9f8d-170">String</span></span>|<span data-ttu-id="f9f8d-171">Unidade organizacional (UO) em que a conta de computador será criada.</span><span class="sxs-lookup"><span data-stu-id="f9f8d-171">Organizational unit (OU) where the computer account will be created.</span></span> <span data-ttu-id="f9f8d-172">Se esse parâmetro for NULL, o contêiner do objeto de computador conhecido será usado como publicado no domínio.</span><span class="sxs-lookup"><span data-stu-id="f9f8d-172">If this parameter is NULL, the well known computer object container will be used as published in the domain.</span></span>|
|<span data-ttu-id="f9f8d-173">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f9f8d-173">roleScopeTagIds</span></span>|<span data-ttu-id="f9f8d-174">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9f8d-174">String collection</span></span>|<span data-ttu-id="f9f8d-175">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="f9f8d-175">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f9f8d-176">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9f8d-176">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9f8d-177">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f9f8d-177">supportsScopeTags</span></span>|<span data-ttu-id="f9f8d-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="f9f8d-178">Boolean</span></span>|<span data-ttu-id="f9f8d-179">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="f9f8d-179">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f9f8d-180">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="f9f8d-180">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f9f8d-181">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="f9f8d-181">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f9f8d-182">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f8d-182">This property is read-only.</span></span> <span data-ttu-id="f9f8d-183">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9f8d-183">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9f8d-184">versão</span><span class="sxs-lookup"><span data-stu-id="f9f8d-184">version</span></span>|<span data-ttu-id="f9f8d-185">Int32</span><span class="sxs-lookup"><span data-stu-id="f9f8d-185">Int32</span></span>|<span data-ttu-id="f9f8d-186">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9f8d-186">Version of the device configuration.</span></span> <span data-ttu-id="f9f8d-187">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9f8d-187">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



<span data-ttu-id="f9f8d-188">Observação: o suporte às propriedades do corpo da solicitação depende do contexto da chamada.</span><span class="sxs-lookup"><span data-stu-id="f9f8d-188">Note: Request body properties support depends on the context of the call.</span></span>  <span data-ttu-id="f9f8d-189">Nem todas as propriedades são apropriadas para todos os fluxos de trabalho.</span><span class="sxs-lookup"><span data-stu-id="f9f8d-189">Not all properties are appropriate for all workflows.</span></span>

## <a name="response"></a><span data-ttu-id="f9f8d-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9f8d-190">Response</span></span>
<span data-ttu-id="f9f8d-191">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f9f8d-191">If successful, this method returns a `200 OK` response code and an updated [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9f8d-192">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f9f8d-192">Example</span></span>
### <a name="request"></a><span data-ttu-id="f9f8d-193">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9f8d-193">Request</span></span>
<span data-ttu-id="f9f8d-194">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f9f8d-194">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f9f8d-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9f8d-195">Response</span></span>
<span data-ttu-id="f9f8d-196">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f9f8d-196">Here is an example of the response.</span></span> <span data-ttu-id="f9f8d-197">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="f9f8d-197">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f9f8d-198">As propriedades retornadas por chamadas reais variam de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="f9f8d-198">Properties returned by actual calls vary according to the context.</span></span>
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



