---
title: Criar macOSEndpointProtectionConfiguration
description: Crie um novo objeto de macOSEndpointProtectionConfiguration.
ms.openlocfilehash: 9f34936359cb3bee08a3427669bc1bc0c2fb7ac2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037761"
---
# <a name="create-macosendpointprotectionconfiguration"></a><span data-ttu-id="56276-103">Criar macOSEndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="56276-103">Create macOSEndpointProtectionConfiguration</span></span>

> <span data-ttu-id="56276-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="56276-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="56276-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="56276-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="56276-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="56276-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="56276-107">Crie um novo objeto de [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="56276-107">Create a new [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="56276-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="56276-108">Prerequisites</span></span>
<span data-ttu-id="56276-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56276-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56276-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="56276-111">Permission type</span></span>|<span data-ttu-id="56276-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="56276-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56276-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="56276-113">Delegated (work or school account)</span></span>|<span data-ttu-id="56276-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56276-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="56276-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="56276-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56276-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56276-116">Not supported.</span></span>|
|<span data-ttu-id="56276-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="56276-117">Application</span></span>|<span data-ttu-id="56276-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56276-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="56276-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="56276-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="56276-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="56276-120">Request headers</span></span>
|<span data-ttu-id="56276-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="56276-121">Header</span></span>|<span data-ttu-id="56276-122">Valor</span><span class="sxs-lookup"><span data-stu-id="56276-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56276-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="56276-123">Authorization</span></span>|<span data-ttu-id="56276-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56276-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56276-125">Accept</span><span class="sxs-lookup"><span data-stu-id="56276-125">Accept</span></span>|<span data-ttu-id="56276-126">application/json</span><span class="sxs-lookup"><span data-stu-id="56276-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56276-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="56276-127">Request body</span></span>
<span data-ttu-id="56276-128">No corpo da solicitação, fornece uma representação JSON para o objeto macOSEndpointProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="56276-128">In the request body, supply a JSON representation for the macOSEndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="56276-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o macOSEndpointProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="56276-129">The following table shows the properties that are required when you create the macOSEndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="56276-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="56276-130">Property</span></span>|<span data-ttu-id="56276-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="56276-131">Type</span></span>|<span data-ttu-id="56276-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="56276-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56276-133">id</span><span class="sxs-lookup"><span data-stu-id="56276-133">id</span></span>|<span data-ttu-id="56276-134">String</span><span class="sxs-lookup"><span data-stu-id="56276-134">String</span></span>|<span data-ttu-id="56276-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="56276-135">Key of the entity.</span></span> <span data-ttu-id="56276-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="56276-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56276-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="56276-137">lastModifiedDateTime</span></span>|<span data-ttu-id="56276-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56276-138">DateTimeOffset</span></span>|<span data-ttu-id="56276-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="56276-139">DateTime the object was last modified.</span></span> <span data-ttu-id="56276-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="56276-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56276-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="56276-141">roleScopeTagIds</span></span>|<span data-ttu-id="56276-142">String collection</span><span class="sxs-lookup"><span data-stu-id="56276-142">String collection</span></span>|<span data-ttu-id="56276-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="56276-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="56276-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="56276-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56276-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="56276-145">supportsScopeTags</span></span>|<span data-ttu-id="56276-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="56276-146">Boolean</span></span>|<span data-ttu-id="56276-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="56276-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="56276-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="56276-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="56276-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="56276-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="56276-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="56276-150">This property is read-only.</span></span> <span data-ttu-id="56276-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="56276-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56276-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="56276-152">createdDateTime</span></span>|<span data-ttu-id="56276-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56276-153">DateTimeOffset</span></span>|<span data-ttu-id="56276-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="56276-154">DateTime the object was created.</span></span> <span data-ttu-id="56276-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="56276-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56276-156">description</span><span class="sxs-lookup"><span data-stu-id="56276-156">description</span></span>|<span data-ttu-id="56276-157">String</span><span class="sxs-lookup"><span data-stu-id="56276-157">String</span></span>|<span data-ttu-id="56276-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="56276-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="56276-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="56276-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56276-160">displayName</span><span class="sxs-lookup"><span data-stu-id="56276-160">displayName</span></span>|<span data-ttu-id="56276-161">String</span><span class="sxs-lookup"><span data-stu-id="56276-161">String</span></span>|<span data-ttu-id="56276-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="56276-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="56276-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="56276-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56276-164">version</span><span class="sxs-lookup"><span data-stu-id="56276-164">version</span></span>|<span data-ttu-id="56276-165">Int32</span><span class="sxs-lookup"><span data-stu-id="56276-165">Int32</span></span>|<span data-ttu-id="56276-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="56276-166">Version of the device configuration.</span></span> <span data-ttu-id="56276-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="56276-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56276-168">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="56276-168">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="56276-169">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="56276-169">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="56276-170">Sistema e configuração de privacidade que determina quais aplicativos de locais de download podem ser executados de em um dispositivo macOS.</span><span class="sxs-lookup"><span data-stu-id="56276-170">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="56276-171">Os valores possíveis são: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span><span class="sxs-lookup"><span data-stu-id="56276-171">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="56276-172">gatekeeperBlockOverride</span><span class="sxs-lookup"><span data-stu-id="56276-172">gatekeeperBlockOverride</span></span>|<span data-ttu-id="56276-173">Booliano</span><span class="sxs-lookup"><span data-stu-id="56276-173">Boolean</span></span>|<span data-ttu-id="56276-174">Se definido como true, o usuário substitui para Gatekeeper não assinado será desabilitado.</span><span class="sxs-lookup"><span data-stu-id="56276-174">If set to true, the user override for Gatekeeper will be disabled.</span></span>|
|<span data-ttu-id="56276-175">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="56276-175">firewallEnabled</span></span>|<span data-ttu-id="56276-176">Booliano</span><span class="sxs-lookup"><span data-stu-id="56276-176">Boolean</span></span>|<span data-ttu-id="56276-177">Se o firewall deve ser habilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="56276-177">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="56276-178">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="56276-178">firewallBlockAllIncoming</span></span>|<span data-ttu-id="56276-179">Booliano</span><span class="sxs-lookup"><span data-stu-id="56276-179">Boolean</span></span>|<span data-ttu-id="56276-180">Corresponde à opção "Bloquear todas as conexões de entrada".</span><span class="sxs-lookup"><span data-stu-id="56276-180">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="56276-181">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="56276-181">firewallEnableStealthMode</span></span>|<span data-ttu-id="56276-182">Booliano</span><span class="sxs-lookup"><span data-stu-id="56276-182">Boolean</span></span>|<span data-ttu-id="56276-183">Corresponde ao "Habilitar modo oculto".</span><span class="sxs-lookup"><span data-stu-id="56276-183">Corresponds to “Enable stealth mode.”</span></span>|
|<span data-ttu-id="56276-184">firewallApplications</span><span class="sxs-lookup"><span data-stu-id="56276-184">firewallApplications</span></span>|<span data-ttu-id="56276-185">coleção [macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md)</span><span class="sxs-lookup"><span data-stu-id="56276-185">[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md) collection</span></span>|<span data-ttu-id="56276-186">Lista de aplicativos com as configurações de firewall.</span><span class="sxs-lookup"><span data-stu-id="56276-186">List of applications with firewall settings.</span></span> <span data-ttu-id="56276-187">Configurações de firewall para aplicativos não incluídos nesta lista são determinadas pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="56276-187">Firewall settings for applications not on this list are determined by the user.</span></span> <span data-ttu-id="56276-188">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="56276-188">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="56276-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="56276-189">Response</span></span>
<span data-ttu-id="56276-190">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="56276-190">If successful, this method returns a `201 Created` response code and a [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56276-191">Exemplo</span><span class="sxs-lookup"><span data-stu-id="56276-191">Example</span></span>
### <a name="request"></a><span data-ttu-id="56276-192">Solicitação</span><span class="sxs-lookup"><span data-stu-id="56276-192">Request</span></span>
<span data-ttu-id="56276-193">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="56276-193">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 711

{
  "@odata.type": "#microsoft.graph.macOSEndpointProtectionConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="56276-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="56276-194">Response</span></span>
<span data-ttu-id="56276-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="56276-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





