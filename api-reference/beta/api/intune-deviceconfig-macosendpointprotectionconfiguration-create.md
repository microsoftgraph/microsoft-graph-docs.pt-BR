---
title: Criar macOSEndpointProtectionConfiguration
description: Criar um novo objeto macOSEndpointProtectionConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d78a111aa81700940a93493c4093e276f7ffc323
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33922795"
---
# <a name="create-macosendpointprotectionconfiguration"></a><span data-ttu-id="de512-103">Criar macOSEndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="de512-103">Create macOSEndpointProtectionConfiguration</span></span>

> <span data-ttu-id="de512-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="de512-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de512-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="de512-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de512-106">Criar um novo objeto [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="de512-106">Create a new [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="de512-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="de512-107">Prerequisites</span></span>
<span data-ttu-id="de512-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de512-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de512-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="de512-110">Permission type</span></span>|<span data-ttu-id="de512-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="de512-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de512-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="de512-112">Delegated (work or school account)</span></span>|<span data-ttu-id="de512-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de512-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="de512-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="de512-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de512-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de512-115">Not supported.</span></span>|
|<span data-ttu-id="de512-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="de512-116">Application</span></span>|<span data-ttu-id="de512-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de512-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="de512-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="de512-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="de512-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="de512-119">Request headers</span></span>
|<span data-ttu-id="de512-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="de512-120">Header</span></span>|<span data-ttu-id="de512-121">Valor</span><span class="sxs-lookup"><span data-stu-id="de512-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de512-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="de512-122">Authorization</span></span>|<span data-ttu-id="de512-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de512-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de512-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="de512-124">Accept</span></span>|<span data-ttu-id="de512-125">application/json</span><span class="sxs-lookup"><span data-stu-id="de512-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de512-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="de512-126">Request body</span></span>
<span data-ttu-id="de512-127">No corpo da solicitação, forneça uma representação JSON do objeto macOSEndpointProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="de512-127">In the request body, supply a JSON representation for the macOSEndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="de512-128">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSEndpointProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="de512-128">The following table shows the properties that are required when you create the macOSEndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="de512-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="de512-129">Property</span></span>|<span data-ttu-id="de512-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="de512-130">Type</span></span>|<span data-ttu-id="de512-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="de512-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de512-132">id</span><span class="sxs-lookup"><span data-stu-id="de512-132">id</span></span>|<span data-ttu-id="de512-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de512-133">String</span></span>|<span data-ttu-id="de512-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="de512-134">Key of the entity.</span></span> <span data-ttu-id="de512-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de512-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de512-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="de512-136">lastModifiedDateTime</span></span>|<span data-ttu-id="de512-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de512-137">DateTimeOffset</span></span>|<span data-ttu-id="de512-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="de512-138">DateTime the object was last modified.</span></span> <span data-ttu-id="de512-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de512-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de512-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="de512-140">roleScopeTagIds</span></span>|<span data-ttu-id="de512-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="de512-141">String collection</span></span>|<span data-ttu-id="de512-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="de512-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="de512-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de512-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de512-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="de512-144">supportsScopeTags</span></span>|<span data-ttu-id="de512-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="de512-145">Boolean</span></span>|<span data-ttu-id="de512-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="de512-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="de512-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="de512-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="de512-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="de512-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="de512-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de512-149">This property is read-only.</span></span> <span data-ttu-id="de512-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de512-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de512-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="de512-151">createdDateTime</span></span>|<span data-ttu-id="de512-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de512-152">DateTimeOffset</span></span>|<span data-ttu-id="de512-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="de512-153">DateTime the object was created.</span></span> <span data-ttu-id="de512-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de512-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de512-155">description</span><span class="sxs-lookup"><span data-stu-id="de512-155">description</span></span>|<span data-ttu-id="de512-156">String</span><span class="sxs-lookup"><span data-stu-id="de512-156">String</span></span>|<span data-ttu-id="de512-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de512-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="de512-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de512-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de512-159">displayName</span><span class="sxs-lookup"><span data-stu-id="de512-159">displayName</span></span>|<span data-ttu-id="de512-160">String</span><span class="sxs-lookup"><span data-stu-id="de512-160">String</span></span>|<span data-ttu-id="de512-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de512-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="de512-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de512-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de512-163">versão</span><span class="sxs-lookup"><span data-stu-id="de512-163">version</span></span>|<span data-ttu-id="de512-164">Int32</span><span class="sxs-lookup"><span data-stu-id="de512-164">Int32</span></span>|<span data-ttu-id="de512-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de512-165">Version of the device configuration.</span></span> <span data-ttu-id="de512-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de512-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de512-167">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="de512-167">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="de512-168">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="de512-168">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="de512-169">Configuração de sistema e privacidade que determina quais locais de download os aplicativos podem ser executados em um dispositivo macOS.</span><span class="sxs-lookup"><span data-stu-id="de512-169">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="de512-170">Os valores possíveis são: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span><span class="sxs-lookup"><span data-stu-id="de512-170">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="de512-171">gatekeeperBlockOverride</span><span class="sxs-lookup"><span data-stu-id="de512-171">gatekeeperBlockOverride</span></span>|<span data-ttu-id="de512-172">Booliano</span><span class="sxs-lookup"><span data-stu-id="de512-172">Boolean</span></span>|<span data-ttu-id="de512-173">Se definido como true, a substituição do usuário para gatekeeper será desabilitada.</span><span class="sxs-lookup"><span data-stu-id="de512-173">If set to true, the user override for Gatekeeper will be disabled.</span></span>|
|<span data-ttu-id="de512-174">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="de512-174">firewallEnabled</span></span>|<span data-ttu-id="de512-175">Booliano</span><span class="sxs-lookup"><span data-stu-id="de512-175">Boolean</span></span>|<span data-ttu-id="de512-176">Se o firewall deve ser habilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="de512-176">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="de512-177">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="de512-177">firewallBlockAllIncoming</span></span>|<span data-ttu-id="de512-178">Booliano</span><span class="sxs-lookup"><span data-stu-id="de512-178">Boolean</span></span>|<span data-ttu-id="de512-179">Corresponde à opção "bloquear todas as conexões de entrada".</span><span class="sxs-lookup"><span data-stu-id="de512-179">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="de512-180">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="de512-180">firewallEnableStealthMode</span></span>|<span data-ttu-id="de512-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="de512-181">Boolean</span></span>|<span data-ttu-id="de512-182">Corresponde a "Habilitar modo oculto".</span><span class="sxs-lookup"><span data-stu-id="de512-182">Corresponds to “Enable stealth mode.”</span></span>|
|<span data-ttu-id="de512-183">firewallApplications</span><span class="sxs-lookup"><span data-stu-id="de512-183">firewallApplications</span></span>|<span data-ttu-id="de512-184">coleção [macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md)</span><span class="sxs-lookup"><span data-stu-id="de512-184">[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md) collection</span></span>|<span data-ttu-id="de512-185">Lista de aplicativos com configurações de firewall.</span><span class="sxs-lookup"><span data-stu-id="de512-185">List of applications with firewall settings.</span></span> <span data-ttu-id="de512-186">As configurações de firewall para aplicativos que não estão nessa lista são determinadas pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="de512-186">Firewall settings for applications not on this list are determined by the user.</span></span> <span data-ttu-id="de512-187">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="de512-187">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="de512-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="de512-188">Response</span></span>
<span data-ttu-id="de512-189">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="de512-189">If successful, this method returns a `201 Created` response code and a [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de512-190">Exemplo</span><span class="sxs-lookup"><span data-stu-id="de512-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="de512-191">Solicitação</span><span class="sxs-lookup"><span data-stu-id="de512-191">Request</span></span>
<span data-ttu-id="de512-192">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="de512-192">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 647

{
  "@odata.type": "#microsoft.graph.macOSEndpointProtectionConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "gatekeeperAllowedAppSource": "macAppStore",
  "gatekeeperBlockOverride": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true,
  "firewallApplications": [
    {
      "@odata.type": "microsoft.graph.macOSFirewallApplication",
      "bundleId": "Bundle Id value",
      "allowsIncomingConnections": true
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="de512-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="de512-193">Response</span></span>
<span data-ttu-id="de512-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="de512-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 819

{
  "@odata.type": "#microsoft.graph.macOSEndpointProtectionConfiguration",
  "id": "7bf7f3ca-f3ca-7bf7-caf3-f77bcaf3f77b",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "gatekeeperAllowedAppSource": "macAppStore",
  "gatekeeperBlockOverride": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true,
  "firewallApplications": [
    {
      "@odata.type": "microsoft.graph.macOSFirewallApplication",
      "bundleId": "Bundle Id value",
      "allowsIncomingConnections": true
    }
  ]
}
```




