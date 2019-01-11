---
title: Criar macOSEndpointProtectionConfiguration
description: Crie um novo objeto de macOSEndpointProtectionConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 160a98e2d05bc362f69741d0459b37aef0c260cf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823034"
---
# <a name="create-macosendpointprotectionconfiguration"></a><span data-ttu-id="f9597-103">Criar macOSEndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="f9597-103">Create macOSEndpointProtectionConfiguration</span></span>

> <span data-ttu-id="f9597-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f9597-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f9597-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f9597-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f9597-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f9597-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f9597-107">Crie um novo objeto de [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f9597-107">Create a new [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f9597-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f9597-108">Prerequisites</span></span>
<span data-ttu-id="f9597-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9597-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9597-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f9597-111">Permission type</span></span>|<span data-ttu-id="f9597-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f9597-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9597-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f9597-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f9597-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9597-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f9597-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f9597-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9597-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9597-116">Not supported.</span></span>|
|<span data-ttu-id="f9597-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f9597-117">Application</span></span>|<span data-ttu-id="f9597-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9597-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9597-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f9597-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f9597-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f9597-120">Request headers</span></span>
|<span data-ttu-id="f9597-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f9597-121">Header</span></span>|<span data-ttu-id="f9597-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f9597-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9597-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f9597-123">Authorization</span></span>|<span data-ttu-id="f9597-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f9597-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9597-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f9597-125">Accept</span></span>|<span data-ttu-id="f9597-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f9597-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9597-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f9597-127">Request body</span></span>
<span data-ttu-id="f9597-128">No corpo da solicitação, fornece uma representação JSON para o objeto macOSEndpointProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f9597-128">In the request body, supply a JSON representation for the macOSEndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="f9597-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o macOSEndpointProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f9597-129">The following table shows the properties that are required when you create the macOSEndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="f9597-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f9597-130">Property</span></span>|<span data-ttu-id="f9597-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9597-131">Type</span></span>|<span data-ttu-id="f9597-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9597-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9597-133">id</span><span class="sxs-lookup"><span data-stu-id="f9597-133">id</span></span>|<span data-ttu-id="f9597-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9597-134">String</span></span>|<span data-ttu-id="f9597-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f9597-135">Key of the entity.</span></span> <span data-ttu-id="f9597-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9597-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9597-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f9597-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f9597-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9597-138">DateTimeOffset</span></span>|<span data-ttu-id="f9597-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="f9597-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f9597-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9597-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9597-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f9597-141">roleScopeTagIds</span></span>|<span data-ttu-id="f9597-142">String collection</span><span class="sxs-lookup"><span data-stu-id="f9597-142">String collection</span></span>|<span data-ttu-id="f9597-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="f9597-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f9597-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9597-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9597-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f9597-145">supportsScopeTags</span></span>|<span data-ttu-id="f9597-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="f9597-146">Boolean</span></span>|<span data-ttu-id="f9597-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="f9597-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f9597-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="f9597-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f9597-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="f9597-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f9597-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9597-150">This property is read-only.</span></span> <span data-ttu-id="f9597-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9597-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9597-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f9597-152">createdDateTime</span></span>|<span data-ttu-id="f9597-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9597-153">DateTimeOffset</span></span>|<span data-ttu-id="f9597-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="f9597-154">DateTime the object was created.</span></span> <span data-ttu-id="f9597-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9597-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9597-156">description</span><span class="sxs-lookup"><span data-stu-id="f9597-156">description</span></span>|<span data-ttu-id="f9597-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9597-157">String</span></span>|<span data-ttu-id="f9597-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9597-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f9597-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9597-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9597-160">displayName</span><span class="sxs-lookup"><span data-stu-id="f9597-160">displayName</span></span>|<span data-ttu-id="f9597-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9597-161">String</span></span>|<span data-ttu-id="f9597-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9597-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f9597-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9597-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9597-164">version</span><span class="sxs-lookup"><span data-stu-id="f9597-164">version</span></span>|<span data-ttu-id="f9597-165">Int32</span><span class="sxs-lookup"><span data-stu-id="f9597-165">Int32</span></span>|<span data-ttu-id="f9597-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9597-166">Version of the device configuration.</span></span> <span data-ttu-id="f9597-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9597-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9597-168">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="f9597-168">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="f9597-169">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="f9597-169">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="f9597-170">Sistema e configuração de privacidade que determina quais aplicativos de locais de download podem ser executados de em um dispositivo macOS.</span><span class="sxs-lookup"><span data-stu-id="f9597-170">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="f9597-171">Os valores possíveis são: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span><span class="sxs-lookup"><span data-stu-id="f9597-171">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="f9597-172">gatekeeperBlockOverride</span><span class="sxs-lookup"><span data-stu-id="f9597-172">gatekeeperBlockOverride</span></span>|<span data-ttu-id="f9597-173">Booliano</span><span class="sxs-lookup"><span data-stu-id="f9597-173">Boolean</span></span>|<span data-ttu-id="f9597-174">Se definido como true, o usuário substitui para Gatekeeper não assinado será desabilitado.</span><span class="sxs-lookup"><span data-stu-id="f9597-174">If set to true, the user override for Gatekeeper will be disabled.</span></span>|
|<span data-ttu-id="f9597-175">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="f9597-175">firewallEnabled</span></span>|<span data-ttu-id="f9597-176">Booliano</span><span class="sxs-lookup"><span data-stu-id="f9597-176">Boolean</span></span>|<span data-ttu-id="f9597-177">Se o firewall deve ser habilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="f9597-177">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="f9597-178">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="f9597-178">firewallBlockAllIncoming</span></span>|<span data-ttu-id="f9597-179">Booliano</span><span class="sxs-lookup"><span data-stu-id="f9597-179">Boolean</span></span>|<span data-ttu-id="f9597-180">Corresponde à opção "Bloquear todas as conexões de entrada".</span><span class="sxs-lookup"><span data-stu-id="f9597-180">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="f9597-181">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="f9597-181">firewallEnableStealthMode</span></span>|<span data-ttu-id="f9597-182">Booliano</span><span class="sxs-lookup"><span data-stu-id="f9597-182">Boolean</span></span>|<span data-ttu-id="f9597-183">Corresponde ao "Habilitar modo oculto".</span><span class="sxs-lookup"><span data-stu-id="f9597-183">Corresponds to “Enable stealth mode.”</span></span>|
|<span data-ttu-id="f9597-184">firewallApplications</span><span class="sxs-lookup"><span data-stu-id="f9597-184">firewallApplications</span></span>|<span data-ttu-id="f9597-185">coleção [macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md)</span><span class="sxs-lookup"><span data-stu-id="f9597-185">[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md) collection</span></span>|<span data-ttu-id="f9597-186">Lista de aplicativos com as configurações de firewall.</span><span class="sxs-lookup"><span data-stu-id="f9597-186">List of applications with firewall settings.</span></span> <span data-ttu-id="f9597-187">Configurações de firewall para aplicativos não incluídos nesta lista são determinadas pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="f9597-187">Firewall settings for applications not on this list are determined by the user.</span></span> <span data-ttu-id="f9597-188">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="f9597-188">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="f9597-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9597-189">Response</span></span>
<span data-ttu-id="f9597-190">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f9597-190">If successful, this method returns a `201 Created` response code and a [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9597-191">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f9597-191">Example</span></span>
### <a name="request"></a><span data-ttu-id="f9597-192">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9597-192">Request</span></span>
<span data-ttu-id="f9597-193">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f9597-193">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f9597-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9597-194">Response</span></span>
<span data-ttu-id="f9597-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f9597-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





