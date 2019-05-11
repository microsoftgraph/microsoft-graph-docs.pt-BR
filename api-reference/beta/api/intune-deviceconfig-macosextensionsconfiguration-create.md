---
title: Criar macOSExtensionsConfiguration
description: Criar um novo objeto macOSExtensionsConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3ec49d7fdd3adb84a05da0892a02c89e7e264707
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33922477"
---
# <a name="create-macosextensionsconfiguration"></a><span data-ttu-id="c185b-103">Criar macOSExtensionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="c185b-103">Create macOSExtensionsConfiguration</span></span>

> <span data-ttu-id="c185b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c185b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c185b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c185b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c185b-106">Criar um novo objeto [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c185b-106">Create a new [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c185b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c185b-107">Prerequisites</span></span>
<span data-ttu-id="c185b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c185b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c185b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c185b-110">Permission type</span></span>|<span data-ttu-id="c185b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c185b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c185b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c185b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c185b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c185b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c185b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c185b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c185b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c185b-115">Not supported.</span></span>|
|<span data-ttu-id="c185b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c185b-116">Application</span></span>|<span data-ttu-id="c185b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c185b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c185b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c185b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c185b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c185b-119">Request headers</span></span>
|<span data-ttu-id="c185b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c185b-120">Header</span></span>|<span data-ttu-id="c185b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c185b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c185b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c185b-122">Authorization</span></span>|<span data-ttu-id="c185b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c185b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c185b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c185b-124">Accept</span></span>|<span data-ttu-id="c185b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c185b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c185b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c185b-126">Request body</span></span>
<span data-ttu-id="c185b-127">No corpo da solicitação, forneça uma representação JSON do objeto macOSExtensionsConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c185b-127">In the request body, supply a JSON representation for the macOSExtensionsConfiguration object.</span></span>

<span data-ttu-id="c185b-128">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSExtensionsConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c185b-128">The following table shows the properties that are required when you create the macOSExtensionsConfiguration.</span></span>

|<span data-ttu-id="c185b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c185b-129">Property</span></span>|<span data-ttu-id="c185b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c185b-130">Type</span></span>|<span data-ttu-id="c185b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c185b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c185b-132">id</span><span class="sxs-lookup"><span data-stu-id="c185b-132">id</span></span>|<span data-ttu-id="c185b-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c185b-133">String</span></span>|<span data-ttu-id="c185b-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c185b-134">Key of the entity.</span></span> <span data-ttu-id="c185b-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c185b-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c185b-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c185b-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c185b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c185b-137">DateTimeOffset</span></span>|<span data-ttu-id="c185b-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="c185b-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c185b-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c185b-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c185b-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c185b-140">roleScopeTagIds</span></span>|<span data-ttu-id="c185b-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c185b-141">String collection</span></span>|<span data-ttu-id="c185b-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="c185b-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c185b-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c185b-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c185b-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c185b-144">supportsScopeTags</span></span>|<span data-ttu-id="c185b-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="c185b-145">Boolean</span></span>|<span data-ttu-id="c185b-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="c185b-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c185b-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="c185b-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c185b-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="c185b-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c185b-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c185b-149">This property is read-only.</span></span> <span data-ttu-id="c185b-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c185b-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c185b-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c185b-151">createdDateTime</span></span>|<span data-ttu-id="c185b-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c185b-152">DateTimeOffset</span></span>|<span data-ttu-id="c185b-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="c185b-153">DateTime the object was created.</span></span> <span data-ttu-id="c185b-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c185b-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c185b-155">description</span><span class="sxs-lookup"><span data-stu-id="c185b-155">description</span></span>|<span data-ttu-id="c185b-156">String</span><span class="sxs-lookup"><span data-stu-id="c185b-156">String</span></span>|<span data-ttu-id="c185b-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c185b-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c185b-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c185b-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c185b-159">displayName</span><span class="sxs-lookup"><span data-stu-id="c185b-159">displayName</span></span>|<span data-ttu-id="c185b-160">String</span><span class="sxs-lookup"><span data-stu-id="c185b-160">String</span></span>|<span data-ttu-id="c185b-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c185b-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c185b-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c185b-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c185b-163">versão</span><span class="sxs-lookup"><span data-stu-id="c185b-163">version</span></span>|<span data-ttu-id="c185b-164">Int32</span><span class="sxs-lookup"><span data-stu-id="c185b-164">Int32</span></span>|<span data-ttu-id="c185b-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c185b-165">Version of the device configuration.</span></span> <span data-ttu-id="c185b-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c185b-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c185b-167">kernelExtensionOverridesAllowed</span><span class="sxs-lookup"><span data-stu-id="c185b-167">kernelExtensionOverridesAllowed</span></span>|<span data-ttu-id="c185b-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="c185b-168">Boolean</span></span>|<span data-ttu-id="c185b-169">Se definido como true, os usuários podem aprovar extensões de kernel adicionais não explicitamente permitidas por perfis de configuração.</span><span class="sxs-lookup"><span data-stu-id="c185b-169">If set to true, users can approve additional kernel extensions not explicitly allowed by configurations profiles.</span></span>|
|<span data-ttu-id="c185b-170">kernelExtensionAllowedTeamIdentifiers</span><span class="sxs-lookup"><span data-stu-id="c185b-170">kernelExtensionAllowedTeamIdentifiers</span></span>|<span data-ttu-id="c185b-171">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c185b-171">String collection</span></span>|<span data-ttu-id="c185b-172">Todas as extensões de kernel assinadas com validade pelos identificadores de equipe nesta lista poderão ser carregadas.</span><span class="sxs-lookup"><span data-stu-id="c185b-172">All kernel extensions validly signed by the team identifiers in this list will be allowed to load.</span></span>|
|<span data-ttu-id="c185b-173">kernelExtensionsAllowed</span><span class="sxs-lookup"><span data-stu-id="c185b-173">kernelExtensionsAllowed</span></span>|<span data-ttu-id="c185b-174">coleção [macOSKernelExtension](../resources/intune-deviceconfig-macoskernelextension.md)</span><span class="sxs-lookup"><span data-stu-id="c185b-174">[macOSKernelExtension](../resources/intune-deviceconfig-macoskernelextension.md) collection</span></span>|<span data-ttu-id="c185b-175">Uma lista de extensões do kernel que terão permissão para carregar.</span><span class="sxs-lookup"><span data-stu-id="c185b-175">A list of kernel extensions that will be allowed to load.</span></span> <span data-ttu-id="c185b-176">.</span><span class="sxs-lookup"><span data-stu-id="c185b-176"></span></span> <span data-ttu-id="c185b-177">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="c185b-177">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="c185b-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="c185b-178">Response</span></span>
<span data-ttu-id="c185b-179">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c185b-179">If successful, this method returns a `201 Created` response code and a [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c185b-180">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c185b-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="c185b-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c185b-181">Request</span></span>
<span data-ttu-id="c185b-182">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c185b-182">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 610

{
  "@odata.type": "#microsoft.graph.macOSExtensionsConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "kernelExtensionOverridesAllowed": true,
  "kernelExtensionAllowedTeamIdentifiers": [
    "Kernel Extension Allowed Team Identifiers value"
  ],
  "kernelExtensionsAllowed": [
    {
      "@odata.type": "microsoft.graph.macOSKernelExtension",
      "teamIdentifier": "Team Identifier value",
      "bundleId": "Bundle Id value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="c185b-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="c185b-183">Response</span></span>
<span data-ttu-id="c185b-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c185b-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 782

{
  "@odata.type": "#microsoft.graph.macOSExtensionsConfiguration",
  "id": "c273f4f6-f4f6-c273-f6f4-73c2f6f473c2",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "kernelExtensionOverridesAllowed": true,
  "kernelExtensionAllowedTeamIdentifiers": [
    "Kernel Extension Allowed Team Identifiers value"
  ],
  "kernelExtensionsAllowed": [
    {
      "@odata.type": "microsoft.graph.macOSKernelExtension",
      "teamIdentifier": "Team Identifier value",
      "bundleId": "Bundle Id value"
    }
  ]
}
```




