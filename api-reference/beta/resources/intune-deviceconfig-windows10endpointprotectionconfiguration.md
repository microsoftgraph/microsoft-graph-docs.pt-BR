---
title: Tipo de recurso windows10EndpointProtectionConfiguration
description: Este tópico fornece descrições dos métodos declarados, das propriedades e das relações expostos pelo recurso Windows10EndpointProtectionConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 51d7efa1cd041c3aa4aa995da2ecfec045d8995a
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66670404"
---
# <a name="windows10endpointprotectionconfiguration-resource-type"></a>Tipo de recurso windows10EndpointProtectionConfiguration

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Este tópico fornece descrições dos métodos declarados, das propriedades e das relações expostos pelo recurso Windows10EndpointProtectionConfiguration.


Herda de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windows10EndpointProtectionConfigurations](../api/intune-deviceconfig-windows10endpointprotectionconfiguration-list.md)|Coleção [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md)|Listar propriedades e relações dos objetos [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).|
|[Obter windows10EndpointProtectionConfiguration](../api/intune-deviceconfig-windows10endpointprotectionconfiguration-get.md)|[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md)|Ler propriedades e relações do objeto [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).|
|[Criar windows10EndpointProtectionConfiguration](../api/intune-deviceconfig-windows10endpointprotectionconfiguration-create.md)|[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md)|Criar um novo objeto [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).|
|[Excluir windows10EndpointProtectionConfiguration](../api/intune-deviceconfig-windows10endpointprotectionconfiguration-delete.md)|Nenhum|Excluir um [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).|
|[Atualizar windows10EndpointProtectionConfiguration](../api/intune-deviceconfig-windows10endpointprotectionconfiguration-update.md)|[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md)|Atualizar as propriedades de um objeto [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de marcas de escopo para esta instância de entidade. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|supportsScopeTags|Booleano|Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo. A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure. Essa propriedade é somente leitura. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|A aplicabilidade da edição do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|A regra de aplicabilidade da versão do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|A regra de aplicabilidade do modo de dispositivo para esta Política. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|descrição|Cadeia de caracteres|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|Cadeia de caracteres|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|versão|Int32|Versão da configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|dmaGuardDeviceEnumerationPolicy|[dmaGuardDeviceEnumerationPolicyType](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|Essa política destina-se a fornecer segurança adicional em dispositivos externos compatíveis com AMD. Ele permite mais controle sobre a enumeração de dispositivos externos compatíveis com AMD incompatíveis com remapeamento de DMA/isolamento de memória do dispositivo e área restrita. Essa política só entra em vigor quando a Proteção contra DMA do Kernel é compatível e habilitada pelo firmware do sistema. A Proteção contra DMA do Kernel é um recurso de plataforma que não pode ser controlado por meio de política ou pelo usuário final. Ele deve ter suporte do sistema no momento da fabricação. Para verificar se o sistema dá suporte à Proteção contra DMA do Kernel, verifique o campo Proteção contra DMA do Kernel na página Resumo do MSINFO32.exe. Os valores possíveis são: `deviceDefault`, `blockAll`, `allowAll`.|
|firewallRules|[Coleção windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md)|Define as configurações de regra de firewall. Essa coleção pode conter um máximo de 150 elementos.|
|userRightsAccessCredentialManagerAsTrustedCaller|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Esse direito de usuário é usado pelo Gerenciador de Credenciais durante o backup/restauração. As credenciais salvas dos usuários poderão ser comprometidas se esse privilégio for fornecido a outras entidades. Há suporte apenas para os estados NotConfigured e Allowed|
|userRightsAllowAccessFromNetwork|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Esse direito de usuário determina quais usuários e grupos têm permissão para se conectar ao computador pela rede. Há suporte para o Estado Permitido.|
|userRightsBlockAccessFromNetwork|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Esse direito de usuário determina quais usuários e grupos estão bloqueados para se conectar ao computador pela rede. Há suporte para o Bloco de Estado.|
|userRightsActAsPartOfTheOperatingSystem|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Esse direito de usuário permite que um processo represente qualquer usuário sem autenticação. Portanto, o processo pode obter acesso aos mesmos recursos locais que esse usuário. Há suporte apenas para os estados NotConfigured e Allowed|
|userRightsLocalLogOn|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Esse direito de usuário determina quais usuários podem fazer logon no computador. Há suporte para Estados Não Configurados, Permitidos |
|userRightsDenyLocalLogOn|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Esse direito de usuário determina quais usuários não podem fazer logon no computador. Há suporte para Estados Não Configurados, Bloqueados |
|userRightsBackupData|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Esse direito de usuário determina quais usuários podem ignorar permissões de arquivo, diretório, registro e outros objetos persistentes ao fazer backup de arquivos e diretórios. Há suporte apenas para os estados NotConfigured e Allowed|
|userRightsChangeSystemTime|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Esse direito de usuário determina quais usuários e grupos podem alterar a hora e a data no relógio interno do computador. Há suporte apenas para os estados NotConfigured e Allowed|
|userRightsCreateGlobalObjects|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Essa configuração de segurança determina se os usuários podem criar objetos globais que estão disponíveis para todas as sessões. Os usuários que podem criar objetos globais podem afetar processos executados em sessões de outros usuários, o que pode levar à falha do aplicativo ou à corrupção de dados. Há suporte apenas para os estados NotConfigured e Allowed|
|userRightsCreatePageFile|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Esse direito de usuário determina quais usuários e grupos podem chamar uma API interna para criar e alterar o tamanho de um arquivo de página. Há suporte apenas para os estados NotConfigured e Allowed|
|userRightsCreatePermanentSharedObjects|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Esse direito de usuário determina quais contas podem ser usadas por processos para criar um objeto de diretório usando o gerenciador de objetos. Há suporte apenas para os estados NotConfigured e Allowed|
|userRightsCreateSymbolicLinks|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Esse direito de usuário determina se o usuário pode criar um link simbólico do computador no qual ele está conectado. Há suporte apenas para os estados NotConfigured e Allowed|
|userRightsCreateToken|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Esse direito de usuário determina quais usuários/grupos podem ser usados por processos para criar um token que pode ser usado para obter acesso a todos os recursos locais quando o processo usa uma API interna para criar um token de acesso. Há suporte apenas para os estados NotConfigured e Allowed|
|userRightsDebugPrograms|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Esse direito de usuário determina quais usuários podem anexar um depurador a qualquer processo ou ao kernel. Há suporte apenas para os estados NotConfigured e Allowed|
|userRightsRemoteDesktopServicesLogOn|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Esse direito de usuário determina quais usuários e grupos são proibidos de fazer logon como um cliente dos Serviços de Área de Trabalho Remota. Há suporte apenas para os estados NotConfigured e Blocked|
|userRightsDelegation|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Esse direito de usuário determina quais usuários podem definir a configuração Confiável para Delegação em um objeto de usuário ou computador. Há suporte apenas para os estados NotConfigured e Allowed.|
|userRightsGenerateSecurityAudits|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Esse direito de usuário determina quais contas podem ser usadas por um processo para adicionar entradas ao log de segurança. O log de segurança é usado para rastrear o acesso não autorizado ao sistema.  Há suporte apenas para os estados NotConfigured e Allowed.|
|userRightsImpersonateClient|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Atribuir esse direito de usuário a um usuário permite que programas em execução em nome desse usuário representem um cliente. Exigir esse direito de usuário para esse tipo de representação impede que um usuário não autorizado convencê-lo a se conectar a um serviço que ele criou e, em seguida, representar esse cliente, o que pode elevar as permissões do usuário não autorizado para níveis administrativos ou do sistema. Há suporte apenas para os estados NotConfigured e Allowed.|
|userRightsIncreaseSchedulingPriority|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Esse direito de usuário determina quais contas podem usar um processo com acesso de Propriedade de Gravação a outro processo para aumentar a prioridade de execução atribuída ao outro processo. Há suporte apenas para os estados NotConfigured e Allowed.|
|userRightsLoadUnloadDrivers|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Esse direito de usuário determina quais usuários podem carregar e descarregar dinamicamente drivers de dispositivo ou outro código no modo kernel. Há suporte apenas para os estados NotConfigured e Allowed.|
|userRightsLockMemory|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Esse direito de usuário determina quais contas podem usar um processo para manter os dados na memória física, o que impede que o sistema pagine os dados para a memória virtual no disco. Há suporte apenas para os estados NotConfigured e Allowed.|
|userRightsManageAuditingAndSecurityLogs|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Esse direito de usuário determina quais usuários podem especificar opções de auditoria de acesso a objeto para recursos individuais, como arquivos, objetos do Active Directory e chaves do Registro. Há suporte apenas para os estados NotConfigured e Allowed.|
|userRightsManageVolumes|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Esse direito de usuário determina quais usuários e grupos podem executar tarefas de manutenção em um volume, como desfragmentação remota. Há suporte apenas para os estados NotConfigured e Allowed.|
|userRightsModifyFirmwareEnvironment|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Esse direito de usuário determina quem pode modificar valores de ambiente de firmware. Há suporte apenas para os estados NotConfigured e Allowed.|
|userRightsModifyObjectLabels|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Esse direito de usuário determina quais contas de usuário podem modificar o rótulo de integridade de objetos, como arquivos, chaves do Registro ou processos pertencentes a outros usuários. Há suporte apenas para os estados NotConfigured e Allowed.|
|userRightsProfileSingleProcess|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Esse direito de usuário determina quais usuários podem usar ferramentas de monitoramento de desempenho para monitorar o desempenho dos processos do sistema. Há suporte apenas para os estados NotConfigured e Allowed.|
|userRightsRemoteShutdown|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Esse direito de usuário determina quais usuários têm permissão para desligar um computador de um local remoto na rede. O uso indevido desse direito de usuário pode resultar em uma negação de serviço. Há suporte apenas para os estados NotConfigured e Allowed.|
|userRightsRestoreData|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Esse direito de usuário determina quais usuários podem ignorar permissões de arquivo, diretório, registro e outros objetos persistentes ao restaurar arquivos e diretórios de backup e determina quais usuários podem definir qualquer entidade de segurança válida como o proprietário de um objeto. Há suporte apenas para os estados NotConfigured e Allowed.|
|userRightsTakeOwnership|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Esse direito de usuário determina quais usuários podem assumir a propriedade de qualquer objeto protegível no sistema, incluindo objetos, arquivos e pastas do Active Directory, impressoras, chaves do Registro, processos e threads. Há suporte apenas para os estados NotConfigured e Allowed.|
|xboxServicesEnableXboxGameSaveTask|Booleano|Essa configuração determina se o xbox Game Save está habilitado (1) ou desabilitado (0).|
|xboxServicesAccessoryManagementServiceStartupMode|[serviceStartType](../resources/intune-deviceconfig-servicestarttype.md)|Essa configuração determina se o tipo de início do serviço de gerenciamento de acessórios é Automático(2), Manual(3), Desabilitado(4). Padrão: manual. Os valores possíveis são: `manual`, `automatic`, `disabled`.|
|xboxServicesLiveAuthManagerServiceStartupMode|[serviceStartType](../resources/intune-deviceconfig-servicestarttype.md)|Essa configuração determina se o tipo de início do serviço Live Auth Manager é Automático(2), Manual(3), Desabilitado(4). Padrão: manual. Os valores possíveis são: `manual`, `automatic`, `disabled`.|
|xboxServicesLiveGameSaveServiceStartupMode|[serviceStartType](../resources/intune-deviceconfig-servicestarttype.md)|Essa configuração determina se o tipo de início do serviço Live Game Save é Automático(2), Manual(3), Desabilitado(4). Padrão: manual. Os valores possíveis são: `manual`, `automatic`, `disabled`.|
|xboxServicesLiveNetworkingServiceStartupMode|[serviceStartType](../resources/intune-deviceconfig-servicestarttype.md)|Essa configuração determina se o tipo de início do serviço de rede é Automático(2), Manual(3), Desabilitado(4). Padrão: manual. Os valores possíveis são: `manual`, `automatic`, `disabled`.|
|localSecurityOptionsBlockMicrosoftAccounts|Booleano|Impedir que os usuários adicionem novas contas da Microsoft a este computador.|
|localSecurityOptionsBlockRemoteLogonWithBlankPassword|Booleano|Habilite contas locais que não estão protegidas por senha para fazer logon de locais diferentes do dispositivo físico. O padrão está habilitado|
|localSecurityOptionsDisableAdministratorAccount|Booleano|Determina se a conta de Administrador Local está habilitada ou desabilitada.|
|localSecurityOptionsAdministratorAccountName|Cadeia de Caracteres|Defina um nome de conta diferente a ser associado ao SID (identificador de segurança) da conta "Administrador".|
|localSecurityOptionsDisableGuestAccount|Booleano|Determina se a conta convidado está habilitada ou desabilitada.|
|localSecurityOptionsGuestAccountName|Cadeia de Caracteres|Defina um nome de conta diferente a ser associado ao SID (identificador de segurança) da conta "Convidado".|
|localSecurityOptionsAllowUndockWithoutHavingToLogon|Booleano|Impedir que um computador portátil seja desencaixado sem precisar fazer logon.|
|localSecurityOptionsBlockUsersInstallingPrinterDrivers|Booleano|Restrinja a instalação de drivers de impressora como parte da conexão com uma impressora compartilhada somente para administradores.|
|localSecurityOptionsBlockRemoteOpticalDriveAccess|Booleano|Habilitar essas configurações permite que apenas o usuário conectado interativamente acesse a mídia de CD-ROM.|
|localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser|[localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|Defina quem tem permissão para formatar e ejetar mídia NTFS removível. Os valores possíveis são: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.|
|localSecurityOptionsMachineInactivityLimit|Int32|Defina o máximo de minutos de inatividade na tela de logon da área de trabalho interativa até que a economia de tela seja executada. Valores válidos de 0 a 9999|
|localSecurityOptionsMachineInactivityLimitInMinutes|Int32|Defina o máximo de minutos de inatividade na tela de logon da área de trabalho interativa até que a economia de tela seja executada. Valores válidos de 0 a 9999|
|localSecurityOptionsDoNotRequireCtrlAltDel|Booleano|Exigir que CTRL+ALT+DEL seja pressionado antes que um usuário possa fazer logon.|
|localSecurityOptionsHideLastSignedInUser|Booleano|Não exiba o nome de usuário da última pessoa que entrou neste dispositivo.|
|localSecurityOptionsHideUsernameAtSignIn|Booleano|Não exiba o nome de usuário da pessoa que está entrando nesse dispositivo depois que as credenciais forem inseridas e antes que a área de trabalho do dispositivo seja mostrada.|
|localSecurityOptionsLogOnMessageTitle|Cadeia de Caracteres|Defina o título da mensagem para os usuários que tentarem fazer logon.|
|localSecurityOptionsLogOnMessageText|Cadeia de caracteres|Defina o texto da mensagem para os usuários que tentarem fazer logon.|
|localSecurityOptionsAllowPKU2UAuthenticationRequests|Boolean|Bloqueie solicitações de autenticação PKU2U para esse dispositivo para usar identidades online.|
|localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool|Booleano|Boolean auxiliar de interface do usuário para a entidade LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager|
|localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager|Cadeia de Caracteres|Edite a cadeia de caracteres padrão da Linguagem de Definição do Descritor de Segurança para permitir ou negar que usuários e grupos façam chamadas remotas para o SAM.|
|localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients|[localSecurityOptionsMinimumSessionSecurity](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|Essa configuração de segurança permite que um cliente exija a negociação de criptografia de 128 bits e/ou segurança de sessão NTLMv2. Os valores possíveis são: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.|
|localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers|[localSecurityOptionsMinimumSessionSecurity](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|Essa configuração de segurança permite que um servidor exija a negociação de criptografia de 128 bits e/ou segurança de sessão NTLMv2. Os valores possíveis são: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.|
|lanManagerAuthenticationLevel|[lanManagerAuthenticationLevel](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|Essa configuração de segurança determina qual protocolo de autenticação de desafio/resposta é usado para logons de rede. Os possíveis valores são: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.|
|lanManagerWorkstationDisableInsecureGuestLogons|Booleano|Se habilitado, o cliente SMB permitirá logons de convidados inseguros. Se não estiver configurado, o cliente SMB rejeitará logons de convidados inseguros.|
|localSecurityOptionsClearVirtualMemoryPageFile|Booliano|Essa configuração de segurança determina se o arquivo de paginação de memória virtual é limpo quando o sistema é desligado.|
|localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn|Booleano|Essa configuração de segurança determina se um computador pode ser desligado sem precisar fazer logon no Windows.|
|localSecurityOptionsAllowUIAccessApplicationElevation|Booleano|Permitir que aplicativos UIAccess solicitem elevação sem usar a área de trabalho segura.|
|localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations|Booleano|Virtualizar falhas de gravação de arquivo e registro em locais de usuário|
|localSecurityOptionsOnlyElevateSignedExecutables|Booleano|Imponha a validação do caminho de certificação PKI para um determinado arquivo executável antes que ele seja permitido para execução.|
|localSecurityOptionsAdministratorElevationPromptBehavior|[localSecurityOptionsAdministratorElevationPromptBehaviorType](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|Defina o comportamento do prompt de elevação para administradores Administração Modo de Aprovação. Os valores possíveis são: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.|
|localSecurityOptionsStandardUserElevationPromptBehavior|[localSecurityOptionsStandardUserElevationPromptBehaviorType](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|Defina o comportamento do prompt de elevação para usuários padrão. Os valores possíveis são: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.|
|localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation|Booleano|Permitir que todas as solicitações de elevação acessem a área de trabalho do usuário interativo em vez da área de trabalho segura. As configurações de política de comportamento de prompt para administradores e usuários padrão são usadas.|
|localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation|Booleano|Instalações de aplicativo que exigem privilégios elevados solicitarão credenciais de administrador. O padrão está habilitado|
|localSecurityOptionsAllowUIAccessApplicationsForSecureLocations|Booleano|Permitir que aplicativos UIAccess solicitem elevação sem usar a área de trabalho segura. O padrão está habilitado|
|localSecurityOptionsUseAdminApprovalMode|Booleano|Define se a conta de administrador interna usa o Administração de Aprovação ou executa todos os aplicativos com privilégios de administrador completos. O padrão está habilitado|
|localSecurityOptionsUseAdminApprovalModeForAdministrators|Booleano|Defina se Administração modo de aprovação e se todas as configurações de política do UAC estão habilitadas, o padrão está habilitado|
|localSecurityOptionsInformationShownOnLockScreen|[localSecurityOptionsInformationShownOnLockScreenType](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|Configure as informações do usuário exibidas quando a sessão está bloqueada. Se não estiver configurado, o nome de exibição do usuário, o domínio e o nome de usuário serão mostrados. Os valores possíveis são: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.|
|localSecurityOptionsInformationDisplayedOnLockScreen|[localSecurityOptionsInformationDisplayedOnLockScreenType](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|Configure as informações do usuário exibidas quando a sessão está bloqueada. Se não estiver configurado, o nome de exibição do usuário, o domínio e o nome de usuário serão mostrados. Os valores possíveis são: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.|
|localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees|Booleano|Essa configuração de segurança determina se o cliente SMB tenta negociar a assinatura de pacote SMB.|
|localSecurityOptionsClientDigitallySignCommunicationsAlways|Booleano|Essa configuração de segurança determina se a assinatura de pacote é exigida pelo componente de cliente SMB.|
|localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers|Booleano|Se essa configuração de segurança estiver habilitada, o redirecionador SMB (Server Message Block) poderá enviar senhas de texto não criptografado para servidores SMB não Microsoft que não dão suporte à criptografia de senha durante a autenticação.|
|localSecurityOptionsDisableServerDigitallySignCommunicationsAlways|Booleano|Essa configuração de segurança determina se a assinatura de pacote é exigida pelo componente de servidor SMB.|
|localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees|Booleano|Essa configuração de segurança determina se o servidor SMB negociará a assinatura de pacote SMB com clientes que o solicitarem.|
|localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares|Booleano|Por padrão, essa configuração de segurança restringe o acesso anônimo a compartilhamentos e pipes às configurações de pipes nomeados que podem ser acessados anonimamente e Compartilhamentos que podem ser acessados anonimamente|
|localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts|Booleano|Essa configuração de segurança determina quais permissões adicionais serão concedidas para conexões anônimas com o computador.|
|localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares|Booleano|Essa configuração de segurança determina se os usuários anônimos devem executar determinadas atividades, como enumerar os nomes de contas de domínio e compartilhamentos de rede.|
|localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange|Booliano|Essa configuração de segurança determina se, na próxima alteração de senha, o valor de hash do LAN Manager (LM) para a nova senha será armazenado. Ele não é armazenado por padrão.|
|localSecurityOptionsSmartCardRemovalBehavior|[localSecurityOptionsSmartCardRemovalBehaviorType](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)|Essa configuração de segurança determina o que acontece quando o cartão inteligente de um usuário conectado é removido do leitor de cartão inteligente. Os valores possíveis são: `noAction`, `lockWorkstation`, `forceLogoff`, `disconnectRemoteDesktopSession`.|
|defenderSecurityCenterDisableAppBrowserUI|Booleano|Usado para desabilitar a exibição da área de proteção do aplicativo e do navegador.|
|defenderSecurityCenterDisableFamilyUI|Booleano|Usado para desabilitar a exibição da área de opções da família.|
|defenderSecurityCenterDisableHealthUI|Booleano|Usado para desabilitar a exibição da área de integridade e desempenho do dispositivo.|
|defenderSecurityCenterDisableNetworkUI|Booleano|Usado para desabilitar a exibição do firewall e da área de proteção de rede.|
|defenderSecurityCenterDisable VirusUI|Booleano|Usado para desabilitar a exibição da área de proteção contra vírus e ameaças.|
|defenderSecurityCenterDisableAccountUI|Booleano|Usado para desabilitar a exibição da área de proteção da conta.|
|defenderSecurityCenterDisableClearTpmUI|Booleano|Usado para desabilitar a exibição do botão Limpar TPM.|
|defenderSecurityCenterDisableHardwareUI|Booleano|Usado para desabilitar a exibição da área de proteção de hardware.|
|defenderSecurityCenterDisableNotificationAreaUI|Booleano|Usado para desabilitar a exibição do controle de área de notificação. O usuário precisa sair e entrar ou reinicializar o computador para que essa configuração entre em vigor.|
|defenderSecurityCenterDisableRansomwareUI|Booleano|Usado para desabilitar a exibição da área de proteção contra ransomware. |
|defenderSecurityCenterDisableSecureBootUI|Booliano|Usado para desabilitar a exibição da área de inicialização segura em Segurança do dispositivo.|
|defenderSecurityCenterDisableTroubleshootingUI|Booleano|Usado para desabilitar a exibição da solução de problemas do processo de segurança em Segurança do dispositivo.|
|defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI|Booleano|Usado para desabilitar a exibição da atualização do firmware do TPM quando um firmware vulnerável é detectado.|
|defenderSecurityCenterOrganizationDisplayName|Cadeia de Caracteres|O nome da empresa que é exibido aos usuários.|
|defenderSecurityCenterHelpEmail|Cadeia de Caracteres|O endereço de email que é exibido aos usuários.|
|defenderSecurityCenterHelpPhone|Cadeia de Caracteres|O número de telefone ou a ID do Skype que é exibido aos usuários.|
|defenderSecurityCenterHelpURL|Cadeia de Caracteres|A URL do portal de ajuda exibida para os usuários.|
|defenderSecurityCenterNotificationsFromApp|[defenderSecurityCenterNotificationsFromAppType](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|Notificações a serem mostradas nas áreas exibidas do aplicativo. Os valores possíveis são: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.|
|defenderSecurityCenterITContactDisplay|[defenderSecurityCenterITContactDisplayType](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|Configure onde exibir informações de contato de TI para os usuários finais. Os valores possíveis são: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.|
|windowsDefenderTamperProtection|[windowsDefenderTamperProtectionOptions](../resources/intune-deviceconfig-windowsdefendertamperprotectionoptions.md)|Defina as configurações do Windows Defender TamperProtection. Os valores possíveis são: `notConfigured`, `enable`, `disable`.|
|firewallBlockStatefulFTP|Boolean|Bloqueia conexões de FTP com estado ao dispositivo|
|firewallIdleTimeoutForSecurityAssociationInSeconds|Int32|Configura o tempo limite ocioso das associações de segurança, em segundos, de 300 para 3.600, inclusive. Após esse período, as associações de segurança expirarão e serão excluídas. Valores válidos de 300 a 3.600|
|firewallPreSharedKeyEncodingMethod|[firewallPreSharedKeyEncodingMethodType](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|Selecione a codificação de chave pré-compartilhada a ser usada. Os valores possíveis são: `deviceDefault`, `none`, `utF8`.|
|firewallIPSecExemptionsNone|Booleano|Configura isenções de IPSec para nenhuma isenção|
|firewallIPSecExemptionsAllowNeighborDiscovery|Boolean|Configura isenções IPSec para permitir códigos do tipo ICMP IPv6 de descoberta de vizinhos|
|firewallIPSecExemptionsAllowICMP|Boolean|Configura isenções IPSec para permitir ICMP|
|firewallIPSecExemptionsAllowRouterDiscovery|Boolean|Configura isenções IPSec para permitir códigos do tipo ICMP IPv6 de descoberta de roteadores|
|firewallIPSecExemptionsAllowDHCP|Boolean|Configura isenções IPSec para permitir tráfego DHCP de IPv4 e IPv6|
|firewallCertificateRevocationListCheckMethod|[firewallCertificateRevocationListCheckMethodType](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|Especifique como a lista de certificados revogados deve ser imposta. Os valores possíveis são: `deviceDefault`, `none`, `attempt`, `require`.|
|firewallMergeKeyingModuleSettings|Boolean|Se um conjunto de autenticação não for totalmente suportado por um módulo de chave, direcione o módulo para ignorar apenas pacotes de autenticação não compatíveis, em vez de todo o conjunto|
|firewallPacketQueueingMethod|[firewallPacketQueueingMethodType](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|Configura como a fila de pacotes deve ser aplicada no cenário de gateway de túnel. Os valores possíveis são: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.|
|firewallProfileDomain|[windowsFirewallNetworkProfile](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|Define as configurações de perfil de firewall das redes do domínio|
|firewallProfilePublic|[windowsFirewallNetworkProfile](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|Define as configurações de perfil de firewall das redes públicas|
|firewallProfilePrivate|[windowsFirewallNetworkProfile](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|Define as configurações de perfil de firewall das redes privadas|
|defenderAdobeReaderLaunchChildProcess|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Valor que indica o comportamento do Adobe Reader da criação de processos filho. Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderAttackSurfaceReductionExcludedPaths|String collection|Lista de arquivos executáveis e pastas a serem excluídos das regras de redução de superfície de ataque|
|defenderOfficeAppsOtherProcessInjectionType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Valor que indica o comportamento dos aplicativos do Office injetando em outros processos. Os valores possíveis são: `userDefined`, `block`, `auditMode`, `warn`, `disable`.|
|defenderOfficeAppsOtherProcessInjection|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Valor que indica o comportamento dos aplicativos do Office injetando em outros processos. Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderOfficeCommunicationAppsLaunchChildProcess|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Valor que indica o comportamento dos aplicativos de comunicação do Office, incluindo o Microsoft Outlook, da criação de processos filho. Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderOfficeAppsExecutableContentCreationOrLaunchType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Valor que indica o comportamento de aplicativos/macros do Office criando ou iniciando conteúdo executável. Os valores possíveis são: `userDefined`, `block`, `auditMode`, `warn`, `disable`.|
|defenderOfficeAppsExecutableContentCreationOrLaunch|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Valor que indica o comportamento de aplicativos/macros do Office criando ou iniciando conteúdo executável. Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderOfficeAppsLaunchChildProcessType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Valor que indica o comportamento do aplicativo do Office iniciando processos filho. Os valores possíveis são: `userDefined`, `block`, `auditMode`, `warn`, `disable`.|
|defenderOfficeAppsLaunchChildProcess|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Valor que indica o comportamento do aplicativo do Office iniciando processos filho. Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderOfficeMacroCodeAllowWin32ImportsType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Valor que indica o comportamento das importações do Win32 do código macro no Office. Os valores possíveis são: `userDefined`, `block`, `auditMode`, `warn`, `disable`.|
|defenderOfficeMacroCodeAllowWin32Imports|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Valor que indica o comportamento das importações do Win32 do código macro no Office. Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderScriptObfuscatedMacroCodeType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Valor que indica o comportamento do código js/vbs/ps/macro ofuscado. Os valores possíveis são: `userDefined`, `block`, `auditMode`, `warn`, `disable`.|
|defenderScriptObfuscatedMacroCode|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Valor que indica o comportamento do código js/vbs/ps/macro ofuscado. Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderScriptDownloadedPayloadExecutionType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Valor que indica o comportamento de js/vbs executando o conteúdo baixado da Internet. Os valores possíveis são: `userDefined`, `block`, `auditMode`, `warn`, `disable`.|
|defenderScriptDownloadedPayloadExecution|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Valor que indica o comportamento de js/vbs executando o conteúdo baixado da Internet. Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderPreventCredentialStealingType|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Valor que indica se o roubo de credenciais do subsistema da autoridade de segurança local do Windows é permitido. Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderProcessCreationType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Valor que indica a resposta a criações de processo provenientes dos comandos PSExec e WMI. Os valores possíveis são: `userDefined`, `block`, `auditMode`, `warn`, `disable`.|
|defenderProcessCreation|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Valor que indica a resposta a criações de processo provenientes dos comandos PSExec e WMI. Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderUntrustedUSBProcessType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Valor que indica a resposta a processos não confiáveis e não assinados executados do USB. Os valores possíveis são: `userDefined`, `block`, `auditMode`, `warn`, `disable`.|
|defenderUntrustedUSBProcess|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Valor que indica a resposta a processos não confiáveis e não assinados executados do USB. Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderUntrustedExecutableType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Valor que indica a resposta a executáveis que não atendem a critérios de prevalência, idade ou lista confiável. Os valores possíveis são: `userDefined`, `block`, `auditMode`, `warn`, `disable`.|
|defenderUntrustedExecutable|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Valor que indica a resposta a executáveis que não atendem a critérios de prevalência, idade ou lista confiável. Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderEmailContentExecutionType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Valor que indica se a execução de conteúdo executável (exe, dll, ps, js, vbs etc.) deve ser descartada do email (webmail/mail-client). Os valores possíveis são: `userDefined`, `block`, `auditMode`, `warn`, `disable`.|
|defenderEmailContentExecution|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Valor que indica se a execução de conteúdo executável (exe, dll, ps, js, vbs etc.) deve ser descartada do email (webmail/mail-client). Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderAdvancedRansomewareProtectionType|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Valor que indica o uso de proteção avançada contra ransomeware. Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderGuardMyFoldersType|[folderProtectionType](../resources/intune-deviceconfig-folderprotectiontype.md)|Valor que indica o comportamento de pastas protegidas. Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.|
|defenderGuardedFoldersAllowedAppPaths|String collection|Lista de caminhos para execução com permissão para acessar as pastas protegidas|
|defenderAdditionalGuardedFolders|String collection|Lista de caminhos de pasta a serem adicionados à lista de pastas protegidas|
|defenderNetworkProtectionType|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Valor que indica o comportamento de NetworkProtection. Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderExploitProtectionXml|Binária|Conteúdo XML com informações sobre a proteção contra vulnerabilidades.|
|defenderExploitProtectionXmlFileName|String|Nome do arquivo do qual DefenderExploitProtectionXml foi obtido.|
|defenderSecurityCenterBlockExploitProtectionOverride|Boolean|Indica se o usuário será ou não impedido de substituir as configurações de Exploit Protection.|
|defenderBlockPersistenceThroughWmiType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Valor que indica o comportamento de persistência de bloco por meio da assinatura de evento WMI. Os valores possíveis são: `userDefined`, `block`, `auditMode`, `warn`, `disable`.|
|appLockerApplicationControl|[appLockerApplicationControlType](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|Permite que o administrador escolha quais tipos de aplicativo permitir nos dispositivos. Os valores possíveis são: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.|
|deviceGuardLocalSystemAuthorityCredentialGuardSettings|[deviceGuardLocalSystemAuthorityCredentialGuardType](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|Ative o Credential Guard quando o nível de segurança da plataforma com inicialização segura e segurança baseada em virtualização estiver habilitado. Os valores possíveis são: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`, `disable`.|
|deviceGuardEnableVirtualizationBasedSecurity|Booleano|Ativa a VBS (segurança baseada em virtualização).|
|deviceGuardEnableSecureBootWithDMA|Booleano|Essa propriedade será preterida em maio de 2019 e será substituída pela propriedade DeviceGuardSecureBootWithDMA. Especifica se o Nível de Segurança da Plataforma está habilitado na próxima reinicialização.|
|deviceGuardSecureBootWithDMA|[secureBootWithDMAType](../resources/intune-deviceconfig-securebootwithdmatype.md)|Especifica se o Nível de Segurança da Plataforma está habilitado na próxima reinicialização. Os valores possíveis são: `notConfigured`, `withoutDMA`, `withDMA`.|
|deviceGuardLaunchSystemGuard|[Capacitação](../resources/intune-deviceconfig-enablement.md)|Permite que o administrador de TI configure o lançamento do System Guard. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|smartScreenEnableInShell|Boolean|Permite que os administradores de TI configurem SmartScreen para Windows.|
|smartScreenBlockOverrideForFiles|Boolean|Permite que administradores de TI controlem se os usuários podem ignorar avisos do SmartScreen e executar arquivos maliciosos.|
|applicationGuardEnabled|Boolean|Habilitar o Windows Defender Application Guard|
|applicationGuardEnabledOptions|[applicationGuardEnabledOptions](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|Habilite Windows Defender Application Guard para builds mais recentes do Windows. Os valores possíveis são: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.|
|applicationGuardBlockFileTransfer|[applicationGuardBlockFileTransferType](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|Bloqueie a área de transferência para transferir o arquivo de imagem, o arquivo de texto ou nenhum deles. Os valores possíveis são: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.|
|applicationGuardBlockNonEnterpriseContent|Boolean|Impedir sites corporativos de carregar conteúdos que não sejam da empresa, como plug-ins de terceiros|
|applicationGuardAllowPersistence|Boolean|Permitir dados persistentes gerados por usuários dentro do contêiner do App Guard (favoritos, cookies, senhas da Web, etc.)|
|applicationGuardForceAuditing|Boolean|A auditoria forçada persistirá logs e eventos do Windows para atender aos critérios de segurança/conformidade (exemplos de evento são logon e logoff do usuário, uso de direitos de privilégios, instalação de software, as alterações do sistema, etc.)|
|applicationGuardBlockClipboardSharing|[applicationGuardBlockClipboardSharingType](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|Impedir a área de transferência de compartilhar dados do host para o contêiner, do contêiner para o host ou em ambas as direções. Os valores possíveis são: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.|
|applicationGuardAllowPrintToPDF|Boolean|Permitir a impressão em PDF pelo contêiner|
|applicationGuardAllowPrintToXPS|Boolean|Permitir a impressão em XPS pelo contêiner|
|applicationGuardAllowPrintToLocalPrinters|Boolean|Permitir a impressão em impressoras locais pelo contêiner|
|applicationGuardAllowPrintToNetworkPrinters|Boolean|Permitir a impressão em impressoras da rede pelo contêiner|
|applicationGuardAllowVirtualGPU|Booliano|Permitir que o Application Guard use GPU virtual|
|applicationGuardAllowFileSaveOnHost|Booleano|Permitir que os usuários baixem arquivos do Edge no contêiner do Application Guard e salve-os no sistema de arquivos do host|
|applicationGuardAllowCameraMicrophoneRedirection|Booleano|Obtém ou define se os aplicativos Microsoft Defender Application Guard podem acessar a câmera e o microfone do dispositivo.|
|applicationGuardCertificateThumbprints|String collection|Permite que determinados certificados raiz no nível do dispositivo sejam compartilhados com o Microsoft Defender Application Guard contêiner.|
|bitLockerAllowStandardUserEncryption|Booleano|Permite que o administrador permita que os usuários padrão habilitem o encrpytion durante Azure AD Join.|
|bitLockerDisableWarningForOtherDiskEncryption|Boolean|Permite que o administrador desabilite o aviso de outras criptografias de disco nas máquinas dos usuários.|
|bitLockerEnableStorageCardEncryptionOnMobile|Boolean|Permite que o administrador exija que a criptografia seja ativada usando BitLocker. Essa política é válida apenas para uma SKU móvel.|
|bitLockerEncryptDevice|Boolean|Permite que o administrador exija que a criptografia seja ativada usando BitLocker.|
|bitLockerSystemDrivePolicy|[bitLockerSystemDrivePolicy](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|Política de unidade do sistema BitLocker.|
|bitLockerFixedDrivePolicy|[bitLockerFixedDrivePolicy](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)|Política de unidade fixa do BitLocker.|
|bitLockerRemovableDrivePolicy|[bitLockerRemovableDrivePolicy](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|Política da unidade removível do BitLocker.|
|bitLockerRecoveryPasswordRotation|[bitLockerRecoveryPasswordRotationType](../resources/intune-deviceconfig-bitlockerrecoverypasswordrotationtype.md)|Essa configuração inicia uma rotação de senha de recuperação controlada pelo cliente após uma recuperação de unidade do sistema operacional (usando bootmgr ou WinRE). Os valores possíveis são: `notConfigured`, `disabled`, `enabledForAzureAd`, `enabledForAzureAdAndHybrid`.|
|defenderDisableScanArchiveFiles|Booleano|Permite ou não a verificação de arquivos.|
|defenderAllowScanArchiveFiles|Booleano|Permite ou não a verificação de arquivos.|
|defenderDisableBehaviorMonitoring|Booleano|Permite ou não Windows Defender de Monitoramento de Comportamento.|
|defenderAllowBehaviorMonitoring|Booleano|Permite ou não Windows Defender de Monitoramento de Comportamento.|
|defenderDisableCloudProtection|Booleano|Para proteger melhor seu computador, Windows Defender enviará informações à Microsoft sobre quaisquer problemas encontrados. A Microsoft analisará essas informações, aprenderá mais sobre problemas que afetam você e outros clientes e oferecerá soluções aprimoradas.|
|defenderAllowCloudProtection|Booliano|Para proteger melhor seu computador, Windows Defender enviará informações à Microsoft sobre quaisquer problemas encontrados. A Microsoft analisará essas informações, aprenderá mais sobre problemas que afetam você e outros clientes e oferecerá soluções aprimoradas.|
|defenderEnableScanIncomingMail|Booliano|Permite ou não a verificação de email.|
|defenderEnableScanMappedNetworkDrivesDuringFullScan|Booleano|Permite ou não permitir uma verificação completa de unidades de rede mapeadas.|
|defenderDisableScanRemovableDrivesDuringFullScan|Booleano|Permite ou não permitir uma verificação completa de unidades removíveis. Durante uma verificação rápida, as unidades removíveis ainda podem ser verificadas.|
|defenderAllowScanRemovableDrivesDuringFullScan|Booleano|Permite ou não permitir uma verificação completa de unidades removíveis. Durante uma verificação rápida, as unidades removíveis ainda podem ser verificadas.|
|defenderDisableScanDownloads|Booleano|Permite ou não Windows Defender de proteção IOAVP.|
|defenderAllowScanDownloads|Booleano|Permite ou não Windows Defender de proteção IOAVP.|
|defenderDisableIntrusionPreventionSystem|Booleano|Permite ou não Windows Defender de Prevenção contra Intrusões.|
|defenderAllowIntrusionPreventionSystem|Booleano|Permite ou não Windows Defender de Prevenção contra Intrusões.|
|defenderDisableOnAccessProtection|Booleano|Permite ou não Windows Defender funcionalidade de Proteção de Acesso.|
|defenderAllowOnAccessProtection|Booleano|Permite ou não Windows Defender funcionalidade de Proteção de Acesso.|
|defenderDisableRealTimeMonitoring|Booleano|Permite ou não permitir Windows Defender de Monitoramento em Tempo Real.|
|defenderAllowRealTimeMonitoring|Booleano|Permite ou não permitir Windows Defender de Monitoramento em Tempo Real.|
|defenderDisableScanNetworkFiles|Booleano|Permite ou não permitir uma verificação de arquivos de rede.|
|defenderAllowScanNetworkFiles|Booleano|Permite ou não permitir uma verificação de arquivos de rede.|
|defenderDisableScanScriptsLoadedInInternetExplorer|Booleano|Permite ou não a Windows Defender verificação de script.|
|defenderAllowScanScriptsLoadedInInternetExplorer|Booleano|Permite ou não a Windows Defender verificação de script.|
|defenderBlockEndUserAccess|Boolean|Permite ou não o acesso do usuário à Windows Defender usuário. Se não for permitido, todas Windows Defender notificações também serão suprimidas.|
|defenderAllowEndUserAccess|Booleano|Permite ou não o acesso do usuário à Windows Defender usuário. Se não for permitido, todas Windows Defender notificações também serão suprimidas.|
|defenderScanMaxCpuPercentage|Int32|Representa o fator de carga média da CPU para o Windows Defender verificação (em porcentagem). O valor padrão é 50. Valores válidos de 0 a 100|
|defenderCheckForSignaturesBeforeRunningScan|Booleano|Essa configuração de política permite que você gerencie se uma verificação de novas definições de vírus e spyware ocorrerá antes de executar uma verificação.|
|defenderCloudBlockLevel|[defenderCloudBlockLevelType](../resources/intune-deviceconfig-defendercloudblockleveltype.md)|Adicionado no Windows 10, versão 1709. Essa configuração de política determina o quão agressivo Windows Defender Antivírus bloqueio e verificação de arquivos suspeitos. O tipo de valor é inteiro. Esse recurso requer a configuração "Ingressar no Microsoft MAPS" habilitada para funcionar. Os valores possíveis são: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.|
|defenderCloudExtendedTimeoutInSeconds|Int32|Adicionado no Windows 10, versão 1709. Esse recurso permite Windows Defender Antivírus bloquear um arquivo suspeito por até 60 segundos e digitalizar na nuvem para garantir que ele seja seguro. O tipo de valor é inteiro, o intervalo é de 0 a 50. Esse recurso depende de três outras configurações do MAPS, todas devem ser habilitadas: "Configurar o recurso 'Bloquear à Primeira Vista'; " Ingressar no Microsoft MAPS"; "Enviar exemplos de arquivo quando uma análise adicional for necessária". Valores válidos de 0 a 50|
|defenderDaysBeforeDeletingQuarantinedMalware|Int32|Período de tempo (em dias) em que os itens de quarentena serão armazenados no sistema. Valores válidos de 0 a 90|
|defenderDisableCatchupFullScan|Booleano|Essa configuração de política permite que você configure verificações de atualização para verificações completas agendadas. Uma verificação de atualização é uma verificação iniciada porque uma verificação agendada regularmente foi perdida. Normalmente, essas verificações agendadas são perdidas porque o computador foi desativado no horário agendado.|
|defenderDisableCatchupQuickScan|Booleano|Essa configuração de política permite que você configure verificações de atualização para verificações rápidas agendadas. Uma verificação de atualização é uma verificação iniciada porque uma verificação agendada regularmente foi perdida. Normalmente, essas verificações agendadas são perdidas porque o computador foi desativado no horário agendado.|
|defenderEnableLowCpuPriority|Booleano|Essa configuração de política permite habilitar ou desabilitar a baixa prioridade de CPU para verificações agendadas.|
|defenderFileExtensionsToExclude|String collection|Extensões de arquivo a serem excluídas das verificações e da proteção em tempo real.|
|defenderFilesAndFoldersToExclude|String collection|Arquivos e pastas a serem excluídos das verificações e da proteção em tempo real.|
|defenderProcessesToExclude|String collection|Processos a serem excluídos das verificações e da proteção em tempo real.|
|defenderPotentiallyUnwantedAppAction|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Adicionado no Windows 10, versão 1607. Especifica o nível de detecção para PUAs (aplicativos potencialmente indesejados). Windows Defender alerta quando um software potencialmente indesejado está sendo baixado ou tenta instalar-se no computador. Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderScanDirection|[defenderRealtimeScanDirection](../resources/intune-deviceconfig-defenderrealtimescandirection.md)|Controla quais conjuntos de arquivos devem ser monitorados. Os valores possíveis são: `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.|
|defenderScanType|[defenderScanType](../resources/intune-deviceconfig-defenderscantype.md)|Seleciona se deseja executar uma verificação rápida ou uma verificação completa. Os valores possíveis são: `userDefined`, `disabled`, `quick`, `full`.|
|defenderScheduledQuickScanTime|TimeOfDay|Seleciona a hora do dia em que a verificação Windows Defender rápida deve ser executada. Por exemplo, um valor de 0=12:00AM, um valor de 60=1:00AM, um valor de 120=2:00 e assim por diante, até um valor de 1380=11:00PM. O valor padrão é 120|
|defenderScheduledScanDay|[Weeklyschedule](../resources/intune-deviceconfig-weeklyschedule.md)|Seleciona o dia em que a verificação Windows Defender deve ser executada. Os valores possíveis são: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.|
|defenderScheduledScanTime|TimeOfDay|Seleciona a hora do dia em que a verificação Windows Defender deve ser executada.|
|defenderSignatureUpdateIntervalInHours|Int32|Especifica o intervalo (em horas) que será usado para verificar se há assinaturas, portanto, em vez de usar ScheduleDay e ScheduleTime, a verificação de novas assinaturas será definida de acordo com o intervalo. Valores válidos de 0 a 24|
|defenderSubmitSamplesConsentType|[defenderSubmitSamplesConsentType](../resources/intune-deviceconfig-defendersubmitsamplesconsenttype.md)|Verifica o nível de consentimento do usuário no Windows Defender para enviar dados. Os valores possíveis são: `sendSafeSamplesAutomatically`, `alwaysPrompt`, `neverSend`, `sendAllSamplesAutomatically`.|
|defenderDetectedMalwareActions|[defenderDetectedMalwareActions](../resources/intune-deviceconfig-defenderdetectedmalwareactions.md)|Permite que um administrador especifique quaisquer níveis de severidade de ameaça válidos e a ID de ação padrão correspondente a ser tomada.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|groupAssignments|[Coleção deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|A lista de atribuições de grupo para o perfil de configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|assignments|Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatuses|Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Status da instalação da configuração de dispositivo por dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatuses|Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Status de instalação da configuração do dispositivo por usuário. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Visão geral de status de dispositivos para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Visão geral de status de usuários para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Visão geral de dispositivos de configuração para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10EndpointProtectionConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "String"
    ],
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "String",
    "maxOSVersion": "String",
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "String",
    "name": "String",
    "ruleType": "String"
  },
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "dmaGuardDeviceEnumerationPolicy": "String",
  "firewallRules": [
    {
      "@odata.type": "microsoft.graph.windowsFirewallRule",
      "displayName": "String",
      "description": "String",
      "packageFamilyName": "String",
      "filePath": "String",
      "serviceName": "String",
      "protocol": 1024,
      "localPortRanges": [
        "String"
      ],
      "remotePortRanges": [
        "String"
      ],
      "localAddressRanges": [
        "String"
      ],
      "remoteAddressRanges": [
        "String"
      ],
      "profileTypes": "String",
      "action": "String",
      "trafficDirection": "String",
      "interfaceTypes": "String",
      "edgeTraversal": "String",
      "localUserAuthorizations": "String"
    }
  ],
  "userRightsAccessCredentialManagerAsTrustedCaller": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsAllowAccessFromNetwork": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsBlockAccessFromNetwork": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsActAsPartOfTheOperatingSystem": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsLocalLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsDenyLocalLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsBackupData": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsChangeSystemTime": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsCreateGlobalObjects": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsCreatePageFile": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsCreatePermanentSharedObjects": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsCreateSymbolicLinks": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsCreateToken": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsDebugPrograms": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsRemoteDesktopServicesLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsDelegation": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsGenerateSecurityAudits": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsImpersonateClient": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsIncreaseSchedulingPriority": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsLoadUnloadDrivers": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsLockMemory": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsManageAuditingAndSecurityLogs": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsManageVolumes": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsModifyFirmwareEnvironment": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsModifyObjectLabels": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsProfileSingleProcess": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsRemoteShutdown": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsRestoreData": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsTakeOwnership": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "xboxServicesEnableXboxGameSaveTask": true,
  "xboxServicesAccessoryManagementServiceStartupMode": "String",
  "xboxServicesLiveAuthManagerServiceStartupMode": "String",
  "xboxServicesLiveGameSaveServiceStartupMode": "String",
  "xboxServicesLiveNetworkingServiceStartupMode": "String",
  "localSecurityOptionsBlockMicrosoftAccounts": true,
  "localSecurityOptionsBlockRemoteLogonWithBlankPassword": true,
  "localSecurityOptionsDisableAdministratorAccount": true,
  "localSecurityOptionsAdministratorAccountName": "String",
  "localSecurityOptionsDisableGuestAccount": true,
  "localSecurityOptionsGuestAccountName": "String",
  "localSecurityOptionsAllowUndockWithoutHavingToLogon": true,
  "localSecurityOptionsBlockUsersInstallingPrinterDrivers": true,
  "localSecurityOptionsBlockRemoteOpticalDriveAccess": true,
  "localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser": "String",
  "localSecurityOptionsMachineInactivityLimit": 1024,
  "localSecurityOptionsMachineInactivityLimitInMinutes": 1024,
  "localSecurityOptionsDoNotRequireCtrlAltDel": true,
  "localSecurityOptionsHideLastSignedInUser": true,
  "localSecurityOptionsHideUsernameAtSignIn": true,
  "localSecurityOptionsLogOnMessageTitle": "String",
  "localSecurityOptionsLogOnMessageText": "String",
  "localSecurityOptionsAllowPKU2UAuthenticationRequests": true,
  "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool": true,
  "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager": "String",
  "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients": "String",
  "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers": "String",
  "lanManagerAuthenticationLevel": "String",
  "lanManagerWorkstationDisableInsecureGuestLogons": true,
  "localSecurityOptionsClearVirtualMemoryPageFile": true,
  "localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn": true,
  "localSecurityOptionsAllowUIAccessApplicationElevation": true,
  "localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations": true,
  "localSecurityOptionsOnlyElevateSignedExecutables": true,
  "localSecurityOptionsAdministratorElevationPromptBehavior": "String",
  "localSecurityOptionsStandardUserElevationPromptBehavior": "String",
  "localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation": true,
  "localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation": true,
  "localSecurityOptionsAllowUIAccessApplicationsForSecureLocations": true,
  "localSecurityOptionsUseAdminApprovalMode": true,
  "localSecurityOptionsUseAdminApprovalModeForAdministrators": true,
  "localSecurityOptionsInformationShownOnLockScreen": "String",
  "localSecurityOptionsInformationDisplayedOnLockScreen": "String",
  "localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees": true,
  "localSecurityOptionsClientDigitallySignCommunicationsAlways": true,
  "localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers": true,
  "localSecurityOptionsDisableServerDigitallySignCommunicationsAlways": true,
  "localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees": true,
  "localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares": true,
  "localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts": true,
  "localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares": true,
  "localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange": true,
  "localSecurityOptionsSmartCardRemovalBehavior": "String",
  "defenderSecurityCenterDisableAppBrowserUI": true,
  "defenderSecurityCenterDisableFamilyUI": true,
  "defenderSecurityCenterDisableHealthUI": true,
  "defenderSecurityCenterDisableNetworkUI": true,
  "defenderSecurityCenterDisableVirusUI": true,
  "defenderSecurityCenterDisableAccountUI": true,
  "defenderSecurityCenterDisableClearTpmUI": true,
  "defenderSecurityCenterDisableHardwareUI": true,
  "defenderSecurityCenterDisableNotificationAreaUI": true,
  "defenderSecurityCenterDisableRansomwareUI": true,
  "defenderSecurityCenterDisableSecureBootUI": true,
  "defenderSecurityCenterDisableTroubleshootingUI": true,
  "defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI": true,
  "defenderSecurityCenterOrganizationDisplayName": "String",
  "defenderSecurityCenterHelpEmail": "String",
  "defenderSecurityCenterHelpPhone": "String",
  "defenderSecurityCenterHelpURL": "String",
  "defenderSecurityCenterNotificationsFromApp": "String",
  "defenderSecurityCenterITContactDisplay": "String",
  "windowsDefenderTamperProtection": "String",
  "firewallBlockStatefulFTP": true,
  "firewallIdleTimeoutForSecurityAssociationInSeconds": 1024,
  "firewallPreSharedKeyEncodingMethod": "String",
  "firewallIPSecExemptionsNone": true,
  "firewallIPSecExemptionsAllowNeighborDiscovery": true,
  "firewallIPSecExemptionsAllowICMP": true,
  "firewallIPSecExemptionsAllowRouterDiscovery": true,
  "firewallIPSecExemptionsAllowDHCP": true,
  "firewallCertificateRevocationListCheckMethod": "String",
  "firewallMergeKeyingModuleSettings": true,
  "firewallPacketQueueingMethod": "String",
  "firewallProfileDomain": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "String",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "firewallProfilePublic": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "String",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "firewallProfilePrivate": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "String",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "defenderAdobeReaderLaunchChildProcess": "String",
  "defenderAttackSurfaceReductionExcludedPaths": [
    "String"
  ],
  "defenderOfficeAppsOtherProcessInjectionType": "String",
  "defenderOfficeAppsOtherProcessInjection": "String",
  "defenderOfficeCommunicationAppsLaunchChildProcess": "String",
  "defenderOfficeAppsExecutableContentCreationOrLaunchType": "String",
  "defenderOfficeAppsExecutableContentCreationOrLaunch": "String",
  "defenderOfficeAppsLaunchChildProcessType": "String",
  "defenderOfficeAppsLaunchChildProcess": "String",
  "defenderOfficeMacroCodeAllowWin32ImportsType": "String",
  "defenderOfficeMacroCodeAllowWin32Imports": "String",
  "defenderScriptObfuscatedMacroCodeType": "String",
  "defenderScriptObfuscatedMacroCode": "String",
  "defenderScriptDownloadedPayloadExecutionType": "String",
  "defenderScriptDownloadedPayloadExecution": "String",
  "defenderPreventCredentialStealingType": "String",
  "defenderProcessCreationType": "String",
  "defenderProcessCreation": "String",
  "defenderUntrustedUSBProcessType": "String",
  "defenderUntrustedUSBProcess": "String",
  "defenderUntrustedExecutableType": "String",
  "defenderUntrustedExecutable": "String",
  "defenderEmailContentExecutionType": "String",
  "defenderEmailContentExecution": "String",
  "defenderAdvancedRansomewareProtectionType": "String",
  "defenderGuardMyFoldersType": "String",
  "defenderGuardedFoldersAllowedAppPaths": [
    "String"
  ],
  "defenderAdditionalGuardedFolders": [
    "String"
  ],
  "defenderNetworkProtectionType": "String",
  "defenderExploitProtectionXml": "binary",
  "defenderExploitProtectionXmlFileName": "String",
  "defenderSecurityCenterBlockExploitProtectionOverride": true,
  "defenderBlockPersistenceThroughWmiType": "String",
  "appLockerApplicationControl": "String",
  "deviceGuardLocalSystemAuthorityCredentialGuardSettings": "String",
  "deviceGuardEnableVirtualizationBasedSecurity": true,
  "deviceGuardEnableSecureBootWithDMA": true,
  "deviceGuardSecureBootWithDMA": "String",
  "deviceGuardLaunchSystemGuard": "String",
  "smartScreenEnableInShell": true,
  "smartScreenBlockOverrideForFiles": true,
  "applicationGuardEnabled": true,
  "applicationGuardEnabledOptions": "String",
  "applicationGuardBlockFileTransfer": "String",
  "applicationGuardBlockNonEnterpriseContent": true,
  "applicationGuardAllowPersistence": true,
  "applicationGuardForceAuditing": true,
  "applicationGuardBlockClipboardSharing": "String",
  "applicationGuardAllowPrintToPDF": true,
  "applicationGuardAllowPrintToXPS": true,
  "applicationGuardAllowPrintToLocalPrinters": true,
  "applicationGuardAllowPrintToNetworkPrinters": true,
  "applicationGuardAllowVirtualGPU": true,
  "applicationGuardAllowFileSaveOnHost": true,
  "applicationGuardAllowCameraMicrophoneRedirection": true,
  "applicationGuardCertificateThumbprints": [
    "String"
  ],
  "bitLockerAllowStandardUserEncryption": true,
  "bitLockerDisableWarningForOtherDiskEncryption": true,
  "bitLockerEnableStorageCardEncryptionOnMobile": true,
  "bitLockerEncryptDevice": true,
  "bitLockerSystemDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerSystemDrivePolicy",
    "encryptionMethod": "String",
    "startupAuthenticationRequired": true,
    "startupAuthenticationBlockWithoutTpmChip": true,
    "startupAuthenticationTpmUsage": "String",
    "startupAuthenticationTpmPinUsage": "String",
    "startupAuthenticationTpmKeyUsage": "String",
    "startupAuthenticationTpmPinAndKeyUsage": "String",
    "minimumPinLength": 1024,
    "recoveryOptions": {
      "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
      "blockDataRecoveryAgent": true,
      "recoveryPasswordUsage": "String",
      "recoveryKeyUsage": "String",
      "hideRecoveryOptions": true,
      "enableRecoveryInformationSaveToStore": true,
      "recoveryInformationToStore": "String",
      "enableBitLockerAfterRecoveryInformationToStore": true
    },
    "prebootRecoveryEnableMessageAndUrl": true,
    "prebootRecoveryMessage": "String",
    "prebootRecoveryUrl": "String"
  },
  "bitLockerFixedDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerFixedDrivePolicy",
    "encryptionMethod": "String",
    "requireEncryptionForWriteAccess": true,
    "recoveryOptions": {
      "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
      "blockDataRecoveryAgent": true,
      "recoveryPasswordUsage": "String",
      "recoveryKeyUsage": "String",
      "hideRecoveryOptions": true,
      "enableRecoveryInformationSaveToStore": true,
      "recoveryInformationToStore": "String",
      "enableBitLockerAfterRecoveryInformationToStore": true
    }
  },
  "bitLockerRemovableDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
    "encryptionMethod": "String",
    "requireEncryptionForWriteAccess": true,
    "blockCrossOrganizationWriteAccess": true
  },
  "bitLockerRecoveryPasswordRotation": "String",
  "defenderDisableScanArchiveFiles": true,
  "defenderAllowScanArchiveFiles": true,
  "defenderDisableBehaviorMonitoring": true,
  "defenderAllowBehaviorMonitoring": true,
  "defenderDisableCloudProtection": true,
  "defenderAllowCloudProtection": true,
  "defenderEnableScanIncomingMail": true,
  "defenderEnableScanMappedNetworkDrivesDuringFullScan": true,
  "defenderDisableScanRemovableDrivesDuringFullScan": true,
  "defenderAllowScanRemovableDrivesDuringFullScan": true,
  "defenderDisableScanDownloads": true,
  "defenderAllowScanDownloads": true,
  "defenderDisableIntrusionPreventionSystem": true,
  "defenderAllowIntrusionPreventionSystem": true,
  "defenderDisableOnAccessProtection": true,
  "defenderAllowOnAccessProtection": true,
  "defenderDisableRealTimeMonitoring": true,
  "defenderAllowRealTimeMonitoring": true,
  "defenderDisableScanNetworkFiles": true,
  "defenderAllowScanNetworkFiles": true,
  "defenderDisableScanScriptsLoadedInInternetExplorer": true,
  "defenderAllowScanScriptsLoadedInInternetExplorer": true,
  "defenderBlockEndUserAccess": true,
  "defenderAllowEndUserAccess": true,
  "defenderScanMaxCpuPercentage": 1024,
  "defenderCheckForSignaturesBeforeRunningScan": true,
  "defenderCloudBlockLevel": "String",
  "defenderCloudExtendedTimeoutInSeconds": 1024,
  "defenderDaysBeforeDeletingQuarantinedMalware": 1024,
  "defenderDisableCatchupFullScan": true,
  "defenderDisableCatchupQuickScan": true,
  "defenderEnableLowCpuPriority": true,
  "defenderFileExtensionsToExclude": [
    "String"
  ],
  "defenderFilesAndFoldersToExclude": [
    "String"
  ],
  "defenderProcessesToExclude": [
    "String"
  ],
  "defenderPotentiallyUnwantedAppAction": "String",
  "defenderScanDirection": "String",
  "defenderScanType": "String",
  "defenderScheduledQuickScanTime": "String (time of day)",
  "defenderScheduledScanDay": "String",
  "defenderScheduledScanTime": "String (time of day)",
  "defenderSignatureUpdateIntervalInHours": 1024,
  "defenderSubmitSamplesConsentType": "String",
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "String",
    "moderateSeverity": "String",
    "highSeverity": "String",
    "severeSeverity": "String"
  }
}
```




