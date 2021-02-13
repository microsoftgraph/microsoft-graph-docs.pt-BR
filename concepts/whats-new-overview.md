---
title: Novidades do Microsoft Graph
description: O que há de novo no Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 6779d735c1c445ce3910fa649b3273405fc7d6da
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159385"
---
# <a name="whats-new-in-microsoft-graph"></a>Novidades do Microsoft Graph

Veja os destaques das novidades nos dois últimos meses do Microsoft Graph, [o que foi adicionado anteriormente](whats-new-earlier.md) e como você pode [compartilhar suas ideias](#want-to-stay-in-the-loop). Para obter uma lista detalhada de atualizações no nível da API, consulte o [registro de alterações da API](https://developer.microsoft.com/graph/changelog/). 

> [!IMPORTANT]
> Os recursos, incluindo APIs e ferramentas, no status de _visualização_, podem ser alterados sem aviso prévio e alguns talvez nunca sejam promovidos ao status DG. Não use os recursos de visualização em aplicativos de produção.


## <a name="february-2021-new-in-preview-only"></a>Fevereiro de 2021: novo apenas em pré-visualização

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
- Atribua informações de geolocalização a um recurso de [pacote de acesso](/graph/api/resources/accesspackage?view=graph-rest-beta&preserve-view=true) na [solicitação de atribuição de pacote de acesso](/graph/api/resources/accesspackageassignmentrequest?view=graph-rest-beta&preserve-view=true).
- Obtenha uma lista de todos os [ambientes de recursos de pacote de acesso](/graph/api/resources/accesspackageresourceenvironment?view=graph-rest-beta&preserve-view=true) que representam as geolocalizações que armazenam os recursos do Microsoft Office SharePoint Online.

### <a name="reports--microsoft-365-usage-reports"></a>Relatórios | Relatórios de uso do Microsoft 365
Obtenha mais propriedades incluídas em [relatórios detalhados para uso do site SharePoint](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-beta&preserve-view=true): anonymousLinkCount, companyLinkCount, externalSharing, geolocation, secureLinkForGuestCount, secureLinkForMemberCount, siteSensitivityLabelId, e unmanagedDevicePolicy.

### <a name="use-sdks"></a>Usar SDKs
Experimente a versão prévia do [Microsoft Graph Java SDK v3](https://github.com/microsoftgraph/msgraph-sdk-java/tree/feature/v3)! Para mais informações, confira a [postagem no blog](https://developer.microsoft.com/graph/blogs/announcing-the-public-preview-of-microsoft-graph-java-sdk-v3/) relacionada.

## <a name="january-2021-new-in-preview-only"></a>Janeiro de 2021: novo apenas em pré-visualização

### <a name="cloud-communications"></a>Comunicações na nuvem
- Organize um evento ao vivo como uma [reuniãoOnline ](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true) - veja um [exemplo](/graph/api/application-post-onlinemeetings?view=graph-rest-beta&preserve-view=true#example-3-create-a-live-event-with-a-user-token). 
- Obtenha o fluxo de conteúdo de um [relatório de participante](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true#example-4-retrieve-the-attendee-report-of-a-live-event), [gravação](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true#example-5-retrieve-the-recording-of-a-live-event) ou gravação alternativa do evento ao vivo.
- Obtenha o status de [presença](/graph/api/resources/presence?view=graph-rest-beta&preserve-view=true) de um usuário que está [fora do escritório](/graph/api/resources/outofofficesettings?view=graph-rest-beta&preserve-view=true) e qualquer mensagem definida para esse status.

### <a name="devices-and-apps--cloud-pc"></a>Dispositivos e aplicativos | Cloud PC
- [Atualize uma senha de domínio do Active Directory ](/graph/api/cloudpconpremisesconnection-updateaddomainpassword?view=graph-rest-beta&preserve-view=true) para uma [conexão de rede local bem-sucedida](/graph/api/resources/cloudPcOnPremisesConnection?view=graph-rest-beta&preserve-view=true).
- [Executar verificações de integridade em uma conexão de rede local](/graph/api/cloudpconpremisesconnection-runhealthcheck?view=graph-rest-beta&preserve-view=true) agora pode expor 5 tipos de erros adicionais no recurso de [verificação de integridade da conexão local](/graph/api/resources/cloudpconpremisesconnectionhealthcheck?view=graph-rest-beta&preserve-view=true). Para obter mais informações sobre os tipos de erro, confira o [log de mudanças](https://developer.microsoft.com/graph/changelog) de janeiro de 2021.

### <a name="devices-and-apps--cloud-printing"></a>Dispositivos e aplicativos | Impressão na nuvem
- [Assine para alterar notificações de impressão em nuvens](universal-print-webhook-notifications.md) - quando um trabalho de impressão é iniciado, e quando o trabalho de impressão está pronto para ser baixado por uma impressora.
- Obtenha uma gama completa de [valores possíveis](/graph/api/resources/printerstatus?view=graph-rest-beta&preserve-view=true#printerprocessingstatedetail-values) para o status de uma [impressora](/graph/api/resources/printer?view=graph-rest-beta&preserve-view=true).
- Use permissões delegadas em aplicativos em nome do usuário conectado:
  - `PrinterShare.ReadBasic.All` para ler informações básicas sobre compartilhamentos de impressoras, excluindo informações de controle de acesso.
  - `PrintConnector.Read.All` para ler conectores de impressão.
  - `PrintConnector.ReadWrite.All` para ler ou gravar conectores de impressão.
  - `PrintJob.Create` para criar trabalhos de impressão e fazer upload de conteúdo para trabalhos de impressão.
  - `PrintSettings.Read.All` para ler as configurações de impressão de todo o locatário.
  - `PrintSettings.ReadWrite.All` para ler ou gravar configurações de impressão para todo o locatário.
  - `Reports.Read.All` para ler o resumo do uso de impressão por usuário especificado ou por impressora.

### <a name="education"></a>Educação
Use [configurações de tarefas](/graph/api/resources/educationAssignmentSettings?view=graph-rest-beta&preserve-view=true) a nível de classe para habilitar ou desabilitar a animação para comemorar a entrega de uma tarefa.

### <a name="groups"></a>Grupos
Obtenha o status de processamento de um grupo dinâmico baseado em regras usando a propriedade **membershipRuleProcessingStatus**. Isso é útil quando um atributo de um usuário é alterado, a associação do usuário em um [grupo Microsoft 365](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) baseado em regras é reavaliada com base nas regras de associação de grupo definidas para a organização. 

### <a name="identity-and-access--directory-management"></a>Identidade e acesso | Gerenciamento do diretório
Obter o [direito de uso](/graph/api/resources/UsageRight?view=graph-rest-beta&preserve-view=true) que um usuário ou dispositivo tem sobre um software de terceiros compilado no PowerApps, ou, direito de uso de um dispositivo sobre uma assinatura. O direito de uso inclui identificadores para o serviço ou produto correspondente, e o estado atual do direito de uso, como ativo, inativo, em alerta, ou em suspensão.

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e login
- Os aplicativos podem usar as permissões do aplicativo para permitir que os administradores gerenciem os [métodos de autenticação](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta&preserve-view=true) dos usuários.
- Suporte ao [Microsoft Authenticator](/graph/api/resources/microsoftauthenticatorauthenticationmethod?view=graph-rest-beta&preserve-view=true) como um método de autenticação de um usuário para entrar ou executar autenticação multifator no Azure Active Directory.
- Use a [política do Microsoft Authenticator](/graph/api/resources/microsoftauthenticatorauthenticationmethodconfiguration?view=graph-rest-beta&preserve-view=true) para definir as configurações e usuários ou grupos que podem usar o Microsoft Authenticator como método de autenticação. Use a política do Microsoft Authenticator no lugar da [política de login por telefone sem senha do Microsoft Authenticator](/graph/api/resources/passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration?view=graph-rest-beta&preserve-view=true), que está obsoleta. 
- Ofereça suporte ao [Windows Hello para Empresas](/graph/api/resources/windowshelloforbusinessauthenticationmethod?view=graph-rest-beta&preserve-view=true) como um método de autenticação para um usuário entrar em dispositivos Windows sem usar uma senha.

### <a name="reports--identity-and-access-reports"></a>Relatórios | Relatórios de identidade e acesso
- [Obtenha um relatório do número de usuários que estão registrados, ou que possuem vários recursos de registro](/graph/api/authenticationmethodsroot-usersregisteredbyfeature?view=graph-rest-beta&preserve-view=true), incluindo autenticação multifator, redefinição de senha de autoatendimento, ou autenticação sem senha.
- [Obtenha um relatório do número de usuários registrados para cada método de autenticação](/graph/api/authenticationmethodsroot-usersregisteredbymethod?view=graph-rest-beta&preserve-view=true), incluindo senha, Windows Hello para Empresas, ou logon de telefone sem senha.

## <a name="want-to-stay-in-the-loop"></a>Quer ficar por dentro?

Estas são algumas maneiras de se envolver:

- Existem cenários em que você gostaria que o Microsoft Graph oferecesse suporte? Sugira e vote em novos recursos no [Microsoft Graph User Voice](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).
    Alguns novos recursos são originados como solicitações populares da comunidade de desenvolvedores. A equipe do Microsoft Graph avalia regularmente as necessidades dos clientes e lança novos recursos na seguinte ordem:

    1. Estreia no status de visualização **_prévia_**. As atualizações da API REST relacionadas estão no ponto de extremidade beta (`https://graph.microsoft.com/beta`).  

    2. Promovido para o status de **_disponibilidade geral_ (GA)**, se um feedback suficiente indicar a viabilidade. Todas as atualizações da API REST relacionadas serão adicionadas ao ponto de extremidade do v 1.0 (`https://graph.microsoft.com/v1.0`). 
- Seja um membro ativo da comunidade do Microsoft Graph! [Participe](https://aka.ms/microsoftgraphcall) da chamada mensal à comunidade do Microsoft Graph.
- Inscreva-se no [programa para desenvolvedores do Microsoft 365](https://developer.microsoft.com/office/dev-program), ganhe uma assinatura gratuita do Microsoft 365 e comece a desenvolver!


## <a name="see-also"></a>Confira também
- Confira o [blog de desenvolvedores do Microsoft Graph](https://developer.microsoft.com/graph/blogs/) periodicamente para comunicados de lançamentos e recursos úteis.
- Navegue pelas informações das inclusões da API do Microsoft Graph e pelas atualizações de comportamento de API no [changelog](https://developer.microsoft.com/graph/changelog/).
- Encontre [destaques de versões anteriores](whats-new-earlier.md).
- Saiba mais sobre o [controle de versão, suporte e mudanças significativas de políticas do Microsoft Graph](versioning-and-support.md).
