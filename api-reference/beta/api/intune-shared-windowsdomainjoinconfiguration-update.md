---
title: Atualizar windowsDomainJoinConfiguration
description: Atualiza as propriedades de um objeto windowsDomainJoinConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1caedda2f05f146d1db1cf8b6d2b070824c0b951
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174148"
---
# <a name="update-windowsdomainjoinconfiguration"></a><span data-ttu-id="21d47-103">Atualizar windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="21d47-103">Update windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="21d47-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="21d47-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="21d47-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="21d47-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="21d47-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="21d47-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21d47-107">Atualiza as propriedades de um objeto [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="21d47-107">Update the properties of a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="21d47-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="21d47-108">Prerequisites</span></span>
<span data-ttu-id="21d47-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21d47-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference).</span></span>

|<span data-ttu-id="21d47-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="21d47-111">Permission type</span></span>|<span data-ttu-id="21d47-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="21d47-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21d47-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="21d47-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="21d47-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="21d47-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="21d47-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21d47-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="21d47-116">&nbsp; &nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="21d47-116">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="21d47-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21d47-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="21d47-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="21d47-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21d47-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21d47-119">Not supported.</span></span>|
|<span data-ttu-id="21d47-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="21d47-120">Application</span></span>|<span data-ttu-id="21d47-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21d47-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21d47-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="21d47-122">HTTP Request</span></span>

<span data-ttu-id="21d47-123">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="21d47-123">**Device configuration**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

<span data-ttu-id="21d47-124">**Registro**</span><span class="sxs-lookup"><span data-stu-id="21d47-124">**Enrollment**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile/domainJoinConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="21d47-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="21d47-125">Request headers</span></span>
|<span data-ttu-id="21d47-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="21d47-126">Header</span></span>|<span data-ttu-id="21d47-127">Valor</span><span class="sxs-lookup"><span data-stu-id="21d47-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21d47-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="21d47-128">Authorization</span></span>|<span data-ttu-id="21d47-129">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="21d47-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21d47-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="21d47-130">Accept</span></span>|<span data-ttu-id="21d47-131">application/json</span><span class="sxs-lookup"><span data-stu-id="21d47-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21d47-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="21d47-132">Request body</span></span>
<span data-ttu-id="21d47-133">No corpo da solicitação, forneça uma representação JSON do objeto [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="21d47-133">In the request body, supply a JSON representation for the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>

<span data-ttu-id="21d47-134">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="21d47-134">The following table shows the properties that are required when you create the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span></span>

|<span data-ttu-id="21d47-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="21d47-135">Property</span></span>|<span data-ttu-id="21d47-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="21d47-136">Type</span></span>|<span data-ttu-id="21d47-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="21d47-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21d47-138">id</span><span class="sxs-lookup"><span data-stu-id="21d47-138">id</span></span>|<span data-ttu-id="21d47-139">String</span><span class="sxs-lookup"><span data-stu-id="21d47-139">String</span></span>|<span data-ttu-id="21d47-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="21d47-140">Key of the entity.</span></span> <span data-ttu-id="21d47-141">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="21d47-141">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="21d47-142">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="21d47-142">**Device configuration**</span></span>|
|<span data-ttu-id="21d47-143">activeDirectoryDomainName</span><span class="sxs-lookup"><span data-stu-id="21d47-143">activeDirectoryDomainName</span></span>|<span data-ttu-id="21d47-144">String</span><span class="sxs-lookup"><span data-stu-id="21d47-144">String</span></span>|<span data-ttu-id="21d47-145">Nome de domínio do Active Directory para ingressar.</span><span class="sxs-lookup"><span data-stu-id="21d47-145">Active Directory domain name to join.</span></span>|
|<span data-ttu-id="21d47-146">computerNameStaticPrefix</span><span class="sxs-lookup"><span data-stu-id="21d47-146">computerNameStaticPrefix</span></span>|<span data-ttu-id="21d47-147">String</span><span class="sxs-lookup"><span data-stu-id="21d47-147">String</span></span>|<span data-ttu-id="21d47-148">Prefixo fixo a ser usado para o nome do computador.</span><span class="sxs-lookup"><span data-stu-id="21d47-148">Fixed prefix to be used for computer name.</span></span>|
|<span data-ttu-id="21d47-149">computerNameSuffixRandomCharCount</span><span class="sxs-lookup"><span data-stu-id="21d47-149">computerNameSuffixRandomCharCount</span></span>|<span data-ttu-id="21d47-150">Int32</span><span class="sxs-lookup"><span data-stu-id="21d47-150">Int32</span></span>|<span data-ttu-id="21d47-151">Caracteres gerados dinamicamente usados como sufixo para o nome do computador.</span><span class="sxs-lookup"><span data-stu-id="21d47-151">Dynamically generated characters used as suffix for computer name.</span></span> <span data-ttu-id="21d47-152">Valores válidos de 3 a 14</span><span class="sxs-lookup"><span data-stu-id="21d47-152">Valid values 3 to 14</span></span>|
|<span data-ttu-id="21d47-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="21d47-153">createdDateTime</span></span>|<span data-ttu-id="21d47-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21d47-154">DateTimeOffset</span></span>|<span data-ttu-id="21d47-155">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="21d47-155">DateTime the object was created.</span></span> <span data-ttu-id="21d47-156">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="21d47-156">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="21d47-157">description</span><span class="sxs-lookup"><span data-stu-id="21d47-157">description</span></span>|<span data-ttu-id="21d47-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="21d47-158">String</span></span>|<span data-ttu-id="21d47-159">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="21d47-159">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="21d47-160">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="21d47-160">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="21d47-161">displayName</span><span class="sxs-lookup"><span data-stu-id="21d47-161">displayName</span></span>|<span data-ttu-id="21d47-162">String</span><span class="sxs-lookup"><span data-stu-id="21d47-162">String</span></span>|<span data-ttu-id="21d47-163">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="21d47-163">Admin provided name of the device configuration.</span></span> <span data-ttu-id="21d47-164">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="21d47-164">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="21d47-165">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="21d47-165">lastModifiedDateTime</span></span>|<span data-ttu-id="21d47-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21d47-166">DateTimeOffset</span></span>|<span data-ttu-id="21d47-167">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="21d47-167">DateTime the object was last modified.</span></span> <span data-ttu-id="21d47-168">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="21d47-168">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="21d47-169">organizationalUnit</span><span class="sxs-lookup"><span data-stu-id="21d47-169">organizationalUnit</span></span>|<span data-ttu-id="21d47-170">String</span><span class="sxs-lookup"><span data-stu-id="21d47-170">String</span></span>|<span data-ttu-id="21d47-171">Unidade organizacional (UO) em que a conta de computador será criada.</span><span class="sxs-lookup"><span data-stu-id="21d47-171">Organizational unit (OU) where the computer account will be created.</span></span> <span data-ttu-id="21d47-172">Se esse parâmetro for NULL, o contêiner do objeto de computador conhecido será usado como publicado no domínio.</span><span class="sxs-lookup"><span data-stu-id="21d47-172">If this parameter is NULL, the well known computer object container will be used as published in the domain.</span></span>|
|<span data-ttu-id="21d47-173">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="21d47-173">roleScopeTagIds</span></span>|<span data-ttu-id="21d47-174">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="21d47-174">String collection</span></span>|<span data-ttu-id="21d47-175">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="21d47-175">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="21d47-176">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="21d47-176">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="21d47-177">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="21d47-177">supportsScopeTags</span></span>|<span data-ttu-id="21d47-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="21d47-178">Boolean</span></span>|<span data-ttu-id="21d47-179">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="21d47-179">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="21d47-180">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="21d47-180">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="21d47-181">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="21d47-181">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="21d47-182">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="21d47-182">This property is read-only.</span></span> <span data-ttu-id="21d47-183">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="21d47-183">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="21d47-184">version</span><span class="sxs-lookup"><span data-stu-id="21d47-184">version</span></span>|<span data-ttu-id="21d47-185">Int32</span><span class="sxs-lookup"><span data-stu-id="21d47-185">Int32</span></span>|<span data-ttu-id="21d47-186">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="21d47-186">Version of the device configuration.</span></span> <span data-ttu-id="21d47-187">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="21d47-187">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



<span data-ttu-id="21d47-188">Observação: o suporte às propriedades do corpo da solicitação depende do contexto da chamada.</span><span class="sxs-lookup"><span data-stu-id="21d47-188">Note: Request body properties support depends on the context of the call.</span></span>  <span data-ttu-id="21d47-189">Nem todas as propriedades são apropriadas para todos os fluxos de trabalho.</span><span class="sxs-lookup"><span data-stu-id="21d47-189">Not all properties are appropriate for all workflows.</span></span>

## <a name="response"></a><span data-ttu-id="21d47-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="21d47-190">Response</span></span>
<span data-ttu-id="21d47-191">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="21d47-191">If successful, this method returns a `200 OK` response code and an updated [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21d47-192">Exemplo</span><span class="sxs-lookup"><span data-stu-id="21d47-192">Example</span></span>
### <a name="request"></a><span data-ttu-id="21d47-193">Solicitação</span><span class="sxs-lookup"><span data-stu-id="21d47-193">Request</span></span>
<span data-ttu-id="21d47-194">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="21d47-194">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="21d47-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="21d47-195">Response</span></span>
<span data-ttu-id="21d47-196">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="21d47-196">Here is an example of the response.</span></span> <span data-ttu-id="21d47-197">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="21d47-197">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="21d47-198">As propriedades retornadas por chamadas reais variam de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="21d47-198">Properties returned by actual calls vary according to the context.</span></span>
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



