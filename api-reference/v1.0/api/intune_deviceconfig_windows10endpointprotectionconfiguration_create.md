# <a name="create-windows10endpointprotectionconfiguration"></a><span data-ttu-id="5160b-101">Criar windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="5160b-101">Create windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="5160b-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5160b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5160b-103">Criar um novo objeto [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5160b-103">Create a new [plannerBucket](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5160b-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5160b-104">Prerequisites</span></span>
<span data-ttu-id="5160b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5160b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5160b-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5160b-107">Permission type</span></span>|<span data-ttu-id="5160b-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5160b-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5160b-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5160b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="5160b-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5160b-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5160b-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5160b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5160b-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5160b-112">Not supported.</span></span>|
|<span data-ttu-id="5160b-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5160b-113">Application</span></span>|<span data-ttu-id="5160b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5160b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5160b-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5160b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5160b-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5160b-116">Request headers</span></span>
|<span data-ttu-id="5160b-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5160b-117">Header</span></span>|<span data-ttu-id="5160b-118">Valor</span><span class="sxs-lookup"><span data-stu-id="5160b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5160b-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="5160b-119">Authorization</span></span>|<span data-ttu-id="5160b-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5160b-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5160b-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5160b-121">Accept</span></span>|<span data-ttu-id="5160b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="5160b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5160b-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5160b-123">Request body</span></span>
<span data-ttu-id="5160b-124">No corpo da solicitação, forneça uma representação JSON do objeto windows10EndpointProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="5160b-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="5160b-125">A tabela a seguir mostra as propriedades que são necessárias ao criar windows10EndpointProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="5160b-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="5160b-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5160b-126">Property</span></span>|<span data-ttu-id="5160b-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="5160b-127">Type</span></span>|<span data-ttu-id="5160b-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="5160b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5160b-129">id</span><span class="sxs-lookup"><span data-stu-id="5160b-129">id</span></span>|<span data-ttu-id="5160b-130">String</span><span class="sxs-lookup"><span data-stu-id="5160b-130">String</span></span>|<span data-ttu-id="5160b-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5160b-131">Key of the setting.</span></span> <span data-ttu-id="5160b-132">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5160b-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5160b-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5160b-133">lastModifiedDateTime</span></span>|<span data-ttu-id="5160b-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5160b-134">DateTimeOffset</span></span>|<span data-ttu-id="5160b-135">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="5160b-135">Indicates the date the object was last modified.</span></span> <span data-ttu-id="5160b-136">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5160b-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5160b-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5160b-137">createdDateTime</span></span>|<span data-ttu-id="5160b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5160b-138">DateTimeOffset</span></span>|<span data-ttu-id="5160b-139">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="5160b-139">DateTime the object was created.</span></span> <span data-ttu-id="5160b-140">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5160b-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5160b-141">descrição</span><span class="sxs-lookup"><span data-stu-id="5160b-141">description</span></span>|<span data-ttu-id="5160b-142">String</span><span class="sxs-lookup"><span data-stu-id="5160b-142">String</span></span>|<span data-ttu-id="5160b-143">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5160b-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5160b-144">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5160b-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5160b-145">displayName</span><span class="sxs-lookup"><span data-stu-id="5160b-145">displayName</span></span>|<span data-ttu-id="5160b-146">String</span><span class="sxs-lookup"><span data-stu-id="5160b-146">String</span></span>|<span data-ttu-id="5160b-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5160b-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5160b-148">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5160b-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5160b-149">version</span><span class="sxs-lookup"><span data-stu-id="5160b-149">version</span></span>|<span data-ttu-id="5160b-150">Int32</span><span class="sxs-lookup"><span data-stu-id="5160b-150">Int32</span></span>|<span data-ttu-id="5160b-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5160b-151">Version of the device configuration.</span></span> <span data-ttu-id="5160b-152">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5160b-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5160b-153">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="5160b-153">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="5160b-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="5160b-154">Boolean</span></span>|<span data-ttu-id="5160b-155">Bloqueia conexões de FTP com estado ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="5160b-155">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="5160b-156">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="5160b-156">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="5160b-157">Int32</span><span class="sxs-lookup"><span data-stu-id="5160b-157">Int32</span></span>|<span data-ttu-id="5160b-158">Configura o tempo limite ocioso das associações de segurança, em segundos, de 300 para 3.600, inclusive.</span><span class="sxs-lookup"><span data-stu-id="5160b-158">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="5160b-159">Após esse período, as associações de segurança expirarão e serão excluídas.</span><span class="sxs-lookup"><span data-stu-id="5160b-159">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="5160b-160">Valores válidos de 300 a 3.600</span><span class="sxs-lookup"><span data-stu-id="5160b-160">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="5160b-161">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="5160b-161">firewallPreSharedKeyEncodingMethod</span></span>|<span data-ttu-id="5160b-162">String</span><span class="sxs-lookup"><span data-stu-id="5160b-162">String</span></span>|<span data-ttu-id="5160b-163">Selecione a codificação de chave pré-compartilhada a ser usada Os valores possíveis são: `deviceDefault`, `none`, `utF8`.</span><span class="sxs-lookup"><span data-stu-id="5160b-163">Select the preshared key encoding to be used Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="5160b-164">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="5160b-164">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="5160b-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="5160b-165">Boolean</span></span>|<span data-ttu-id="5160b-166">Configura isenções IPSec para permitir códigos do tipo ICMP IPv6 de descoberta de vizinhos</span><span class="sxs-lookup"><span data-stu-id="5160b-166">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="5160b-167">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="5160b-167">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="5160b-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="5160b-168">Boolean</span></span>|<span data-ttu-id="5160b-169">Configura isenções IPSec para permitir ICMP</span><span class="sxs-lookup"><span data-stu-id="5160b-169">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="5160b-170">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="5160b-170">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="5160b-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="5160b-171">Boolean</span></span>|<span data-ttu-id="5160b-172">Configura isenções IPSec para permitir códigos do tipo ICMP IPv6 de descoberta de roteadores</span><span class="sxs-lookup"><span data-stu-id="5160b-172">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="5160b-173">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="5160b-173">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="5160b-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="5160b-174">Boolean</span></span>|<span data-ttu-id="5160b-175">Configura isenções IPSec para permitir tráfego DHCP de IPv4 e IPv6</span><span class="sxs-lookup"><span data-stu-id="5160b-175">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="5160b-176">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="5160b-176">firewallCertificateRevocationListCheckMethod</span></span>|<span data-ttu-id="5160b-177">String</span><span class="sxs-lookup"><span data-stu-id="5160b-177">String</span></span>|<span data-ttu-id="5160b-178">Especifique como a lista de revogação de certificados é aplicada Os valores possíveis são: `deviceDefault`, `none`, `attempt`, `require`.</span><span class="sxs-lookup"><span data-stu-id="5160b-178">Specify how the certificate revocation list is to be enforced Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="5160b-179">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="5160b-179">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="5160b-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="5160b-180">Boolean</span></span>|<span data-ttu-id="5160b-181">Se um conjunto de autenticação não for totalmente suportado por um módulo de chave, direcione o módulo para ignorar apenas pacotes de autenticação não compatíveis, em vez de todo o conjunto</span><span class="sxs-lookup"><span data-stu-id="5160b-181">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="5160b-182">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="5160b-182">firewallPacketQueueingMethod</span></span>|<span data-ttu-id="5160b-183">String</span><span class="sxs-lookup"><span data-stu-id="5160b-183">String</span></span>|<span data-ttu-id="5160b-184">Configura como o enfileiramento de pacote deve ser aplicado no cenário de gateway de túnel Os valores possíveis são: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span><span class="sxs-lookup"><span data-stu-id="5160b-184">Configures how packet queueing should be applied in the tunnel gateway scenario Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="5160b-185">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="5160b-185">firewallProfileDomain</span></span>|[<span data-ttu-id="5160b-186">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="5160b-186">windowsFirewallNetworkProfile</span></span>](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|<span data-ttu-id="5160b-187">Define as configurações de perfil de firewall das redes do domínio</span><span class="sxs-lookup"><span data-stu-id="5160b-187">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="5160b-188">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="5160b-188">firewallProfilePublic</span></span>|[<span data-ttu-id="5160b-189">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="5160b-189">windowsFirewallNetworkProfile</span></span>](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|<span data-ttu-id="5160b-190">Define as configurações de perfil de firewall das redes públicas</span><span class="sxs-lookup"><span data-stu-id="5160b-190">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="5160b-191">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="5160b-191">firewallProfilePrivate</span></span>|[<span data-ttu-id="5160b-192">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="5160b-192">windowsFirewallNetworkProfile</span></span>](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|<span data-ttu-id="5160b-193">Define as configurações de perfil de firewall das redes privadas</span><span class="sxs-lookup"><span data-stu-id="5160b-193">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="5160b-194">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="5160b-194">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="5160b-195">String collection</span><span class="sxs-lookup"><span data-stu-id="5160b-195">String collection</span></span>|<span data-ttu-id="5160b-196">Lista de arquivos executáveis e pastas a serem excluídos das regras de redução de superfície de ataque</span><span class="sxs-lookup"><span data-stu-id="5160b-196">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="5160b-197">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="5160b-197">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="5160b-198">String collection</span><span class="sxs-lookup"><span data-stu-id="5160b-198">String collection</span></span>|<span data-ttu-id="5160b-199">Lista de caminhos para execução com permissão para acessar as pastas protegidas</span><span class="sxs-lookup"><span data-stu-id="5160b-199">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="5160b-200">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="5160b-200">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="5160b-201">String collection</span><span class="sxs-lookup"><span data-stu-id="5160b-201">String collection</span></span>|<span data-ttu-id="5160b-202">Lista de caminhos de pasta a serem adicionados à lista de pastas protegidas</span><span class="sxs-lookup"><span data-stu-id="5160b-202">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="5160b-203">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="5160b-203">defenderExploitProtectionXml</span></span>|<span data-ttu-id="5160b-204">Binária</span><span class="sxs-lookup"><span data-stu-id="5160b-204">Binary</span></span>|<span data-ttu-id="5160b-205">Conteúdo XML com informações sobre a proteção contra vulnerabilidades.</span><span class="sxs-lookup"><span data-stu-id="5160b-205">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="5160b-206">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="5160b-206">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="5160b-207">String</span><span class="sxs-lookup"><span data-stu-id="5160b-207">String</span></span>|<span data-ttu-id="5160b-208">Nome do arquivo do qual DefenderExploitProtectionXml foi obtido.</span><span class="sxs-lookup"><span data-stu-id="5160b-208">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="5160b-209">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="5160b-209">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="5160b-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="5160b-210">Boolean</span></span>|<span data-ttu-id="5160b-211">Indica se o usuário será ou não impedido de substituir as configurações de Exploit Protection.</span><span class="sxs-lookup"><span data-stu-id="5160b-211">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="5160b-212">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="5160b-212">appLockerApplicationControl</span></span>|<span data-ttu-id="5160b-213">String</span><span class="sxs-lookup"><span data-stu-id="5160b-213">String</span></span>|<span data-ttu-id="5160b-214">Permite que o administrador escolha quais tipos de aplicativo permitir nos dispositivos.</span><span class="sxs-lookup"><span data-stu-id="5160b-214">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="5160b-215">Os valores possíveis são: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span><span class="sxs-lookup"><span data-stu-id="5160b-215">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="5160b-216">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="5160b-216">smartScreenEnableInShell</span></span>|<span data-ttu-id="5160b-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="5160b-217">Boolean</span></span>|<span data-ttu-id="5160b-218">Permite que os administradores de TI configurem SmartScreen para Windows.</span><span class="sxs-lookup"><span data-stu-id="5160b-218">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="5160b-219">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="5160b-219">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="5160b-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="5160b-220">Boolean</span></span>|<span data-ttu-id="5160b-221">Permite que administradores de TI controlem se os usuários podem ignorar avisos do SmartScreen e executar arquivos maliciosos.</span><span class="sxs-lookup"><span data-stu-id="5160b-221">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="5160b-222">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="5160b-222">applicationGuardEnabled</span></span>|<span data-ttu-id="5160b-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="5160b-223">Boolean</span></span>|<span data-ttu-id="5160b-224">Habilitar o Windows Defender Application Guard</span><span class="sxs-lookup"><span data-stu-id="5160b-224">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="5160b-225">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="5160b-225">applicationGuardBlockFileTransfer</span></span>|<span data-ttu-id="5160b-226">String</span><span class="sxs-lookup"><span data-stu-id="5160b-226">String</span></span>|<span data-ttu-id="5160b-227">Impedir a área de transferência de transferir arquivo de imagem, arquivo de texto ou ambos Os valores possíveis são: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span><span class="sxs-lookup"><span data-stu-id="5160b-227">Block clipboard to transfer image file, text file or neither of them Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="5160b-228">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="5160b-228">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="5160b-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="5160b-229">Boolean</span></span>|<span data-ttu-id="5160b-230">Impedir sites corporativos de carregar conteúdos que não sejam da empresa, como plug-ins de terceiros</span><span class="sxs-lookup"><span data-stu-id="5160b-230">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="5160b-231">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="5160b-231">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="5160b-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="5160b-232">Boolean</span></span>|<span data-ttu-id="5160b-233">Permitir dados persistentes gerados por usuários dentro do contêiner do App Guard (favoritos, cookies, senhas da Web, etc.)</span><span class="sxs-lookup"><span data-stu-id="5160b-233">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="5160b-234">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="5160b-234">applicationGuardForceAuditing</span></span>|<span data-ttu-id="5160b-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="5160b-235">Boolean</span></span>|<span data-ttu-id="5160b-236">A auditoria forçada persistirá logs e eventos do Windows para atender aos critérios de segurança/conformidade (exemplos de evento são logon e logoff do usuário, uso de direitos de privilégios, instalação de software, as alterações do sistema, etc.)</span><span class="sxs-lookup"><span data-stu-id="5160b-236">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="5160b-237">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="5160b-237">applicationGuardBlockClipboardSharing</span></span>|<span data-ttu-id="5160b-238">String</span><span class="sxs-lookup"><span data-stu-id="5160b-238">String</span></span>|<span data-ttu-id="5160b-239">Impedir a área de transferência de compartilhar dados do Host para o Contêiner, do Contêiner para o Host ou em ambas as direções.</span><span class="sxs-lookup"><span data-stu-id="5160b-239">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="5160b-240">Os valores possíveis são: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span><span class="sxs-lookup"><span data-stu-id="5160b-240">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="5160b-241">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="5160b-241">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="5160b-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="5160b-242">Boolean</span></span>|<span data-ttu-id="5160b-243">Permitir a impressão em PDF pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="5160b-243">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="5160b-244">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="5160b-244">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="5160b-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="5160b-245">Boolean</span></span>|<span data-ttu-id="5160b-246">Permitir a impressão em XPS pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="5160b-246">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="5160b-247">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="5160b-247">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="5160b-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="5160b-248">Boolean</span></span>|<span data-ttu-id="5160b-249">Permitir a impressão em Impressoras Locais pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="5160b-249">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="5160b-250">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="5160b-250">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="5160b-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="5160b-251">Boolean</span></span>|<span data-ttu-id="5160b-252">Permitir a impressão em Impressoras da Rede pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="5160b-252">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="5160b-253">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="5160b-253">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="5160b-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="5160b-254">Boolean</span></span>|<span data-ttu-id="5160b-255">Permite que o administrador desabilite o aviso de outras criptografias de disco nas máquinas dos usuários.</span><span class="sxs-lookup"><span data-stu-id="5160b-255">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="5160b-256">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="5160b-256">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="5160b-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="5160b-257">Boolean</span></span>|<span data-ttu-id="5160b-258">Permite que o administrador exija que a criptografia seja ativada usando BitLocker.</span><span class="sxs-lookup"><span data-stu-id="5160b-258">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="5160b-259">Essa política é válida apenas para uma SKU móvel.</span><span class="sxs-lookup"><span data-stu-id="5160b-259">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="5160b-260">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="5160b-260">bitLockerEncryptDevice</span></span>|<span data-ttu-id="5160b-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="5160b-261">Boolean</span></span>|<span data-ttu-id="5160b-262">Permite que o administrador exija que a criptografia seja ativada usando BitLocker.</span><span class="sxs-lookup"><span data-stu-id="5160b-262">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="5160b-263">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="5160b-263">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="5160b-264">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="5160b-264">bitLockerRemovableDrivePolicy</span></span>](../resources/intune_deviceconfig_bitlockerremovabledrivepolicy.md)|<span data-ttu-id="5160b-265">Política da unidade removível do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="5160b-265">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="5160b-266">Resposta</span><span class="sxs-lookup"><span data-stu-id="5160b-266">Response</span></span>
<span data-ttu-id="5160b-267">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5160b-267">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5160b-268">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5160b-268">Example</span></span>
### <a name="request"></a><span data-ttu-id="5160b-269">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5160b-269">Request</span></span>
<span data-ttu-id="5160b-270">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5160b-270">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 4309

{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "firewallBlockStatefulFTP": true,
  "firewallIdleTimeoutForSecurityAssociationInSeconds": 2,
  "firewallPreSharedKeyEncodingMethod": "none",
  "firewallIPSecExemptionsAllowNeighborDiscovery": true,
  "firewallIPSecExemptionsAllowICMP": true,
  "firewallIPSecExemptionsAllowRouterDiscovery": true,
  "firewallIPSecExemptionsAllowDHCP": true,
  "firewallCertificateRevocationListCheckMethod": "none",
  "firewallMergeKeyingModuleSettings": true,
  "firewallPacketQueueingMethod": "disabled",
  "firewallProfileDomain": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeBlocked": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "policyRulesFromGroupPolicyMerged": true
  },
  "firewallProfilePublic": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeBlocked": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "policyRulesFromGroupPolicyMerged": true
  },
  "firewallProfilePrivate": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeBlocked": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "policyRulesFromGroupPolicyMerged": true
  },
  "defenderAttackSurfaceReductionExcludedPaths": [
    "Defender Attack Surface Reduction Excluded Paths value"
  ],
  "defenderGuardedFoldersAllowedAppPaths": [
    "Defender Guarded Folders Allowed App Paths value"
  ],
  "defenderAdditionalGuardedFolders": [
    "Defender Additional Guarded Folders value"
  ],
  "defenderExploitProtectionXml": "ZGVmZW5kZXJFeHBsb2l0UHJvdGVjdGlvblhtbA==",
  "defenderExploitProtectionXmlFileName": "Defender Exploit Protection Xml File Name value",
  "defenderSecurityCenterBlockExploitProtectionOverride": true,
  "appLockerApplicationControl": "enforceComponentsAndStoreApps",
  "smartScreenEnableInShell": true,
  "smartScreenBlockOverrideForFiles": true,
  "applicationGuardEnabled": true,
  "applicationGuardBlockFileTransfer": "blockImageAndTextFile",
  "applicationGuardBlockNonEnterpriseContent": true,
  "applicationGuardAllowPersistence": true,
  "applicationGuardForceAuditing": true,
  "applicationGuardBlockClipboardSharing": "blockBoth",
  "applicationGuardAllowPrintToPDF": true,
  "applicationGuardAllowPrintToXPS": true,
  "applicationGuardAllowPrintToLocalPrinters": true,
  "applicationGuardAllowPrintToNetworkPrinters": true,
  "bitLockerDisableWarningForOtherDiskEncryption": true,
  "bitLockerEnableStorageCardEncryptionOnMobile": true,
  "bitLockerEncryptDevice": true,
  "bitLockerRemovableDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "requireEncryptionForWriteAccess": true,
    "blockCrossOrganizationWriteAccess": true
  }
}
```

### <a name="response"></a><span data-ttu-id="5160b-271">Resposta</span><span class="sxs-lookup"><span data-stu-id="5160b-271">Response</span></span>
<span data-ttu-id="5160b-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5160b-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4417

{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
  "id": "09709403-9403-0970-0394-700903947009",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "firewallBlockStatefulFTP": true,
  "firewallIdleTimeoutForSecurityAssociationInSeconds": 2,
  "firewallPreSharedKeyEncodingMethod": "none",
  "firewallIPSecExemptionsAllowNeighborDiscovery": true,
  "firewallIPSecExemptionsAllowICMP": true,
  "firewallIPSecExemptionsAllowRouterDiscovery": true,
  "firewallIPSecExemptionsAllowDHCP": true,
  "firewallCertificateRevocationListCheckMethod": "none",
  "firewallMergeKeyingModuleSettings": true,
  "firewallPacketQueueingMethod": "disabled",
  "firewallProfileDomain": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeBlocked": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "policyRulesFromGroupPolicyMerged": true
  },
  "firewallProfilePublic": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeBlocked": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "policyRulesFromGroupPolicyMerged": true
  },
  "firewallProfilePrivate": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeBlocked": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "policyRulesFromGroupPolicyMerged": true
  },
  "defenderAttackSurfaceReductionExcludedPaths": [
    "Defender Attack Surface Reduction Excluded Paths value"
  ],
  "defenderGuardedFoldersAllowedAppPaths": [
    "Defender Guarded Folders Allowed App Paths value"
  ],
  "defenderAdditionalGuardedFolders": [
    "Defender Additional Guarded Folders value"
  ],
  "defenderExploitProtectionXml": "ZGVmZW5kZXJFeHBsb2l0UHJvdGVjdGlvblhtbA==",
  "defenderExploitProtectionXmlFileName": "Defender Exploit Protection Xml File Name value",
  "defenderSecurityCenterBlockExploitProtectionOverride": true,
  "appLockerApplicationControl": "enforceComponentsAndStoreApps",
  "smartScreenEnableInShell": true,
  "smartScreenBlockOverrideForFiles": true,
  "applicationGuardEnabled": true,
  "applicationGuardBlockFileTransfer": "blockImageAndTextFile",
  "applicationGuardBlockNonEnterpriseContent": true,
  "applicationGuardAllowPersistence": true,
  "applicationGuardForceAuditing": true,
  "applicationGuardBlockClipboardSharing": "blockBoth",
  "applicationGuardAllowPrintToPDF": true,
  "applicationGuardAllowPrintToXPS": true,
  "applicationGuardAllowPrintToLocalPrinters": true,
  "applicationGuardAllowPrintToNetworkPrinters": true,
  "bitLockerDisableWarningForOtherDiskEncryption": true,
  "bitLockerEnableStorageCardEncryptionOnMobile": true,
  "bitLockerEncryptDevice": true,
  "bitLockerRemovableDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "requireEncryptionForWriteAccess": true,
    "blockCrossOrganizationWriteAccess": true
  }
}
```



