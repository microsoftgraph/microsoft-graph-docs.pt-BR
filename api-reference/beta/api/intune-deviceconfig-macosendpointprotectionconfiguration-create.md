---
title: Criar macOSEndpointProtectionConfiguration
description: Criar um novo objeto macOSEndpointProtectionConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2d58b7fe404fa41f2858f1198160b55880323d7a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32518748"
---
# <a name="create-macosendpointprotectionconfiguration"></a><span data-ttu-id="68c80-103">Criar macOSEndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="68c80-103">Create macOSEndpointProtectionConfiguration</span></span>

> <span data-ttu-id="68c80-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="68c80-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="68c80-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="68c80-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68c80-106">Criar um novo objeto [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="68c80-106">Create a new [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="68c80-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="68c80-107">Prerequisites</span></span>
<span data-ttu-id="68c80-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68c80-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68c80-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="68c80-110">Permission type</span></span>|<span data-ttu-id="68c80-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="68c80-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68c80-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="68c80-112">Delegated (work or school account)</span></span>|<span data-ttu-id="68c80-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68c80-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="68c80-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="68c80-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68c80-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="68c80-115">Not supported.</span></span>|
|<span data-ttu-id="68c80-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="68c80-116">Application</span></span>|<span data-ttu-id="68c80-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="68c80-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="68c80-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="68c80-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="68c80-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="68c80-119">Request headers</span></span>
|<span data-ttu-id="68c80-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="68c80-120">Header</span></span>|<span data-ttu-id="68c80-121">Valor</span><span class="sxs-lookup"><span data-stu-id="68c80-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="68c80-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="68c80-122">Authorization</span></span>|<span data-ttu-id="68c80-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="68c80-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="68c80-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="68c80-124">Accept</span></span>|<span data-ttu-id="68c80-125">application/json</span><span class="sxs-lookup"><span data-stu-id="68c80-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="68c80-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="68c80-126">Request body</span></span>
<span data-ttu-id="68c80-127">No corpo da solicitação, forneça uma representação JSON do objeto macOSEndpointProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="68c80-127">In the request body, supply a JSON representation for the macOSEndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="68c80-128">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSEndpointProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="68c80-128">The following table shows the properties that are required when you create the macOSEndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="68c80-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="68c80-129">Property</span></span>|<span data-ttu-id="68c80-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="68c80-130">Type</span></span>|<span data-ttu-id="68c80-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="68c80-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68c80-132">id</span><span class="sxs-lookup"><span data-stu-id="68c80-132">id</span></span>|<span data-ttu-id="68c80-133">String</span><span class="sxs-lookup"><span data-stu-id="68c80-133">String</span></span>|<span data-ttu-id="68c80-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="68c80-134">Key of the entity.</span></span> <span data-ttu-id="68c80-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="68c80-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="68c80-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="68c80-136">lastModifiedDateTime</span></span>|<span data-ttu-id="68c80-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68c80-137">DateTimeOffset</span></span>|<span data-ttu-id="68c80-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="68c80-138">DateTime the object was last modified.</span></span> <span data-ttu-id="68c80-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="68c80-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="68c80-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="68c80-140">roleScopeTagIds</span></span>|<span data-ttu-id="68c80-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="68c80-141">String collection</span></span>|<span data-ttu-id="68c80-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="68c80-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="68c80-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="68c80-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="68c80-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="68c80-144">supportsScopeTags</span></span>|<span data-ttu-id="68c80-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="68c80-145">Boolean</span></span>|<span data-ttu-id="68c80-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="68c80-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="68c80-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="68c80-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="68c80-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="68c80-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="68c80-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="68c80-149">This property is read-only.</span></span> <span data-ttu-id="68c80-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="68c80-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="68c80-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="68c80-151">createdDateTime</span></span>|<span data-ttu-id="68c80-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68c80-152">DateTimeOffset</span></span>|<span data-ttu-id="68c80-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="68c80-153">DateTime the object was created.</span></span> <span data-ttu-id="68c80-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="68c80-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="68c80-155">description</span><span class="sxs-lookup"><span data-stu-id="68c80-155">description</span></span>|<span data-ttu-id="68c80-156">String</span><span class="sxs-lookup"><span data-stu-id="68c80-156">String</span></span>|<span data-ttu-id="68c80-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="68c80-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="68c80-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="68c80-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="68c80-159">displayName</span><span class="sxs-lookup"><span data-stu-id="68c80-159">displayName</span></span>|<span data-ttu-id="68c80-160">String</span><span class="sxs-lookup"><span data-stu-id="68c80-160">String</span></span>|<span data-ttu-id="68c80-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="68c80-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="68c80-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="68c80-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="68c80-163">versão</span><span class="sxs-lookup"><span data-stu-id="68c80-163">version</span></span>|<span data-ttu-id="68c80-164">Int32</span><span class="sxs-lookup"><span data-stu-id="68c80-164">Int32</span></span>|<span data-ttu-id="68c80-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="68c80-165">Version of the device configuration.</span></span> <span data-ttu-id="68c80-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="68c80-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="68c80-167">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="68c80-167">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="68c80-168">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="68c80-168">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="68c80-169">Configuração de sistema e privacidade que determina quais locais de download os aplicativos podem ser executados em um dispositivo macOS.</span><span class="sxs-lookup"><span data-stu-id="68c80-169">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="68c80-170">Os valores possíveis são: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span><span class="sxs-lookup"><span data-stu-id="68c80-170">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="68c80-171">gatekeeperBlockOverride</span><span class="sxs-lookup"><span data-stu-id="68c80-171">gatekeeperBlockOverride</span></span>|<span data-ttu-id="68c80-172">Booliano</span><span class="sxs-lookup"><span data-stu-id="68c80-172">Boolean</span></span>|<span data-ttu-id="68c80-173">Se definido como true, a substituição do usuário para gatekeeper será desabilitada.</span><span class="sxs-lookup"><span data-stu-id="68c80-173">If set to true, the user override for Gatekeeper will be disabled.</span></span>|
|<span data-ttu-id="68c80-174">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="68c80-174">firewallEnabled</span></span>|<span data-ttu-id="68c80-175">Booliano</span><span class="sxs-lookup"><span data-stu-id="68c80-175">Boolean</span></span>|<span data-ttu-id="68c80-176">Se o firewall deve ser habilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="68c80-176">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="68c80-177">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="68c80-177">firewallBlockAllIncoming</span></span>|<span data-ttu-id="68c80-178">Booliano</span><span class="sxs-lookup"><span data-stu-id="68c80-178">Boolean</span></span>|<span data-ttu-id="68c80-179">Corresponde à opção "bloquear todas as conexões de entrada".</span><span class="sxs-lookup"><span data-stu-id="68c80-179">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="68c80-180">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="68c80-180">firewallEnableStealthMode</span></span>|<span data-ttu-id="68c80-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="68c80-181">Boolean</span></span>|<span data-ttu-id="68c80-182">Corresponde a "Habilitar modo oculto".</span><span class="sxs-lookup"><span data-stu-id="68c80-182">Corresponds to “Enable stealth mode.”</span></span>|
|<span data-ttu-id="68c80-183">firewallApplications</span><span class="sxs-lookup"><span data-stu-id="68c80-183">firewallApplications</span></span>|<span data-ttu-id="68c80-184">coleção [macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md)</span><span class="sxs-lookup"><span data-stu-id="68c80-184">[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md) collection</span></span>|<span data-ttu-id="68c80-185">Lista de aplicativos com configurações de firewall.</span><span class="sxs-lookup"><span data-stu-id="68c80-185">List of applications with firewall settings.</span></span> <span data-ttu-id="68c80-186">As configurações de firewall para aplicativos que não estão nessa lista são determinadas pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="68c80-186">Firewall settings for applications not on this list are determined by the user.</span></span> <span data-ttu-id="68c80-187">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="68c80-187">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="68c80-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="68c80-188">Response</span></span>
<span data-ttu-id="68c80-189">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="68c80-189">If successful, this method returns a `201 Created` response code and a [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68c80-190">Exemplo</span><span class="sxs-lookup"><span data-stu-id="68c80-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="68c80-191">Solicitação</span><span class="sxs-lookup"><span data-stu-id="68c80-191">Request</span></span>
<span data-ttu-id="68c80-192">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="68c80-192">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="68c80-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="68c80-193">Response</span></span>
<span data-ttu-id="68c80-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="68c80-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





