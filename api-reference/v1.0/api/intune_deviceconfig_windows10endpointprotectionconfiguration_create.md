# <a name="create-windows10endpointprotectionconfiguration"></a><span data-ttu-id="6bd40-101">Criar windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="6bd40-101">Create windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="6bd40-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6bd40-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6bd40-103">Criar um novo objeto [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6bd40-103">Create a new [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6bd40-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6bd40-104">Prerequisites</span></span>
<span data-ttu-id="6bd40-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6bd40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6bd40-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6bd40-107">Permission type</span></span>|<span data-ttu-id="6bd40-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6bd40-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6bd40-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6bd40-109">Delegated (work or school account)</span></span>|<span data-ttu-id="6bd40-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6bd40-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6bd40-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6bd40-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6bd40-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6bd40-112">Not supported.</span></span>|
|<span data-ttu-id="6bd40-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6bd40-113">Application</span></span>|<span data-ttu-id="6bd40-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6bd40-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6bd40-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6bd40-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6bd40-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6bd40-116">Request headers</span></span>
|<span data-ttu-id="6bd40-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6bd40-117">Header</span></span>|<span data-ttu-id="6bd40-118">Valor</span><span class="sxs-lookup"><span data-stu-id="6bd40-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6bd40-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="6bd40-119">Authorization</span></span>|<span data-ttu-id="6bd40-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="6bd40-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6bd40-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6bd40-121">Accept</span></span>|<span data-ttu-id="6bd40-122">application/json</span><span class="sxs-lookup"><span data-stu-id="6bd40-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6bd40-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6bd40-123">Request body</span></span>
<span data-ttu-id="6bd40-124">No corpo da solicitação, forneça uma representação JSON do objeto windows10EndpointProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6bd40-124">In the request body, supply a JSON representation for the windows10EndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="6bd40-125">A tabela a seguir mostra as propriedades que são necessárias ao criar windows10EndpointProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6bd40-125">The following table shows the properties that are required when you create the windows10EndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="6bd40-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6bd40-126">Property</span></span>|<span data-ttu-id="6bd40-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="6bd40-127">Type</span></span>|<span data-ttu-id="6bd40-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="6bd40-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bd40-129">id</span><span class="sxs-lookup"><span data-stu-id="6bd40-129">id</span></span>|<span data-ttu-id="6bd40-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6bd40-130">String</span></span>|<span data-ttu-id="6bd40-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6bd40-131">Key of the entity.</span></span> <span data-ttu-id="6bd40-132">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bd40-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bd40-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6bd40-133">lastModifiedDateTime</span></span>|<span data-ttu-id="6bd40-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6bd40-134">DateTimeOffset</span></span>|<span data-ttu-id="6bd40-135">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="6bd40-135">DateTime the object was last modified.</span></span> <span data-ttu-id="6bd40-136">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bd40-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bd40-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6bd40-137">createdDateTime</span></span>|<span data-ttu-id="6bd40-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6bd40-138">DateTimeOffset</span></span>|<span data-ttu-id="6bd40-139">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="6bd40-139">DateTime the object was created.</span></span> <span data-ttu-id="6bd40-140">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bd40-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bd40-141">description</span><span class="sxs-lookup"><span data-stu-id="6bd40-141">description</span></span>|<span data-ttu-id="6bd40-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6bd40-142">String</span></span>|<span data-ttu-id="6bd40-143">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6bd40-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6bd40-144">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bd40-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bd40-145">displayName</span><span class="sxs-lookup"><span data-stu-id="6bd40-145">displayName</span></span>|<span data-ttu-id="6bd40-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6bd40-146">String</span></span>|<span data-ttu-id="6bd40-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6bd40-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6bd40-148">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bd40-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bd40-149">version</span><span class="sxs-lookup"><span data-stu-id="6bd40-149">version</span></span>|<span data-ttu-id="6bd40-150">Int32</span><span class="sxs-lookup"><span data-stu-id="6bd40-150">Int32</span></span>|<span data-ttu-id="6bd40-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6bd40-151">Version of the device configuration.</span></span> <span data-ttu-id="6bd40-152">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bd40-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bd40-153">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="6bd40-153">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="6bd40-154">Booleano</span><span class="sxs-lookup"><span data-stu-id="6bd40-154">Boolean</span></span>|<span data-ttu-id="6bd40-155">Bloqueia conexões de FTP com estado ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="6bd40-155">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="6bd40-156">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="6bd40-156">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="6bd40-157">Int32</span><span class="sxs-lookup"><span data-stu-id="6bd40-157">Int32</span></span>|<span data-ttu-id="6bd40-158">Configura o tempo limite ocioso das associações de segurança, em segundos, de 300 para 3.600, inclusive.</span><span class="sxs-lookup"><span data-stu-id="6bd40-158">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="6bd40-159">Após esse período, as associações de segurança expirarão e serão excluídas.</span><span class="sxs-lookup"><span data-stu-id="6bd40-159">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="6bd40-160">Valores válidos de 300 a 3.600</span><span class="sxs-lookup"><span data-stu-id="6bd40-160">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="6bd40-161">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="6bd40-161">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="6bd40-162">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="6bd40-162">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune_deviceconfig_firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="6bd40-163">Selecionar a codificação de chave pré-compartilhada a ser usada.</span><span class="sxs-lookup"><span data-stu-id="6bd40-163">Select the preshared key encoding to be used Possible values are: , , .</span></span> <span data-ttu-id="6bd40-164">Os valores possíveis são: `deviceDefault`, `none`, `utF8`.</span><span class="sxs-lookup"><span data-stu-id="6bd40-164">The possible values are:</span></span>|
|<span data-ttu-id="6bd40-165">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="6bd40-165">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="6bd40-166">Booleano</span><span class="sxs-lookup"><span data-stu-id="6bd40-166">Boolean</span></span>|<span data-ttu-id="6bd40-167">Configura isenções IPSec para permitir códigos do tipo ICMP IPv6 de descoberta de vizinhos</span><span class="sxs-lookup"><span data-stu-id="6bd40-167">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="6bd40-168">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="6bd40-168">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="6bd40-169">Booleano</span><span class="sxs-lookup"><span data-stu-id="6bd40-169">Boolean</span></span>|<span data-ttu-id="6bd40-170">Configura isenções IPSec para permitir ICMP</span><span class="sxs-lookup"><span data-stu-id="6bd40-170">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="6bd40-171">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="6bd40-171">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="6bd40-172">Booleano</span><span class="sxs-lookup"><span data-stu-id="6bd40-172">Boolean</span></span>|<span data-ttu-id="6bd40-173">Configura isenções IPSec para permitir códigos do tipo ICMP IPv6 de descoberta de roteadores</span><span class="sxs-lookup"><span data-stu-id="6bd40-173">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="6bd40-174">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="6bd40-174">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="6bd40-175">Booleano</span><span class="sxs-lookup"><span data-stu-id="6bd40-175">Boolean</span></span>|<span data-ttu-id="6bd40-176">Configura isenções IPSec para permitir tráfego DHCP de IPv4 e IPv6</span><span class="sxs-lookup"><span data-stu-id="6bd40-176">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="6bd40-177">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="6bd40-177">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="6bd40-178">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="6bd40-178">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune_deviceconfig_firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="6bd40-179">Especifique como a lista de revogação de certificado deve ser imposta.</span><span class="sxs-lookup"><span data-stu-id="6bd40-179">Specify how the certificate revocation list is to be enforced Possible values are: , , , .</span></span> <span data-ttu-id="6bd40-180">Os valores possíveis são: `deviceDefault`, `none`, `attempt`, `require`.</span><span class="sxs-lookup"><span data-stu-id="6bd40-180">The possible values are `deviceDefault`, `none`, `attempt`, `require`, , , , , , , , or .</span></span>|
|<span data-ttu-id="6bd40-181">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="6bd40-181">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="6bd40-182">Booleano</span><span class="sxs-lookup"><span data-stu-id="6bd40-182">Boolean</span></span>|<span data-ttu-id="6bd40-183">Se um conjunto de autenticação não for totalmente suportado por um módulo de chave, direcione o módulo para ignorar apenas pacotes de autenticação não compatíveis, em vez de todo o conjunto</span><span class="sxs-lookup"><span data-stu-id="6bd40-183">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="6bd40-184">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="6bd40-184">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="6bd40-185">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="6bd40-185">firewallPacketQueueingMethodType</span></span>](../resources/intune_deviceconfig_firewallpacketqueueingmethodtype.md)|<span data-ttu-id="6bd40-186">Configura como o enfileiramento de pacotes deve ser aplicado no cenário gateway de túnel.</span><span class="sxs-lookup"><span data-stu-id="6bd40-186">Configures how packet queueing should be applied in the tunnel gateway scenario Possible values are: , , , , .</span></span> <span data-ttu-id="6bd40-187">Os valores possíveis são: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span><span class="sxs-lookup"><span data-stu-id="6bd40-187">The possible values are `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`, , , , , , , or .</span></span>|
|<span data-ttu-id="6bd40-188">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="6bd40-188">firewallProfileDomain</span></span>|[<span data-ttu-id="6bd40-189">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="6bd40-189">windowsFirewallNetworkProfile</span></span>](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|<span data-ttu-id="6bd40-190">Define as configurações de perfil de firewall das redes do domínio</span><span class="sxs-lookup"><span data-stu-id="6bd40-190">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="6bd40-191">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="6bd40-191">firewallProfilePublic</span></span>|[<span data-ttu-id="6bd40-192">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="6bd40-192">windowsFirewallNetworkProfile</span></span>](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|<span data-ttu-id="6bd40-193">Define as configurações de perfil de firewall das redes públicas</span><span class="sxs-lookup"><span data-stu-id="6bd40-193">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="6bd40-194">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="6bd40-194">firewallProfilePrivate</span></span>|[<span data-ttu-id="6bd40-195">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="6bd40-195">windowsFirewallNetworkProfile</span></span>](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|<span data-ttu-id="6bd40-196">Define as configurações de perfil de firewall das redes privadas</span><span class="sxs-lookup"><span data-stu-id="6bd40-196">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="6bd40-197">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="6bd40-197">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="6bd40-198">Coleção de sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="6bd40-198">String collection</span></span>|<span data-ttu-id="6bd40-199">Lista de arquivos executáveis e pastas a serem excluídos das regras de redução de superfície de ataque</span><span class="sxs-lookup"><span data-stu-id="6bd40-199">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="6bd40-200">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="6bd40-200">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="6bd40-201">Coleção de sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="6bd40-201">String collection</span></span>|<span data-ttu-id="6bd40-202">Lista de caminhos para execução com permissão para acessar as pastas protegidas</span><span class="sxs-lookup"><span data-stu-id="6bd40-202">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="6bd40-203">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="6bd40-203">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="6bd40-204">Coleção de sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="6bd40-204">String collection</span></span>|<span data-ttu-id="6bd40-205">Lista de caminhos de pasta a serem adicionados à lista de pastas protegidas</span><span class="sxs-lookup"><span data-stu-id="6bd40-205">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="6bd40-206">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="6bd40-206">defenderExploitProtectionXml</span></span>|<span data-ttu-id="6bd40-207">Binária</span><span class="sxs-lookup"><span data-stu-id="6bd40-207">Binary</span></span>|<span data-ttu-id="6bd40-208">Conteúdo XML com informações sobre a proteção contra vulnerabilidades.</span><span class="sxs-lookup"><span data-stu-id="6bd40-208">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="6bd40-209">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="6bd40-209">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="6bd40-210">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6bd40-210">String</span></span>|<span data-ttu-id="6bd40-211">Nome do arquivo do qual DefenderExploitProtectionXml foi obtido.</span><span class="sxs-lookup"><span data-stu-id="6bd40-211">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="6bd40-212">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="6bd40-212">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="6bd40-213">Booleano</span><span class="sxs-lookup"><span data-stu-id="6bd40-213">Boolean</span></span>|<span data-ttu-id="6bd40-214">Indica se o usuário será ou não impedido de substituir as configurações de Exploit Protection.</span><span class="sxs-lookup"><span data-stu-id="6bd40-214">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="6bd40-215">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="6bd40-215">appLockerApplicationControl</span></span>|[<span data-ttu-id="6bd40-216">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="6bd40-216">appLockerApplicationControlType</span></span>](../resources/intune_deviceconfig_applockerapplicationcontroltype.md)|<span data-ttu-id="6bd40-217">Habilita o administrador a escolher quais tipos de aplicativo quer permitir nos dispositivos.</span><span class="sxs-lookup"><span data-stu-id="6bd40-217">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="6bd40-218">Os valores possíveis são: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span><span class="sxs-lookup"><span data-stu-id="6bd40-218">The possible values are `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`, , , , , , , or .</span></span>|
|<span data-ttu-id="6bd40-219">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="6bd40-219">smartScreenEnableInShell</span></span>|<span data-ttu-id="6bd40-220">Booleano</span><span class="sxs-lookup"><span data-stu-id="6bd40-220">Boolean</span></span>|<span data-ttu-id="6bd40-221">Permite que os administradores de TI configurem SmartScreen para Windows.</span><span class="sxs-lookup"><span data-stu-id="6bd40-221">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="6bd40-222">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="6bd40-222">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="6bd40-223">Booleano</span><span class="sxs-lookup"><span data-stu-id="6bd40-223">Boolean</span></span>|<span data-ttu-id="6bd40-224">Permite que administradores de TI controlem se os usuários podem ignorar avisos do SmartScreen e executar arquivos maliciosos.</span><span class="sxs-lookup"><span data-stu-id="6bd40-224">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="6bd40-225">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="6bd40-225">applicationGuardEnabled</span></span>|<span data-ttu-id="6bd40-226">Booleano</span><span class="sxs-lookup"><span data-stu-id="6bd40-226">Boolean</span></span>|<span data-ttu-id="6bd40-227">Habilitar o Windows Defender Application Guard</span><span class="sxs-lookup"><span data-stu-id="6bd40-227">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="6bd40-228">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="6bd40-228">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="6bd40-229">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="6bd40-229">applicationGuardBlockFileTransferType</span></span>](../resources/intune_deviceconfig_applicationguardblockfiletransfertype.md)|<span data-ttu-id="6bd40-230">Impedir a área de transferência de transferir um arquivo de imagem, arquivo de texto ou nenhum deles.</span><span class="sxs-lookup"><span data-stu-id="6bd40-230">Block clipboard to transfer image file, text file or neither of them Possible values are: , , , , .</span></span> <span data-ttu-id="6bd40-231">Os valores possíveis são: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span><span class="sxs-lookup"><span data-stu-id="6bd40-231">The possible values are `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`, , , , , , , or .</span></span>|
|<span data-ttu-id="6bd40-232">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="6bd40-232">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="6bd40-233">Booleano</span><span class="sxs-lookup"><span data-stu-id="6bd40-233">Boolean</span></span>|<span data-ttu-id="6bd40-234">Impedir sites corporativos de carregar conteúdos que não sejam da empresa, como plug-ins de terceiros</span><span class="sxs-lookup"><span data-stu-id="6bd40-234">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="6bd40-235">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="6bd40-235">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="6bd40-236">Booleano</span><span class="sxs-lookup"><span data-stu-id="6bd40-236">Boolean</span></span>|<span data-ttu-id="6bd40-237">Permitir dados persistentes gerados por usuários dentro do contêiner do App Guard (favoritos, cookies, senhas da Web, etc.)</span><span class="sxs-lookup"><span data-stu-id="6bd40-237">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="6bd40-238">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="6bd40-238">applicationGuardForceAuditing</span></span>|<span data-ttu-id="6bd40-239">Booleano</span><span class="sxs-lookup"><span data-stu-id="6bd40-239">Boolean</span></span>|<span data-ttu-id="6bd40-240">A auditoria forçada manterá logs e eventos do Windows para atender aos critérios de segurança/conformidade (exemplos de evento são logon e logoff do usuário, uso de direitos de privilégios, instalação de software, as alterações do sistema, etc.)</span><span class="sxs-lookup"><span data-stu-id="6bd40-240">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="6bd40-241">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="6bd40-241">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="6bd40-242">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="6bd40-242">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune_deviceconfig_applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="6bd40-243">Impedir a área de transferência de compartilhar dados do Host para o Contêiner, do Contêiner para o Host ou em ambas as direções.</span><span class="sxs-lookup"><span data-stu-id="6bd40-243">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="6bd40-244">Os valores possíveis são: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span><span class="sxs-lookup"><span data-stu-id="6bd40-244">The possible values are `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`, , , , , , , or .</span></span>|
|<span data-ttu-id="6bd40-245">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="6bd40-245">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="6bd40-246">Booleano</span><span class="sxs-lookup"><span data-stu-id="6bd40-246">Boolean</span></span>|<span data-ttu-id="6bd40-247">Permitir a impressão em PDF pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="6bd40-247">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="6bd40-248">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="6bd40-248">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="6bd40-249">Booleano</span><span class="sxs-lookup"><span data-stu-id="6bd40-249">Boolean</span></span>|<span data-ttu-id="6bd40-250">Permitir a impressão em XPS pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="6bd40-250">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="6bd40-251">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="6bd40-251">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="6bd40-252">Booleano</span><span class="sxs-lookup"><span data-stu-id="6bd40-252">Boolean</span></span>|<span data-ttu-id="6bd40-253">Permitir a impressão em Impressoras Locais pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="6bd40-253">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="6bd40-254">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="6bd40-254">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="6bd40-255">Booleano</span><span class="sxs-lookup"><span data-stu-id="6bd40-255">Boolean</span></span>|<span data-ttu-id="6bd40-256">Permitir a impressão em Impressoras da Rede pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="6bd40-256">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="6bd40-257">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="6bd40-257">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="6bd40-258">Booleano</span><span class="sxs-lookup"><span data-stu-id="6bd40-258">Boolean</span></span>|<span data-ttu-id="6bd40-259">Permite que o administrador desabilite o aviso de outras criptografias de disco nas máquinas dos usuários.</span><span class="sxs-lookup"><span data-stu-id="6bd40-259">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="6bd40-260">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="6bd40-260">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="6bd40-261">Booleano</span><span class="sxs-lookup"><span data-stu-id="6bd40-261">Boolean</span></span>|<span data-ttu-id="6bd40-262">Permite que o administrador exija que a criptografia seja ativada usando BitLocker.</span><span class="sxs-lookup"><span data-stu-id="6bd40-262">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="6bd40-263">Essa política é válida apenas para uma SKU móvel.</span><span class="sxs-lookup"><span data-stu-id="6bd40-263">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="6bd40-264">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="6bd40-264">bitLockerEncryptDevice</span></span>|<span data-ttu-id="6bd40-265">Booleano</span><span class="sxs-lookup"><span data-stu-id="6bd40-265">Boolean</span></span>|<span data-ttu-id="6bd40-266">Permite que o administrador exija que a criptografia seja ativada usando BitLocker.</span><span class="sxs-lookup"><span data-stu-id="6bd40-266">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="6bd40-267">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="6bd40-267">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="6bd40-268">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="6bd40-268">bitLockerRemovableDrivePolicy</span></span>](../resources/intune_deviceconfig_bitlockerremovabledrivepolicy.md)|<span data-ttu-id="6bd40-269">Política da unidade removível do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="6bd40-269">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="6bd40-270">Resposta</span><span class="sxs-lookup"><span data-stu-id="6bd40-270">Response</span></span>
<span data-ttu-id="6bd40-271">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6bd40-271">If successful, this method returns a `201 Created` response code and a [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6bd40-272">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6bd40-272">Example</span></span>
### <a name="request"></a><span data-ttu-id="6bd40-273">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6bd40-273">Request</span></span>
<span data-ttu-id="6bd40-274">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6bd40-274">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6bd40-275">Resposta</span><span class="sxs-lookup"><span data-stu-id="6bd40-275">Response</span></span>
<span data-ttu-id="6bd40-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6bd40-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



