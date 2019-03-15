---
title: Tipo de recurso windows10EndpointProtectionConfiguration
description: Este tópico fornece descrições dos métodos declarados, das propriedades e das relações expostos pelo recurso Windows10EndpointProtectionConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a4f034a6b35c1ae8bd8172a20c5da0ee2e818623
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571701"
---
# <a name="windows10endpointprotectionconfiguration-resource-type"></a>Tipo de recurso windows10EndpointProtectionConfiguration

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

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
|id|String|Chave da entidade. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de marcas de escopo para esta instância de entidade. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|supportsScopeTags|Boolean|Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo. A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure. Essa propriedade é somente leitura. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|descrição|String|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|String|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|versão|Int32|Versão da configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|dmaGuardDeviceEnumerationPolicy|[dmaGuardDeviceEnumerationPolicyType](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|Essa política destina-se a fornecer segurança adicional contra dispositivos compatíveis com DMA externo. Permite mais controle sobre a enumeração de dispositivos compatíveis com DMA externo incompatíveis com o remapeamento de DMA/isolamento de memória do dispositivo e área restrita. Essa política só entra em vigor quando a proteção DMA de kernel é suportada e habilitada pelo firmware do sistema. A proteção DMA de kernel é um recurso de plataforma que não pode ser controlado via política ou pelo usuário final. É preciso ter suporte do sistema no momento da fabricação. Para verificar se o sistema suporta a proteção DMA de kernel, verifique o campo proteção DMA de kernel na página Resumo de MSINFO32. exe. Os valores possíveis são: `deviceDefault`, `blockAll`, `allowAll`.|
|firewallRules|coleção [windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md)|Define as configurações da regra de firewall. Essa coleção pode conter um máximo de 150 elementos.|
|userRightsAccessCredentialManagerAsTrustedCaller|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Esse direito de usuário é usado pelo Gerenciador de credenciais durante o backup/restauração. As credenciais salvas dos usuários podem ser comprometidas se esse privilégio for dado a outras entidades. Há suporte apenas para os Estados não configurado e permitido|
|userRightsAllowAccessFromNetwork|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Esse direito de usuário determina quais usuários e grupos têm permissão para se conectar ao computador pela rede. O estado permitido é suportado.|
|userRightsBlockAccessFromNetwork|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Esse direito de usuário determina quais usuários e grupos são bloqueados para se conectarem ao computador pela rede. Há suporte para o bloco de estado.|
|userRightsActAsPartOfTheOperatingSystem|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Esse direito de usuário permite que um processo represente qualquer usuário sem autenticação. Portanto, o processo pode ter acesso aos mesmos recursos locais que esse usuário. Há suporte apenas para os Estados não configurado e permitido|
|userRightsLocalLogOn|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Esse direito de usuário determina quais usuários podem fazer logon no computador. Estados não conFigurados, permitidos e bloqueados são todos suportados |
|userRightsBackupData|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Esse direito de usuário determina quais usuários podem ignorar permissões de arquivo, diretório, registro e outros objetos persistentes ao fazer backup de arquivos e diretórios. Há suporte apenas para os Estados não configurado e permitido|
|userRightsChangeSystemTime|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Este direito de usuário determina quais usuários e grupos podem alterar a hora e a data no relógio interno do computador. Há suporte apenas para os Estados não configurado e permitido|
|userRightsCreateGlobalObjects|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Configuração de segurança que determina se os usuários podem criar objetos globais que estão disponíveis para todas as sessões. Os usuários que podem criar objetos globais podem afetar processos executados em sessões de outros usuários, o que pode levar a falhas de aplicativos ou corrupção de dados. Há suporte apenas para os Estados não configurado e permitido|
|userRightsCreatePageFile|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Esse direito de usuário determina quais usuários e grupos podem chamar uma API interna para criar e alterar o tamanho de um arquivo de paginação. Há suporte apenas para os Estados não configurado e permitido|
|userRightsCreatePermanentSharedObjects|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Este direito de usuário determina quais contas podem ser usadas por processos para criar um objeto de diretório usando o Gerenciador de objetos. Há suporte apenas para os Estados não configurado e permitido|
|userRightsCreateSymbolicLinks|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Esse direito de usuário determina se o usuário pode criar um link simbólico do computador no qual está conectado. Há suporte apenas para os Estados não configurado e permitido|
|userRightsCreateToken|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Esse direito de usuário determina quais usuários/grupos podem ser usados por processos para criar um token que pode ser usado para obter acesso a qualquer recurso local quando o processo usa uma API interna para criar um token de acesso. Há suporte apenas para os Estados não configurado e permitido|
|userRightsDebugPrograms|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Esse direito de usuário determina quais usuários podem anexar um depurador a qualquer processo ou ao kernel. Há suporte apenas para os Estados não configurado e permitido|
|userRightsRemoteDesktopServicesLogOn|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Este direito de usuário determina quais usuários e grupos estão proibidos de fazer logon como um cliente de serviços de área de trabalho remota. Há suporte apenas para os Estados não conFigurados e bloqueados|
|userRightsDelegation|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Este direito de usuário determina quais usuários podem definir a configuração confiável para delegação em um objeto de usuário ou computador. Há suporte apenas para os Estados não conFigurados e permitidos.|
|userRightsGenerateSecurityAudits|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Este direito de usuário determina quais contas podem ser usadas por um processo para adicionar entradas ao log de segurança. O log de segurança é usado para rastrear o acesso de sistema não autorizado.  Há suporte apenas para os Estados não conFigurados e permitidos.|
|userRightsImpersonateClient|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|A atribuição desse direito de usuário a um usuário permite que programas executados em nome desse usuário representem um cliente. A exigência desse direito de usuário para esse tipo de representação impede que um usuário não autorizado convença um cliente a se conectar a um serviço que ele criou e, em seguida, representando esse cliente, o que pode elevar as permissões do usuário não autorizado para níveis administrativos ou de sistema. Há suporte apenas para os Estados não conFigurados e permitidos.|
|userRightsIncreaseSchedulingPriority|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Este direito de usuário determina quais contas podem usar um processo com acesso de propriedade de gravação a outro processo para aumentar a prioridade de execução atribuída ao outro processo. Há suporte apenas para os Estados não conFigurados e permitidos.|
|userRightsLoadUnloadDrivers|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Esse direito de usuário determina quais usuários podem carregar e descarregar dinamicamente drivers de dispositivo ou outro código no modo kernel. Há suporte apenas para os Estados não conFigurados e permitidos.|
|userRightsLockMemory|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Esse direito de usuário determina quais contas podem usar um processo para manter os dados na memória física, o que impede que o sistema pagine os dados para a memória virtual em disco. Há suporte apenas para os Estados não conFigurados e permitidos.|
|userRightsManageAuditingAndSecurityLogs|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Esse direito de usuário determina quais usuários podem especificar opções de auditoria de acesso a objetos para recursos individuais, como arquivos, objetos do Active Directory e chaves do registro. Há suporte apenas para os Estados não conFigurados e permitidos.|
|userRightsManageVolumes|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Esse direito de usuário determina quais usuários e grupos podem executar tarefas de manutenção em um volume, como a desfragmentação remota. Há suporte apenas para os Estados não conFigurados e permitidos.|
|userRightsModifyFirmwareEnvironment|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Esse direito de usuário determina quem pode modificar os valores de ambiente de firmware. Há suporte apenas para os Estados não conFigurados e permitidos.|
|userRightsModifyObjectLabels|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Este direito de usuário determina quais contas de usuário podem modificar o rótulo de integridade de objetos, como arquivos, chaves de registro ou processos pertencentes a outros usuários. Há suporte apenas para os Estados não conFigurados e permitidos.|
|userRightsProfileSingleProcess|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Esse direito de usuário determina quais usuários podem usar ferramentas de monitoramento de desempenho para monitorar o desempenho de processos do sistema. Há suporte apenas para os Estados não conFigurados e permitidos.|
|userRightsRemoteShutdown|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Esse direito de usuário determina quais usuários têm permissão para desligar um computador de um local remoto na rede. O mau uso desse direito de usuário pode resultar em uma negação de serviço. Há suporte apenas para os Estados não conFigurados e permitidos.|
|userRightsRestoreData|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Esse direito de usuário determina quais usuários podem ignorar permissões de arquivo, diretório, registro e outros objetos persistentes ao restaurar backups de arquivos e diretórios e determina quais usuários podem definir qualquer entidade de segurança válida como o proprietário de um objeto. Há suporte apenas para os Estados não conFigurados e permitidos.|
|userRightsTakeOwnership|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Esse direito de usuário determina quais usuários podem assumir a propriedade de qualquer objeto protegível no sistema, incluindo objetos do Active Directory, arquivos e pastas, impressoras, chaves do registro, processos e threads. Há suporte apenas para os Estados não conFigurados e permitidos.|
|userRightsRegisterProcessAsService|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Essa configuração de segurança determina quais contas de serviço são impedidas de registrar um processo como um serviço. Observação: esta configuração de segurança não se aplica às contas de sistema, serviço local ou serviço de rede. Só há suporte para o estado bloqueado.|
|xboxServicesEnableXboxGameSaveTask|Boolean|Essa configuração determina se o salvamento de jogos do Xbox está habilitado (1) ou desabilitado (0).|
|xboxServicesAccessoryManagementServiceStartupMode|[inStarttype](../resources/intune-deviceconfig-servicestarttype.md)|Esta configuração determina se o tipo de início do serviço de gerenciamento de acessórios é automático (2), manual (3), desabilitado (4). Padrão: manual. Os valores possíveis são: `manual`, `automatic`, `disabled`.|
|xboxServicesLiveAuthManagerServiceStartupMode|[inStarttype](../resources/intune-deviceconfig-servicestarttype.md)|Essa configuração determina se o tipo de início do serviço do Live Authentication Manager é automático (2), manual (3), desabilitado (4). Padrão: manual. Os valores possíveis são: `manual`, `automatic`, `disabled`.|
|xboxServicesLiveGameSaveServiceStartupMode|[inStarttype](../resources/intune-deviceconfig-servicestarttype.md)|Essa configuração determina se o tipo de início do serviço de salvamento do Live Game é automático (2), manual (3), desabilitado (4). Padrão: manual. Os valores possíveis são: `manual`, `automatic`, `disabled`.|
|xboxServicesLiveNetworkingServiceStartupMode|[inStarttype](../resources/intune-deviceconfig-servicestarttype.md)|Esta configuração determina se o tipo de início do serviço de rede é automático (2), manual (3), desabilitado (4). Padrão: manual. Os valores possíveis são: `manual`, `automatic`, `disabled`.|
|localSecurityOptionsBlockMicrosoftAccounts|Boolean|Impedir que os usuários adicionem novas contas da Microsoft a este computador.|
|localSecurityOptionsBlockRemoteLogonWithBlankPassword|Boolean|Habilitar contas locais que não estão protegidas por senha para fazer logon de locais diferentes do dispositivo físico. O padrão é habilitado|
|localSecurityOptionsDisableAdministratorAccount|Boolean|Determina se a conta de administrador local está habilitada ou desabilitada.|
|localSecurityOptionsAdministratorAccountName|String|Defina um nome de conta diferente a ser associado ao identificador de segurança (SID) da conta "administrador".|
|localSecurityOptionsDisableGuestAccount|Boolean|Determina se a conta de convidado está habilitada ou desabilitada.|
|localSecurityOptionsGuestAccountName|String|Defina um nome de conta diferente a ser associado ao identificador de segurança (SID) da conta "convidado".|
|localSecurityOptionsAllowUndockWithoutHavingToLogon|Boolean|Impedir que um computador portátil seja desencaixado sem ter que fazer logon.|
|localSecurityOptionsBlockUsersInstallingPrinterDrivers|Boolean|Restringir a instalação dos drivers de impressora como parte da conexão a uma impressora compartilhada somente para administradores.|
|localSecurityOptionsBlockRemoteOpticalDriveAccess|Boolean|Habilitar essa configuração permite que somente o usuário conectado interativamente acesse a mídia de CD-ROM.|
|localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser|[localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|Defina quem tem permissão para formatar e ejetar a mídia NTFS removível. Os valores possíveis são: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.|
|localSecurityOptionsMachineInactivityLimit|Int32|Defina o máximo de minutos de inatividade na tela de logon do desktop interativo até que a proteção de tela seja executada. Valores válidos de 0 a 9999|
|localSecurityOptionsMachineInactivityLimitInMinutes|Int32|Defina o máximo de minutos de inatividade na tela de logon do desktop interativo até que a proteção de tela seja executada. Valores válidos de 0 a 9999|
|localSecurityOptionsDoNotRequireCtrlAltDel|Boolean|Exigir CTRL + ALT + DEL para ser pressionada para que um usuário possa fazer logon.|
|localSecurityOptionsHideLastSignedInUser|Boolean|Não exibe o nome de usuário da última pessoa que entrou neste dispositivo.|
|localSecurityOptionsHideUsernameAtSignIn|Boolean|Não exibe o nome de usuário da pessoa que está entrando neste dispositivo depois que as credenciais são inseridas e antes da área de trabalho do dispositivo ser exibida.|
|localSecurityOptionsLogOnMessageTitle|String|Defina o título da mensagem para usuários que tentam fazer logon.|
|localSecurityOptionsLogOnMessageText|String|Definir o texto da mensagem para usuários que tentam fazer logon.|
|localSecurityOptionsAllowPKU2UAuthenticationRequests|Boolean|Bloquear solicitações de autenticação PKU2U para este dispositivo para usar identidades online.|
|localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool|Boolean|Boolean do auxiliar da interface do usuário para entidade LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager|
|localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager|String|Edite a cadeia de caracteres de definição de descritor de segurança padrão para permitir ou impedir que usuários e grupos façam chamadas remotas para o SAM.|
|localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients|[localSecurityOptionsMinimumSessionSecurity](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|Essa configuração de segurança permite que um cliente exija a negociação de criptografia de 128 bits e/ou segurança de sessão NTLMv2. Os valores possíveis são: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.|
|localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers|[localSecurityOptionsMinimumSessionSecurity](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|Essa configuração de segurança permite que um servidor exija a negociação de criptografia de 128 bits e/ou segurança de sessão NTLMv2. Os valores possíveis são: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.|
|lanManagerAuthenticationLevel|[lanManagerAuthenticationLevel](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|Essa configuração de segurança determina qual protocolo de autenticação de desafio/resposta é usado para logons de rede. Os valores possíveis são: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.|
|lanManagerWorkstationDisableInsecureGuestLogons|Boolean|Se for habilitada, o cliente SMB permitirá logons de convidados não seguros. Se não configurada, o cliente SMB rejeitará logons de convidados não seguros.|
|localSecurityOptionsClearVirtualMemoryPageFile|Boolean|Configuração de segurança que determina se o arquivo de paginação de memória virtual será limpo quando o sistema for desligado.|
|localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn|Boolean|Configuração de segurança que determina se um computador pode ser desligado sem a necessidade de fazer logon no Windows.|
|localSecurityOptionsAllowUIAccessApplicationElevation|Boolean|Permitir que aplicativos UIAccess solicitem elevação sem usar a área de trabalho segura.|
|localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations|Boolean|Virtualizar falhas de gravação de arquivo e registro para locais por usuário|
|localSecurityOptionsOnlyElevateSignedExecutables|Boolean|Impor a validação de caminho de certificação PKI para um determinado arquivo executável antes que seja permitido executar.|
|localSecurityOptionsAdministratorElevationPromptBehavior|[localSecurityOptionsAdministratorElevationPromptBehaviorType](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|Definir o comportamento do prompt de elevação para administradores no modo de aprovação de administrador. Os valores possíveis são: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.|
|localSecurityOptionsStandardUserElevationPromptBehavior|[localSecurityOptionsStandardUserElevationPromptBehaviorType](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|Definir o comportamento do prompt de elevação para usuários padrão. Os valores possíveis são: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.|
|localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation|Boolean|Habilite todas as solicitações de elevação para ir para a área de trabalho do usuário interativo, e não para a área de trabalho segura. As configurações de política de comportamento de prompt para administradores e usuários padrão são usadas.|
|localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation|Boolean|Instalações de aplicativos que exigem privilégios elevados solicitarão credenciais de administrador. O padrão é habilitado|
|localSecurityOptionsAllowUIAccessApplicationsForSecureLocations|Boolean|Permitir que aplicativos UIAccess solicitem elevação sem usar a área de trabalho segura. O padrão é habilitado|
|localSecurityOptionsUseAdminApprovalMode|Boolean|Define se a conta de administrador interna usa o modo de aprovação de administrador ou executa todos os aplicativos com privilégios de administrador completo. O padrão é habilitado|
|localSecurityOptionsUseAdminApprovalModeForAdministrators|Boolean|Definir se o modo de aprovação de administrador e todas as configurações de política de UAC estão habilitados, o padrão é habilitado|
|localSecurityOptionsInformationShownOnLockScreen|[localSecurityOptionsInformationShownOnLockScreenType](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|Configure as informações do usuário que são exibidas quando a sessão está bloqueada. Se não configurada, o nome de exibição do usuário, o domínio e o nome de usuário serão exibidos. Os valores possíveis são: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.|
|localSecurityOptionsInformationDisplayedOnLockScreen|[localSecurityOptionsInformationDisplayedOnLockScreenType](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|Configure as informações do usuário que são exibidas quando a sessão está bloqueada. Se não configurada, o nome de exibição do usuário, o domínio e o nome de usuário serão exibidos. Os valores possíveis são: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.|
|localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees|Boolean|Configuração de segurança que determina se o cliente SMB tentará negociar assinatura de pacote SMB.|
|localSecurityOptionsClientDigitallySignCommunicationsAlways|Boolean|Configuração de segurança que determina se a assinatura de pacotes é necessária para o componente do cliente SMB.|
|localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers|Boolean|Se essa configuração de segurança estiver habilitada, o redirecionador de bloco de mensagens de servidor (SMB) terá permissão para enviar senhas de texto não criptografado para servidores SMB não Microsoft que não ofereçam suporte à criptografia de senha durante a autenticação.|
|localSecurityOptionsDisableServerDigitallySignCommunicationsAlways|Boolean|Configuração de segurança que determina se a assinatura de pacotes é necessária para o componente do servidor SMB.|
|localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees|Boolean|Configuração de segurança que determina se o servidor SMB negociará assinatura de pacote SMB com clientes que solicitarem.|
|localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares|Boolean|Por padrão, essa configuração de segurança restringe o acesso anônimo a compartilhamentos e pipes para as configurações de pipes nomeados que podem ser acessados anonimamente e comPartilhamentos que podem ser acessados anonimamente|
|localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts|Boolean|Essa configuração de segurança determina quais permissões adicionais serão concedidas para conexões anônimas com o computador.|
|localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares|Boolean|Configuração de segurança que determina se os usuários anônimos devem executar determinadas atividades, como enumeração de nomes de contas de domínio e compartilhamentos de rede.|
|localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange|Boolean|Essa configuração de segurança determina se, na próxima alteração de senha, o valor de hash do LM (LAN Manager) para a nova senha é armazenado. Ele não é armazenado por padrão.|
|localSecurityOptionsSmartCardRemovalBehavior|[localSecurityOptionsSmartCardRemovalBehaviorType](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)|Essa configuração de segurança determina o que acontece quando o cartão inteligente de um usuário conectado é removido do leitor de cartão inteligente. Os valores possíveis são: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.|
|defenderSecurityCenterDisableAppBrowserUI|Boolean|Usado para desabilitar a exibição da área de proteção de aplicativo e navegador.|
|defenderSecurityCenterDisableFamilyUI|Boolean|Usado para desabilitar a exibição da área de opções da família.|
|defenderSecurityCenterDisableHealthUI|Boolean|Usado para desabilitar a exibição da área de desempenho e integridade do dispositivo.|
|defenderSecurityCenterDisableNetworkUI|Boolean|Usado para desabilitar a exibição da área de firewall e proteção de rede.|
|defenderSecurityCenterDisableVirusUI|Boolean|Usado para desabilitar a exibição da área de proteção contra vírus e ameaças.|
|defenderSecurityCenterDisableAccountUI|Boolean|Usado para desabilitar a exibição da área de proteção da conta.|
|defenderSecurityCenterDisableClearTpmUI|Boolean|Usado para desabilitar a exibição do botão limpar TPM.|
|defenderSecurityCenterDisableHardwareUI|Boolean|Usado para desabilitar a exibição da área de proteção de hardware.|
|defenderSecurityCenterDisableNotificationAreaUI|Boolean|Usado para desabilitar a exibição do controle da área de notificação. O usuário precisa sair e entrar ou reiniciar o computador para que essa configuração entre em vigor.|
|defenderSecurityCenterDisableRansomwareUI|Boolean|Usado para desabilitar a exibição da área de proteção contra ransomware. |
|defenderSecurityCenterDisableSecureBootUI|Boolean|Usado para desabilitar a exibição da área de inicialização segura sob segurança de dispositivo.|
|defenderSecurityCenterDisableTroubleshootingUI|Boolean|Usado para desabilitar a exibição do processo de segurança Solucionando problemas de segurança de dispositivo.|
|defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI|Boolean|Usado para desabilitar a exibição de atualizar o firmware do TPM quando um firmware vulnerável é detectado.|
|defenderSecurityCenterOrganizationDisplayName|String|O nome da empresa que é exibido para os usuários.|
|defenderSecurityCenterHelpEmail|String|O endereço de email que é exibido para os usuários.|
|defenderSecurityCenterHelpPhone|String|O número de telefone ou Skype ID que é exibido aos usuários.|
|defenderSecurityCenterHelpURL|String|A URL do portal da ajuda que é exibida para os usuários.|
|defenderSecurityCenterNotificationsFromApp|[defenderSecurityCenterNotificationsFromAppType](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|Notificações para mostrar das áreas de aplicativo exibidas. Os valores possíveis são: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.|
|defenderSecurityCenterITContactDisplay|[defenderSecurityCenterITContactDisplayType](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|Configurar onde exibir informações de contato de ti para usuários finais. Os valores possíveis são: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.|
|firewallBlockStatefulFTP|Boolean|Bloqueia conexões de FTP com estado ao dispositivo|
|firewallIdleTimeoutForSecurityAssociationInSeconds|Int32|Configura o tempo limite ocioso das associações de segurança, em segundos, de 300 para 3.600, inclusive. Após esse período, as associações de segurança expirarão e serão excluídas. Valores válidos de 300 a 3.600|
|firewallPreSharedKeyEncodingMethod|[firewallPreSharedKeyEncodingMethodType](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|Selecione a codificação de chave pré-compartilhada a ser usada. Os valores possíveis são: `deviceDefault`, `none`, `utF8`.|
|firewallIPSecExemptionsAllowNeighborDiscovery|Boolean|Configura isenções IPSec para permitir códigos do tipo ICMP IPv6 de descoberta de vizinhos|
|firewallIPSecExemptionsAllowICMP|Boolean|Configura isenções IPSec para permitir ICMP|
|firewallIPSecExemptionsAllowRouterDiscovery|Boolean|Configura isenções IPSec para permitir códigos do tipo ICMP IPv6 de descoberta de roteadores|
|firewallIPSecExemptionsAllowDHCP|Boolean|Configura isenções IPSec para permitir tráfego DHCP de IPv4 e IPv6|
|firewallCertificateRevocationListCheckMethod|[firewallCertificateRevocationListCheckMethodType](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|Especifique como a lista de certificados revogados será imposta. Os valores possíveis são: `deviceDefault`, `none`, `attempt`, `require`.|
|firewallMergeKeyingModuleSettings|Boolean|Se um conjunto de autenticação não for totalmente suportado por um módulo de chave, direcione o módulo para ignorar apenas pacotes de autenticação não compatíveis, em vez de todo o conjunto|
|firewallPacketQueueingMethod|[firewallPacketQueueingMethodType](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|Configura como o enfileiramento de pacotes deve ser aplicado no cenário de gateway de túnel. Os valores possíveis são: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.|
|firewallProfileDomain|[windowsFirewallNetworkProfile](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|Define as configurações de perfil de firewall das redes do domínio|
|firewallProfilePublic|[windowsFirewallNetworkProfile](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|Define as configurações de perfil de firewall das redes públicas|
|firewallProfilePrivate|[windowsFirewallNetworkProfile](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|Define as configurações de perfil de firewall das redes privadas|
|defenderAdobeReaderLaunchChildProcess|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|O valor que indica o comportamento do Adobe Reader de criar processos filhos. Os valores possíveis são: `userDefined`, `enable`, `auditMode`.|
|defenderAttackSurfaceReductionExcludedPaths|String collection|Lista de arquivos executáveis e pastas a serem excluídos das regras de redução de superfície de ataque|
|defenderOfficeAppsOtherProcessInjectionType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Valor que indica o comportamento dos aplicativos do Office que injetam em outros processos. Os valores possíveis são: `userDefined`, `block`, `auditMode`.|
|defenderOfficeAppsOtherProcessInjection|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Valor que indica o comportamento dos aplicativos do Office que injetam em outros processos. Os valores possíveis são: `userDefined`, `enable`, `auditMode`.|
|defenderOfficeCommunicationAppsLaunchChildProcess|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|O valor que indica o comportamento dos aplicativos de comunicação do Office, incluindo o Microsoft Outlook, da criação de processos filhos. Os valores possíveis são: `userDefined`, `enable`, `auditMode`.|
|defenderOfficeAppsExecutableContentCreationOrLaunchType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Valor que indica o comportamento de aplicativos/macros do Office criando ou iniciando conteúdo executável. Os valores possíveis são: `userDefined`, `block`, `auditMode`.|
|defenderOfficeAppsExecutableContentCreationOrLaunch|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Valor que indica o comportamento de aplicativos/macros do Office criando ou iniciando conteúdo executável. Os valores possíveis são: `userDefined`, `enable`, `auditMode`.|
|defenderOfficeAppsLaunchChildProcessType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Valor que indica o comportamento do aplicativo do Office que está iniciando processos filhos. Os valores possíveis são: `userDefined`, `block`, `auditMode`.|
|defenderOfficeAppsLaunchChildProcess|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Valor que indica o comportamento do aplicativo do Office que está iniciando processos filhos. Os valores possíveis são: `userDefined`, `enable`, `auditMode`.|
|defenderOfficeMacroCodeAllowWin32ImportsType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Valor que indica o comportamento das importações Win32 do código de macro no Office. Os valores possíveis são: `userDefined`, `block`, `auditMode`.|
|defenderOfficeMacroCodeAllowWin32Imports|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Valor que indica o comportamento das importações Win32 do código de macro no Office. Os valores possíveis são: `userDefined`, `enable`, `auditMode`.|
|defenderScriptObfuscatedMacroCodeType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Valor que indica o comportamento do código js/vbs/PS/macro ofuscado. Os valores possíveis são: `userDefined`, `block`, `auditMode`.|
|defenderScriptObfuscatedMacroCode|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Valor que indica o comportamento do código js/vbs/PS/macro ofuscado. Os valores possíveis são: `userDefined`, `enable`, `auditMode`.|
|defenderScriptDownloadedPayloadExecutionType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|O valor que indica o comportamento do js/vbs executando a carga baixada da Internet. Os valores possíveis são: `userDefined`, `block`, `auditMode`.|
|defenderScriptDownloadedPayloadExecution|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|O valor que indica o comportamento do js/vbs executando a carga baixada da Internet. Os valores possíveis são: `userDefined`, `enable`, `auditMode`.|
|defenderPreventCredentialStealingType|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Valor que indica se a credencial que está sendo roubada do subsistema de autoridade de segurança local do Windows é permitida. Os valores possíveis são: `userDefined`, `enable`, `auditMode`.|
|defenderProcessCreationType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|O valor que indica a resposta a criações de processos que se originam de comandos do PSExec e WMI. Os valores possíveis são: `userDefined`, `block`, `auditMode`.|
|defenderProcessCreation|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|O valor que indica a resposta a criações de processos que se originam de comandos do PSExec e WMI. Os valores possíveis são: `userDefined`, `enable`, `auditMode`.|
|defenderUntrustedUSBProcessType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Valor que indica a resposta a processos não confiáveis e não assinados executados no USB. Os valores possíveis são: `userDefined`, `block`, `auditMode`.|
|defenderUntrustedUSBProcess|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Valor que indica a resposta a processos não confiáveis e não assinados executados no USB. Os valores possíveis são: `userDefined`, `enable`, `auditMode`.|
|defenderUntrustedExecutableType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Valor que indica a resposta a executáveis que não atendem a um critério de lista predominante, de idade ou confiável. Os valores possíveis são: `userDefined`, `block`, `auditMode`.|
|defenderUntrustedExecutable|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Valor que indica a resposta a executáveis que não atendem a um critério de lista predominante, de idade ou confiável. Os valores possíveis são: `userDefined`, `enable`, `auditMode`.|
|defenderEmailContentExecutionType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|O valor que indica se a execução do conteúdo executável (exe, dll, PS, js, vbs, etc.) deve ser cancelada de email (webmail/email). Os valores possíveis são: `userDefined`, `block`, `auditMode`.|
|defenderEmailContentExecution|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|O valor que indica se a execução do conteúdo executável (exe, dll, PS, js, vbs, etc.) deve ser cancelada de email (webmail/email). Os valores possíveis são: `userDefined`, `enable`, `auditMode`.|
|defenderAdvancedRansomewareProtectionType|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|O valor que indica o uso da proteção avançada contra o Ransomeware. Os valores possíveis são: `userDefined`, `enable`, `auditMode`.|
|defenderGuardMyFoldersType|[folderProtectionType](../resources/intune-deviceconfig-folderprotectiontype.md)|Valor que indica o comportamento das pastas protegidas. Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.|
|defenderGuardedFoldersAllowedAppPaths|Coleção de cadeias de caracteres|Lista de caminhos para execução com permissão para acessar as pastas protegidas|
|defenderAdditionalGuardedFolders|String collection|Lista de caminhos de pasta a serem adicionados à lista de pastas protegidas|
|defenderNetworkProtectionType|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Valor que indica o comportamento de NetworkProtection. Os valores possíveis são: `userDefined`, `enable`, `auditMode`.|
|defenderExploitProtectionXml|Binária|Conteúdo XML com informações sobre a proteção contra vulnerabilidades.|
|defenderExploitProtectionXmlFileName|String|Nome do arquivo do qual DefenderExploitProtectionXml foi obtido.|
|defenderSecurityCenterBlockExploitProtectionOverride|Boolean|Indica se o usuário será ou não impedido de substituir as configurações de Exploit Protection.|
|appLockerApplicationControl|[appLockerApplicationControlType](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|Permite que o administrador escolha quais tipos de aplicativo permitir nos dispositivos. Os valores possíveis são: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.|
|deviceGuardLocalSystemAuthorityCredentialGuardSettings|[deviceGuardLocalSystemAuthorityCredentialGuardType](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|Ative o Credential Guard quando o nível de segurança da plataforma com segurança baseada em inicialização e virtualização segura estiverem habilitados. Os valores possíveis são: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.|
|deviceGuardEnableVirtualizationBasedSecurity|Boolean|Ativa a segurança baseada em virtualização (VBS).|
|deviceGuardEnableSecureBootWithDMA|Boolean|Especifica se o nível de segurança da plataforma está habilitado na próxima reinicialização.|
|deviceGuardLaunchSystemGuard|[habilitação](../resources/intune-shared-enablement.md)|Permite que o administrador de ti configure o lançamento do System Guard. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|smartScreenEnableInShell|Boolean|Permite que os administradores de TI configurem SmartScreen para Windows.|
|smartScreenBlockOverrideForFiles|Boolean|Permite que administradores de TI controlem se os usuários podem ignorar avisos do SmartScreen e executar arquivos maliciosos.|
|applicationGuardEnabled|Boolean|Habilitar o Windows Defender Application Guard|
|applicationGuardEnabledOptions|[applicationGuardEnabledOptions](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|Habilitar o Windows Defender Application Guard para novas versões do Windows. Os valores possíveis são: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.|
|applicationGuardBlockFileTransfer|[applicationGuardBlockFileTransferType](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|Bloquear a área de transferência para transferir o arquivo de imagem, o arquivo de texto ou nenhum deles. Os valores possíveis são: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.|
|applicationGuardBlockNonEnterpriseContent|Boolean|Impedir sites corporativos de carregar conteúdos que não sejam da empresa, como plug-ins de terceiros|
|applicationGuardAllowPersistence|Boolean|Permitir dados persistentes gerados por usuários dentro do contêiner do App Guard (favoritos, cookies, senhas da Web, etc.)|
|applicationGuardForceAuditing|Boolean|A auditoria forçada persistirá logs e eventos do Windows para atender aos critérios de segurança/conformidade (exemplos de evento são logon e logoff do usuário, uso de direitos de privilégios, instalação de software, as alterações do sistema, etc.)|
|applicationGuardBlockClipboardSharing|[applicationGuardBlockClipboardSharingType](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|Impedir a área de transferência de compartilhar dados do host para o contêiner, do contêiner para o host ou em ambas as direções. Os valores possíveis são: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.|
|applicationGuardAllowPrintToPDF|Boolean|Permitir a impressão em PDF pelo contêiner|
|applicationGuardAllowPrintToXPS|Boolean|Permitir a impressão em XPS pelo contêiner|
|applicationGuardAllowPrintToLocalPrinters|Boolean|Permitir a impressão em impressoras locais pelo contêiner|
|applicationGuardAllowPrintToNetworkPrinters|Boolean|Permitir a impressão em impressoras da rede pelo contêiner|
|applicationGuardAllowVirtualGPU|Boolean|Permitir que o Application Guard use virtual GPU|
|applicationGuardAllowFileSaveOnHost|Boolean|Permitir que os usuários baixem arquivos da borda no contêiner do Application Guard e salve-os no sistema de arquivos host|
|bitLockerAllowStandardUserEncryption|Boolean|Permite que o administrador permita que os usuários padrão habilitem o encrpytion durante o ingresso no Azure AD.|
|bitLockerDisableWarningForOtherDiskEncryption|Boolean|Permite que o administrador desabilite o aviso de outras criptografias de disco nas máquinas dos usuários.|
|bitLockerEnableStorageCardEncryptionOnMobile|Boolean|Permite que o administrador exija que a criptografia seja ativada usando BitLocker. Essa política é válida apenas para uma SKU móvel.|
|bitLockerEncryptDevice|Boolean|Permite que o administrador exija que a criptografia seja ativada usando BitLocker.|
|bitLockerSystemDrivePolicy|[bitLockerSystemDrivePolicy](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|Política de unidade de sistema BitLocker.|
|bitLockerFixedDrivePolicy|[bitLockerFixedDrivePolicy](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)|Política de unidade fixa do BitLocker.|
|bitLockerRemovableDrivePolicy|[bitLockerRemovableDrivePolicy](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|Política da unidade removível do BitLocker.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|groupAssignments|coleção [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|A lista de atribuições de grupo para o perfil de configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
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
  "userRightsRegisterProcessAsService": {
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
  "firewallBlockStatefulFTP": true,
  "firewallIdleTimeoutForSecurityAssociationInSeconds": 1024,
  "firewallPreSharedKeyEncodingMethod": "String",
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
  "appLockerApplicationControl": "String",
  "deviceGuardLocalSystemAuthorityCredentialGuardSettings": "String",
  "deviceGuardEnableVirtualizationBasedSecurity": true,
  "deviceGuardEnableSecureBootWithDMA": true,
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
  }
}
```




