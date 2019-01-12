---
title: Atualizar macOSEndpointProtectionConfiguration
description: Atualize as propriedades de um objeto macOSEndpointProtectionConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6a9f2c5a1523b934258734befb7e5bea5955e4bc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967907"
---
# <a name="update-macosendpointprotectionconfiguration"></a><span data-ttu-id="2482f-103">Atualizar macOSEndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="2482f-103">Update macOSEndpointProtectionConfiguration</span></span>

> <span data-ttu-id="2482f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2482f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2482f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2482f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2482f-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2482f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2482f-107">Atualize as propriedades de um objeto [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="2482f-107">Update the properties of a [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2482f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2482f-108">Prerequisites</span></span>
<span data-ttu-id="2482f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2482f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2482f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2482f-111">Permission type</span></span>|<span data-ttu-id="2482f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2482f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2482f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2482f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2482f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2482f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2482f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2482f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2482f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2482f-116">Not supported.</span></span>|
|<span data-ttu-id="2482f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2482f-117">Application</span></span>|<span data-ttu-id="2482f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2482f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2482f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2482f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2482f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2482f-120">Request headers</span></span>
|<span data-ttu-id="2482f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2482f-121">Header</span></span>|<span data-ttu-id="2482f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2482f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2482f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2482f-123">Authorization</span></span>|<span data-ttu-id="2482f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2482f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2482f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2482f-125">Accept</span></span>|<span data-ttu-id="2482f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2482f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2482f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2482f-127">Request body</span></span>
<span data-ttu-id="2482f-128">No corpo da solicitação, fornece uma representação JSON para o objeto [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="2482f-128">In the request body, supply a JSON representation for the [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="2482f-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2482f-129">The following table shows the properties that are required when you create the [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md).</span></span>

|<span data-ttu-id="2482f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2482f-130">Property</span></span>|<span data-ttu-id="2482f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2482f-131">Type</span></span>|<span data-ttu-id="2482f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2482f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2482f-133">id</span><span class="sxs-lookup"><span data-stu-id="2482f-133">id</span></span>|<span data-ttu-id="2482f-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2482f-134">String</span></span>|<span data-ttu-id="2482f-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2482f-135">Key of the entity.</span></span> <span data-ttu-id="2482f-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2482f-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2482f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2482f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="2482f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2482f-138">DateTimeOffset</span></span>|<span data-ttu-id="2482f-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="2482f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="2482f-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2482f-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2482f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2482f-141">roleScopeTagIds</span></span>|<span data-ttu-id="2482f-142">String collection</span><span class="sxs-lookup"><span data-stu-id="2482f-142">String collection</span></span>|<span data-ttu-id="2482f-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="2482f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2482f-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2482f-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2482f-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2482f-145">supportsScopeTags</span></span>|<span data-ttu-id="2482f-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="2482f-146">Boolean</span></span>|<span data-ttu-id="2482f-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="2482f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2482f-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="2482f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2482f-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="2482f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2482f-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2482f-150">This property is read-only.</span></span> <span data-ttu-id="2482f-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2482f-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2482f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2482f-152">createdDateTime</span></span>|<span data-ttu-id="2482f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2482f-153">DateTimeOffset</span></span>|<span data-ttu-id="2482f-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="2482f-154">DateTime the object was created.</span></span> <span data-ttu-id="2482f-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2482f-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2482f-156">description</span><span class="sxs-lookup"><span data-stu-id="2482f-156">description</span></span>|<span data-ttu-id="2482f-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2482f-157">String</span></span>|<span data-ttu-id="2482f-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2482f-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2482f-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2482f-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2482f-160">displayName</span><span class="sxs-lookup"><span data-stu-id="2482f-160">displayName</span></span>|<span data-ttu-id="2482f-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2482f-161">String</span></span>|<span data-ttu-id="2482f-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2482f-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2482f-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2482f-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2482f-164">version</span><span class="sxs-lookup"><span data-stu-id="2482f-164">version</span></span>|<span data-ttu-id="2482f-165">Int32</span><span class="sxs-lookup"><span data-stu-id="2482f-165">Int32</span></span>|<span data-ttu-id="2482f-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2482f-166">Version of the device configuration.</span></span> <span data-ttu-id="2482f-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2482f-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2482f-168">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="2482f-168">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="2482f-169">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="2482f-169">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="2482f-170">Sistema e configuração de privacidade que determina quais aplicativos de locais de download podem ser executados de em um dispositivo macOS.</span><span class="sxs-lookup"><span data-stu-id="2482f-170">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="2482f-171">Os valores possíveis são: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span><span class="sxs-lookup"><span data-stu-id="2482f-171">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="2482f-172">gatekeeperBlockOverride</span><span class="sxs-lookup"><span data-stu-id="2482f-172">gatekeeperBlockOverride</span></span>|<span data-ttu-id="2482f-173">Booliano</span><span class="sxs-lookup"><span data-stu-id="2482f-173">Boolean</span></span>|<span data-ttu-id="2482f-174">Se definido como true, o usuário substitui para Gatekeeper não assinado será desabilitado.</span><span class="sxs-lookup"><span data-stu-id="2482f-174">If set to true, the user override for Gatekeeper will be disabled.</span></span>|
|<span data-ttu-id="2482f-175">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="2482f-175">firewallEnabled</span></span>|<span data-ttu-id="2482f-176">Booliano</span><span class="sxs-lookup"><span data-stu-id="2482f-176">Boolean</span></span>|<span data-ttu-id="2482f-177">Se o firewall deve ser habilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="2482f-177">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="2482f-178">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="2482f-178">firewallBlockAllIncoming</span></span>|<span data-ttu-id="2482f-179">Booliano</span><span class="sxs-lookup"><span data-stu-id="2482f-179">Boolean</span></span>|<span data-ttu-id="2482f-180">Corresponde à opção "Bloquear todas as conexões de entrada".</span><span class="sxs-lookup"><span data-stu-id="2482f-180">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="2482f-181">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="2482f-181">firewallEnableStealthMode</span></span>|<span data-ttu-id="2482f-182">Booliano</span><span class="sxs-lookup"><span data-stu-id="2482f-182">Boolean</span></span>|<span data-ttu-id="2482f-183">Corresponde ao "Habilitar modo oculto".</span><span class="sxs-lookup"><span data-stu-id="2482f-183">Corresponds to “Enable stealth mode.”</span></span>|
|<span data-ttu-id="2482f-184">firewallApplications</span><span class="sxs-lookup"><span data-stu-id="2482f-184">firewallApplications</span></span>|<span data-ttu-id="2482f-185">coleção [macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md)</span><span class="sxs-lookup"><span data-stu-id="2482f-185">[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md) collection</span></span>|<span data-ttu-id="2482f-186">Lista de aplicativos com as configurações de firewall.</span><span class="sxs-lookup"><span data-stu-id="2482f-186">List of applications with firewall settings.</span></span> <span data-ttu-id="2482f-187">Configurações de firewall para aplicativos não incluídos nesta lista são determinadas pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="2482f-187">Firewall settings for applications not on this list are determined by the user.</span></span> <span data-ttu-id="2482f-188">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="2482f-188">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="2482f-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="2482f-189">Response</span></span>
<span data-ttu-id="2482f-190">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2482f-190">If successful, this method returns a `200 OK` response code and an updated [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2482f-191">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2482f-191">Example</span></span>
### <a name="request"></a><span data-ttu-id="2482f-192">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2482f-192">Request</span></span>
<span data-ttu-id="2482f-193">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2482f-193">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 636

{
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

### <a name="response"></a><span data-ttu-id="2482f-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="2482f-194">Response</span></span>
<span data-ttu-id="2482f-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2482f-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





