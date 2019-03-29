---
title: Criar macOSEndpointProtectionConfiguration
description: Criar um novo objeto macOSEndpointProtectionConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 927288f6828cbf9c13791e750f240dd58b7ab972
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30983880"
---
# <a name="create-macosendpointprotectionconfiguration"></a><span data-ttu-id="4ec0c-103">Criar macOSEndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="4ec0c-103">Create macOSEndpointProtectionConfiguration</span></span>

> <span data-ttu-id="4ec0c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4ec0c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ec0c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4ec0c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ec0c-106">Criar um novo objeto [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="4ec0c-106">Create a new [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4ec0c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4ec0c-107">Prerequisites</span></span>
<span data-ttu-id="4ec0c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ec0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ec0c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4ec0c-110">Permission type</span></span>|<span data-ttu-id="4ec0c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4ec0c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ec0c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4ec0c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4ec0c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ec0c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4ec0c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4ec0c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ec0c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ec0c-115">Not supported.</span></span>|
|<span data-ttu-id="4ec0c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4ec0c-116">Application</span></span>|<span data-ttu-id="4ec0c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ec0c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ec0c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4ec0c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4ec0c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4ec0c-119">Request headers</span></span>
|<span data-ttu-id="4ec0c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4ec0c-120">Header</span></span>|<span data-ttu-id="4ec0c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4ec0c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ec0c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4ec0c-122">Authorization</span></span>|<span data-ttu-id="4ec0c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4ec0c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ec0c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4ec0c-124">Accept</span></span>|<span data-ttu-id="4ec0c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4ec0c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ec0c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4ec0c-126">Request body</span></span>
<span data-ttu-id="4ec0c-127">No corpo da solicitação, forneça uma representação JSON do objeto macOSEndpointProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="4ec0c-127">In the request body, supply a JSON representation for the macOSEndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="4ec0c-128">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSEndpointProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="4ec0c-128">The following table shows the properties that are required when you create the macOSEndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="4ec0c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4ec0c-129">Property</span></span>|<span data-ttu-id="4ec0c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4ec0c-130">Type</span></span>|<span data-ttu-id="4ec0c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ec0c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ec0c-132">id</span><span class="sxs-lookup"><span data-stu-id="4ec0c-132">id</span></span>|<span data-ttu-id="4ec0c-133">String</span><span class="sxs-lookup"><span data-stu-id="4ec0c-133">String</span></span>|<span data-ttu-id="4ec0c-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4ec0c-134">Key of the entity.</span></span> <span data-ttu-id="4ec0c-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ec0c-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ec0c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4ec0c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4ec0c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ec0c-137">DateTimeOffset</span></span>|<span data-ttu-id="4ec0c-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="4ec0c-138">DateTime the object was last modified.</span></span> <span data-ttu-id="4ec0c-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ec0c-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ec0c-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4ec0c-140">roleScopeTagIds</span></span>|<span data-ttu-id="4ec0c-141">Coleção String</span><span class="sxs-lookup"><span data-stu-id="4ec0c-141">String collection</span></span>|<span data-ttu-id="4ec0c-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="4ec0c-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4ec0c-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ec0c-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ec0c-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4ec0c-144">supportsScopeTags</span></span>|<span data-ttu-id="4ec0c-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ec0c-145">Boolean</span></span>|<span data-ttu-id="4ec0c-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="4ec0c-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4ec0c-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="4ec0c-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4ec0c-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="4ec0c-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4ec0c-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4ec0c-149">This property is read-only.</span></span> <span data-ttu-id="4ec0c-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ec0c-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ec0c-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4ec0c-151">createdDateTime</span></span>|<span data-ttu-id="4ec0c-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ec0c-152">DateTimeOffset</span></span>|<span data-ttu-id="4ec0c-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="4ec0c-153">DateTime the object was created.</span></span> <span data-ttu-id="4ec0c-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ec0c-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ec0c-155">descrição</span><span class="sxs-lookup"><span data-stu-id="4ec0c-155">description</span></span>|<span data-ttu-id="4ec0c-156">String</span><span class="sxs-lookup"><span data-stu-id="4ec0c-156">String</span></span>|<span data-ttu-id="4ec0c-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4ec0c-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4ec0c-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ec0c-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ec0c-159">displayName</span><span class="sxs-lookup"><span data-stu-id="4ec0c-159">displayName</span></span>|<span data-ttu-id="4ec0c-160">String</span><span class="sxs-lookup"><span data-stu-id="4ec0c-160">String</span></span>|<span data-ttu-id="4ec0c-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4ec0c-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4ec0c-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ec0c-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ec0c-163">versão</span><span class="sxs-lookup"><span data-stu-id="4ec0c-163">version</span></span>|<span data-ttu-id="4ec0c-164">Int32</span><span class="sxs-lookup"><span data-stu-id="4ec0c-164">Int32</span></span>|<span data-ttu-id="4ec0c-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4ec0c-165">Version of the device configuration.</span></span> <span data-ttu-id="4ec0c-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ec0c-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ec0c-167">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="4ec0c-167">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="4ec0c-168">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="4ec0c-168">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="4ec0c-169">Configuração de sistema e privacidade que determina quais locais de download os aplicativos podem ser executados em um dispositivo macOS.</span><span class="sxs-lookup"><span data-stu-id="4ec0c-169">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="4ec0c-170">Os valores possíveis são: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span><span class="sxs-lookup"><span data-stu-id="4ec0c-170">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="4ec0c-171">gatekeeperBlockOverride</span><span class="sxs-lookup"><span data-stu-id="4ec0c-171">gatekeeperBlockOverride</span></span>|<span data-ttu-id="4ec0c-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ec0c-172">Boolean</span></span>|<span data-ttu-id="4ec0c-173">Se definido como true, a substituição do usuário para gatekeeper será desabilitada.</span><span class="sxs-lookup"><span data-stu-id="4ec0c-173">If set to true, the user override for Gatekeeper will be disabled.</span></span>|
|<span data-ttu-id="4ec0c-174">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="4ec0c-174">firewallEnabled</span></span>|<span data-ttu-id="4ec0c-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ec0c-175">Boolean</span></span>|<span data-ttu-id="4ec0c-176">Se o firewall deve ser habilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="4ec0c-176">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="4ec0c-177">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="4ec0c-177">firewallBlockAllIncoming</span></span>|<span data-ttu-id="4ec0c-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ec0c-178">Boolean</span></span>|<span data-ttu-id="4ec0c-179">Corresponde à opção "bloquear todas as conexões de entrada".</span><span class="sxs-lookup"><span data-stu-id="4ec0c-179">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="4ec0c-180">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="4ec0c-180">firewallEnableStealthMode</span></span>|<span data-ttu-id="4ec0c-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ec0c-181">Boolean</span></span>|<span data-ttu-id="4ec0c-182">Corresponde a "Habilitar modo oculto".</span><span class="sxs-lookup"><span data-stu-id="4ec0c-182">Corresponds to “Enable stealth mode.”</span></span>|
|<span data-ttu-id="4ec0c-183">firewallApplications</span><span class="sxs-lookup"><span data-stu-id="4ec0c-183">firewallApplications</span></span>|<span data-ttu-id="4ec0c-184">coleção [macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md)</span><span class="sxs-lookup"><span data-stu-id="4ec0c-184">[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md) collection</span></span>|<span data-ttu-id="4ec0c-185">Lista de aplicativos com configurações de firewall.</span><span class="sxs-lookup"><span data-stu-id="4ec0c-185">List of applications with firewall settings.</span></span> <span data-ttu-id="4ec0c-186">As configurações de firewall para aplicativos que não estão nessa lista são determinadas pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="4ec0c-186">Firewall settings for applications not on this list are determined by the user.</span></span> <span data-ttu-id="4ec0c-187">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="4ec0c-187">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="4ec0c-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ec0c-188">Response</span></span>
<span data-ttu-id="4ec0c-189">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4ec0c-189">If successful, this method returns a `201 Created` response code and a [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ec0c-190">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4ec0c-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="4ec0c-191">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4ec0c-191">Request</span></span>
<span data-ttu-id="4ec0c-192">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4ec0c-192">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4ec0c-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ec0c-193">Response</span></span>
<span data-ttu-id="4ec0c-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4ec0c-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




