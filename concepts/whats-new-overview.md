---
title: Novidades do Microsoft Graph
description: O que há de novo no Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 85c3a540c6aa2f0c7f3b00bf86a3e727997743b3
ms.sourcegitcommit: 93b6781adf2c889235022d34ab50e2a4d62760c5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/07/2020
ms.locfileid: "46589141"
---
# <a name="whats-new-in-microsoft-graph"></a>Novidades do Microsoft Graph

Veja os destaques das recentes novidades do Microsoft Graph, [o que foi adicionado anteriormente](whats-new-earlier.md) e como você pode [compartilhar suas idéias](#want-to-stay-in-the-loop). Para obter uma lista detalhada de atualizações no nível da API, consulte o [registro de alterações da API](changelog.md). 

> [!IMPORTANT]
> Os recursos, incluindo APIs e ferramentas, no status de _visualização_, podem ser alterados sem aviso prévio e alguns talvez nunca sejam promovidos ao status DG. Não use os recursos de visualização em aplicativos de produção.

## <a name="july-2020-new-and-generally-available"></a>Julho de 2020: novos e disponíveis para o público em geral

### <a name="calendar"></a>Calendário
GA do recurso que permite aos organizadores permitir propostas de horário alternativo para reuniões ou convites para [propor novos horários para uma reunião](outlook-calendar-meeting-proposals.md) quando eles [aceitarem provisoriamente](/graph/api/event-tentativelyaccept?view=graph-rest-1.0) ou [recusarem](/graph/api/event-decline?view=graph-rest-1.0) um evento.

### <a name="change-notifications"></a>Notificações de alteração
Removida do recurso [changeNotification](/graph/api/resources/changenotification) a propriedade **sequenceNumber** introduzida erroneamente.

### <a name="groups"></a>Grupos
DG das seguintes propriedades para a entidade [group](/graph/api/resources/group?view=graph-rest-v1.0): **assignedLabels**, **expirationDateTime**, **membershipRule**, **membershipRuleProcessingState**, **preferredLanguage**e **theme**.

### <a name="identity-and-access"></a>Identidade e acesso
- Remover um usuário como proprietário registrado ou usuário de um [dispositivo](/graph/api/resources/device).
- Acompanhe as alterações de representações locais de aplicativos recém-criadas, atualizadas ou deletadas (representada por recursos[servicePrincipals](/graph/api/resources/serviceprincipal)) e permissões delegadas concedidas (representadas por recursos[oAuth2PermissionGrant](/graph/api/resources/oauth2permissiongrant)) sem executar uma leitura completa de toda a coleção de recursos.
- GA da [política para reforçar o padrão de segurança](/graph/api/resources/identitysecuritydefaultsenforcementpolicy) que protege as organizações contra ataques comuns.

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e entrada
- GA de [políticas de acesso condicional](/graph/api/resources/conditionalAccessPolicy) que são regras personalizadas que definem um cenário de acesso.
- GA de [posições nomeadas](/graph/api/resources/namedLocation) representando regras personalizadas que definem os locais de rede usados em uma política de acesso condicional.

### <a name="schema-extensions"></a>Extensões de esquema
O recurso [extensões de esquema](/graph/api/resources/schemaextension) já está disponível para o público em geral no[Microsoft Cloud for US Government](/graph/deployments).

### <a name="teamwork"></a>Trabalho em equipe
Use as permissões delegadas de `TeamsAppInstallation.ReadForTeam` ou `TeamsAppInstallation.ReadWriteForTeam` ou permissões de aplicativo de `TeamsAppInstallation.ReadForTeam.All` ou `TeamsAppInstallation.ReadWriteForTeam.All` para [listar aplicativos instalados em uma equipe](/graph/api/teamsappinstallation-list).

## <a name="july-2020-new-in-preview-only"></a>Julho de 2020: novos apenas na visualização

### <a name="cloud-communications"></a>Comunicações na nuvem
- Use a operação [atualizar](/graph/api/onlinemeeting-update?view=graph-rest-beta) para atualizar **startDateTime**, **endDateTime**, **participantes**, ou propriedade de **assunto**de uma [reunião online](/graph/api/resources/onlinemeeting?view=graph-rest-beta).
- Inscreva-se para receber notificações sobre alterações na disponibilidade de um usuário do Microsoft Teams, conforme representado pelo recurso [presence](/graph/api/resources/presence?view=graph-rest-beta).

### <a name="cloud-communications--call-records"></a>Comunicação em nuvem | Gravação
- [Obtenha](/graph/api/callrecords-callrecord-getpstncalls?view=graph-rest-beta) os registros de chamadas da rede pública de telefonia comutada (PSTN).
- [Obtenha](/graph/api/callrecords-callrecord-getdirectroutingcalls?view=graph-rest-beta) os registros de chamadas de roteamento direto.

### <a name="compliance--ediscovery"></a>Conformidade | Descoberta eletrônica
Estréia dos [Casos de descoberta eletrônica](/graph/api/resources/ediscoverycase?view=graph-rest-beta) que podem conter responsáveis, bloqueios, coleções, conjuntos de revisão, e exportações que podem ser usados como evidência em casos jurídicos.
Os aplicativos agora podem [consultar](/graph/api/resources/reviewsetquery?view=graph-rest-beta) e [revisar o conjunto de dados](/graph/api/resources/reviewset?view=graph-rest-beta) coletado para uso em litígio, investigação ou solicitação regulatória. Esse estreia faz parte da [Descoberta Eletrônica Avançada](/microsoft-365/compliance/overview-ediscovery-20?view=o365-worldwide)do Microsoft 365.

### <a name="devices-and-apps--cloud-printing"></a>Dispositivos e aplicativos | Impressão na nuvem
- Use as permissões do aplicativo `Printer.ReadWrite.All` e a [codificação do IPP (Protocolo de Impressão via Internet)](https://tools.ietf.org/html/rfc8010) para [atualizar uma impressora ](/graph/api/printer-update?view=graph-rest-beta).
- Use uma das permissões de aplicativo, `PrintJob.ReadBasic.All`, `PrintJob.Read.All`, `PrintJob.ReadWriteBasic.All`ou `PrintJob.ReadWrite.All`, para [obter um trabalho de impressão](/graph/api/printjob-get?view=graph-rest-beta) ou [listar trabalhos de impressão para uma impressora](/graph/api/printer-list-jobs?view=graph-rest-beta).
- Quando [obtiver um trabalho de impressão](/graph/api/printjob-get?view=graph-rest-beta), use `$expand` para obter [tarefas de impressão](/graph/api/resources/printtask?view=graph-rest-beta) que estão executando ou que foram executadas no trabalho. Imprimir tarefas, [definições de tarefas](/graph/api/resources/printtaskdefinition?view=graph-rest-beta)e [disparadores de tarefas](/graph/api/resources/printtasktrigger?view=graph-rest-beta) são usados em [impressão segura](universal-print-concept-overview.md#extending-universal-print-to-support-pull-printing).
- [Redirecione um trabalho de impressão](/graph/api/printjob-redirect?view=graph-rest-beta) para uma impressora diferente, como parte da impressão segura.

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gerenciamento corporativo
Atualizações do Intune em [julho](changelog.md#july-2020) em beta.

### <a name="groups"></a>Grupos
Use a propriedade **isAssignableToRole** de um [grupo](/graph/api/resources/group?view=graph-rest-beta) do Microsoft 365 e a defina durante a criação de um grupo para indicar se ele pode ser atribuído a uma função do Azure AD. Isso [ajuda a gerenciar as atribuições de função no Azure AD](/azure/active-directory/users-groups-roles/roles-groups-concept), de modo que, em vez de atribuir um usuário individual a uma função do Azure AD, um administrador global ou um administrador de funções privilegiadas pode criar um grupo do Microsoft 365 e atribuir o grupo a essa função, para que quando os usuários se unam ao _grupo_, eles recebam a função pretendida indiretamente.

### <a name="identity-and-access"></a>Identidade e acesso
- [Adquira um token de acesso](/graph/api/synchronization-synchronization-acquireAccessToken?view=graph-rest-beta) para autorizar o serviço de provisionamento do Azure AD para provisionar usuários em um aplicativo.
- [Obtenha](/graph/api/entitlementmanagementsettings-get?view=graph-rest-beta) ou [atualize](/graph/api/entitlementmanagementsettings-update?view=graph-rest-beta) as configurações de gerenciamento de qualificação que controlam o acesso a grupos, aplicativos e sites do SharePoint Online para usuários internos e externos à sua organização. 

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e entrada
- Inclua os níveis de risco do usuário (`low`, `medium`, `high`, `none`) como consideração para aplicar uma [política de acesso condicional](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta).
- [Use a alteração de senha como um controle Grant](/graph/api/resources/conditionalaccessgrantcontrols?view=graph-rest-beta#special-considerations-when-using-passwordchange-as-a-control) para passar uma política de acesso condicional.
- Use um [provedor de conexão de ID aberta](/graph/api/resources/openidconnectprovider?view=graph-rest-beta) (ODIC) como um provedor de identidade em um locatário do Azure AD e um locatário do Azure AD B2C. Sua propriedade **claimsMapping** permite que o Azure AD [mapeie as declarações](/graph/api/resources/claimsmapping?view=graph-rest-beta) de um provedor OIDC para as declarações que o Azure AD reconhece e usa.

### <a name="people-and-workplace-intelligence--insights"></a>Inteligência social e do ambiente de trabalho | Ideias
Use mais o [controle de privacidade granular](insights-customize-item-insights-privacy.md) sobre a disponibilidade e a exibição das [informações do item](/graph/api/resources/iteminsights?view=graph-rest-beta) no Microsoft 365. Essas informações representam as relações entre um usuário e documentos no OneDrive for Business, calculadas usando uma análise avançada e técnicas de aprendizado de máquina. 

### <a name="people-and-workplace-intelligence--profile-card-customization"></a>Inteligência de pessoas e local de trabalho | Personalização de cartão de perfil
Os administradores podem [personalizar as propriedades expostas no cartão de perfil de suas organizações](add-properties-profilecard.md) usando a API para [propriedade de cartão de perfil](/graph/api/resources/profilecardproperty?view=graph-rest-beta).

### <a name="sites-and-lists"></a>Sites e listas
Acesse a taxonomia do [repositório de termos](/graph/api/resources/termstore-store?view=graph-rest-beta) a hierarquia que consite em recursos de [grupo](/graph/api/resources/termstore-group?view=graph-rest-beta), [definição](/graph/api/resources/termstore-set?view=graph-rest-beta), e [termo](/graph/api/resources/termstore-term?view=graph-rest-beta), e [relacione](/graph/api/resources/termstore-relation?view=graph-rest-beta) recursos entre os termos.

### <a name="workbooks-and-charts"></a>Pastas de trabalho e gráficos
[Obtenha o status e todos os resultados](/graph/api/workbookoperation-get?view=graph-rest-beta) de uma operação [de longa execução](/graph/api/resources/workbookoperation?view=graph-rest-beta) em uma [pasta de trabalho](/graph/api/resources/workbook?view=graph-rest-beta).

## <a name="june-2020-new-and-generally-available"></a>Junho de 2020: novos e disponíveis para o público em geral

### <a name="cloud-communications--online-meeting"></a>Comunicações na nuvem | Reunião online
- Use o cabeçalho HTTP `Accept-Language`ao [criar uma reunião online](/graph/api/application-post-onlinemeetings?view=graph-rest-1.0) para fornecer informações de participação baseadas no local.
- Use [createOrGet](/graph/api/onlinemeeting-createorget?view=graph-rest-1.0) para retornar uma reunião online que tenha um valor **externalId** específico ou, caso nenhum valor desse tipo exista, para simplificar a incorporação da reunião resultante a um calendário de terceiros.

### <a name="files"></a>Arquivos
- Suporte aprimorado à sincronização:
  - Use a propriedade **pendingOperations** para identificar quaisquer [operações](/graph/api/resources/pendingoperations) que possam atualizar o conteúdo binário de um arquivo [driveItem](/graph/api/resources/driveitem) e que estejam pendentes.
  - [Restaure](/graph/api/driveitem-restore) um **driveItem** que tenha sido excluído e esteja na lixeira do OneDrive pessoal.
- Obtenha ou defina a orientação de uma [foto](/graph/api/resources/photo). A configuração é compatível com o OneDrive Personal.
- Use o Algoritmo de Hash Seguro (SHA-256) para aprimorar a segurança e a integridade dos dados do [arquivo](/graph/api/resources/file).
- Use o parâmetro `deferCommit` para adiar a criação final ao [carregar geralmente um arquivo grande](/graph/api/driveitem-createuploadsession) no OneDrive for Business, até que um aplicativo faça uma solicitação para concluir o carregamento.
- Use a propriedade **fileSize** para fornecer uma estimativa como parte do parâmetro do **item**, de modo a fazer uma verificação de cota antes de [carregar um arquivo](/graph/api/driveitem-createuploadsession) no OneDrive pessoal.
- Localize [storagePlanInformation](/graph/api/resources/storageplaninformation) por meio da propriedade **cota** de um recurso de [unidade](/graph/api/resources/drive) para ver se existem planos de uma cota de armazenamento mais alta disponíveis.

### <a name="groups"></a>Grupos
Use as permissões de aplicativo `Group.Read.All` e `Group.ReadWrite.All` para obter recursos de uma [conversa](/graph/api/resources/conversation) do grupo e de uma [sequência de conversa](/graph/api/resources/conversationthread).

### <a name="identity-and-access"></a>Identidade e acesso 
- Disponibilidade generalizada de dois conjuntos de APIs de [proteção de identidade](/graph/api/resources/identityprotectionroot): APIs de [detecção de riscos](/graph/api/resources/riskdetection) e de [usuário arriscado](/graph/api/resources/riskyuser).

### <a name="security"></a>Segurança
- Rastreie o seguinte como propriedades de um [alerta](/graph/api/resources/alert?view=graph-rest-1.0):
  - IDs de incidentes relacionados ao alerta.
  - Identificar um [recurso](/graph/api/resources/securityResource?view=graph-rest-1.0#securityresourcetype-values) como atacado ou como um recurso relacionado no alerta.
  - Especificar os locais de origem e destino de uma [conexão de rede](/graph/api/resources/networkconnection?view=graph-rest-1.0) relacionada ao alerta.

### <a name="sites-and-lists"></a>Sites e listas
Especifique dados de localização geográfica em uma [definição de coluna](/graph/api/resources/columndefinition) para um recurso de uma [lista](/graph/api/resources/list) do SharePoint.

### <a name="teamwork"></a>Trabalho em equipe
- Use a permissão delegada [AppCatalog.Read.All](/graph/permissions-reference#appcatalog-resource-permissions) para listar [aplicativos](/graph/api/resources/teamsapp?view=graph-rest-1.0) do catálogo de aplicativos do Microsoft Teams.
- [Obtenha informações sobre a pasta](/graph/api/channel-get-filesfolder) que mapeia para a guia **Arquivos** de um [canal](/graph/api/resources/channel) do Teams.
- [Obtenha o do canal padrão](/graph/api/team-get-primarychannel) — rotulado como **Geral** — de uma [equipe](/graph/api/resources/team).


## <a name="june-2020-new-in-preview-only"></a>Junho de 2020: novos apenas na visualização

### <a name="calendar"></a>Calendário
Além de monitorar as alterações incrementais de eventos em um **calendarView** (um conjunto ou eventos delimitados por datas de início _e_ fim), use a função [delta](/graph/api/event-delta?view=graph-rest-beta) nos eventos de uma caixa de correio do usuário ou eventos em um calendário específico do usuário.

### <a name="cloud-communications--presence"></a>Comunicações na nuvem | Presença
[Obtenha o status de presença](/graph/api/presence-get?view=graph-rest-beta) de todos os usuários em uma organização ou de um usuário específico na organização.

### <a name="devices-and-apps--cloud-printing"></a>Dispositivos e aplicativos | Impressão na nuvem
- Especificar as [margens de impressão](/graph/api/resources/printmargin?view=graph-rest-beta) ao configurar um [documento para impressão](/graph/api/resources/printdocument?view=graph-rest-beta).
- Compatível com os seguintes [recursos da impressora](/graph/api/resources/printercapabilities?view=graph-rest-beta):
  - instruções de alimentação
  - impressão de intervalos de páginas
  - resolução da impressão em DPIs
  - tamanho máximo da fila de tarefas de impressão em bytes
  - compartimentos de entrada
  - margens
  - ordenação
  - escala do documento
- Compatível com a resolução da impressão (DPI) e com a escala do documento como parte das [configurações padrão da impressora](/graph/api/resources/printerdefaults?view=graph-rest-beta).
- Compatível com as seguintes [configurações do documento](/graph/api/resources/printerdocumentconfiguration?view=graph-rest-beta):
  - compartimentos de entrada
  - compartimentos de saída
  - tamanhos de papel
  - margens
  - tipos de papel
  - acabamentos como grampeamento ou encadernação
  - páginas por folha
  - layout multipáginas especificando a direção do layout das páginas na folha
  - ordenação
  - escala
- Expandir os documentos ao [listar as tarefas de impressão](/graph/api/printer-list-jobs?view=graph-rest-beta).
- [Registre uma impressora ]() e use o recurso [printerCreateOperation](/graph/api/resources/printercreateoperation?view=graph-rest-beta) para monitorar e verificar o registro da impressora.
- [Obtenha a operação de registro](/graph/api/printoperation-get?view=graph-rest-beta) da impressora de longa duração no usuário atual ou no locatário do aplicativo.
- Algumas propriedades e tipos de enumeração renomeados; confira os detalhes nas atualizações do log de alterações da impressão em nuvem do mês de [junho](changelog.md#june-2020).

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gerenciamento corporativo
Atualizações do Intune em [junho](changelog.md#june-2020) — em beta.

### <a name="education"></a>Educação
- Possibilidade de usar permissões delegadas `EduRoster.ReadBasic` para [obter](/graph/api/educationuser-get?view=graph-rest-beta) a ID de um(a) [professor(a)](/graph/api/resources/educationteacher?view=graph-rest-beta) ou [aluno(a)](/graph/api/resources/educationstudent?view=graph-rest-beta) em um programa de uma fonte externa, na forma de uma propriedade **externalId**.
- Use a propriedade **externalSource** para monitorar o valor `lms` se uma [organização](/graph/api/resources/educationorganization?view=graph-rest-beta) de ensino ou [aula](/graph/api/resources/educationclass?view=graph-rest-beta) forem criados a partir de um sistema de gerenciamento de aprendizagem (LMS).

### <a name="identity-and-access"></a>Identidade e acesso
- Os profissionais de TI podem usar os recursos do [conector](/graph/api/resources/connector?view=graph-rest-beta) que sejam agentes leves para se conectar ao [Proxy de Aplicativos do Azure AD](/azure/active-directory/manage-apps/what-is-application-proxy) e [publicar aplicativos web locais externamente](/graph/api/resources/onpremisespublishing?view=graph-rest-beta)para que os usuários remotos de suas organizações possam acessá-los de forma segura.
- Gerenciar uma [política de autenticação](/graph/api/resources/authenticationflowspolicy?view=graph-rest-beta) no nível de locatário para ativar ou desativar um [serviço autoatendimento de cadastramento](/graph/api/resources/selfservicesignupauthenticationflowconfiguration?view=graph-rest-beta) para usuários externos.
- [Provisionar uma conta de usuário sob demanda](/graph/api/synchronization-synchronizationjob-provision-on-demand?view=graph-rest-beta) e ser capaz de especificar quais objetos provisionar e quais regras de sincronização executar.

### <a name="search"></a>Busca
- Utilizar os aperfeiçoamentos de uma [propriedade](/graph/api/resources/property?view=graph-rest-beta) em um [esquema](/graph/api/resources/schema?view=graph-rest-beta): **isRefinable** para habilitar a filtragem dos resultados de busca e obter um controle mais refinado da experiência de busca, além de **aliases** e **rótulos** para maior relevância.
- Capacidade de especificar até 128 recursos de **propriedades** em um **esquema**.
- Use [get externalItem](/graph/api/externalitem-get?view=graph-rest-beta) para fins de diagnóstico.

### <a name="users"></a>Usuários
- Use a propriedade **userPurpose** em [mailboxSettings](/graph/api/resources/mailboxsettings?view=graph-rest-beta) para identificar e diferenciar uma caixa de correio para um único usuário de uma caixa de correio compartilhada e do equipamento de caixa de correio no Exchange Online. 
- Use as [configurações de usuário](/graph/api/resources/usersettings?view=graph-rest-beta) para [obter](/graph/api/regionalandlanguagesettings-get?view=graph-rest-beta) ou [atualizar](/graph/api/regionalandlanguagesettings-update?view=graph-rest-beta) [idiomas preferenciais e configurações regionais](/graph/api/resources/regionalandlanguagesettings?view=graph-rest-beta).
- As configurações de usuário são uma relação acessível por meio do [usuário](/graph/api/resources/user?view=graph-rest-beta) que permite uma experiência de usuário consistente em todos os aplicativos, bastando tocar no perfil de usuário do Azure AD para refletir as mesmas preferências do usuário. Veja [como as configurações de usuário diferem das configurações da caixa de correio](/graph/api/resources/user?view=graph-rest-beta#user-preferences-for-languages-and-regional-formats). 


## <a name="want-to-stay-in-the-loop"></a>Quer ficar por dentro?

Estas são algumas maneiras de se envolver:

- Existem cenários em que você gostaria que o Microsoft Graph oferecesse suporte? Sugira e vote em novos recursos no [Microsoft Graph User Voice](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).
    Alguns novos recursos são originados como solicitações populares da comunidade de desenvolvedores. A equipe do Microsoft Graph avalia regularmente as necessidades dos clientes e lança novos recursos na seguinte ordem:

    1. Estreia no status de visualização **_prévia_**. As atualizações da API REST relacionadas estão no ponto de extremidade beta (`https://graph.microsoft.com/beta`).  

    2. Promovido para o status de**_disponibilidade geral_ (GA)**, se um feedback suficiente indicar a viabilidade. Todas as atualizações da API REST relacionadas serão adicionadas ao ponto de extremidade do v 1.0 (`https://graph.microsoft.com/v1.0`). 
- Seja um membro ativo da comunidade do Microsoft Graph! [Participe](https://aka.ms/microsoftgraphcall) da chamada mensal à comunidade do Microsoft Graph.
- Inscreva-se no [programa para desenvolvedores do Microsoft 365](https://developer.microsoft.com/office/dev-program), ganhe uma assinatura gratuita do Microsoft 365 e comece a desenvolver!


## <a name="see-also"></a>Confira também
- Confira o [blog de desenvolvedores do Microsoft Graph](https://developer.microsoft.com/graph/blogs/) periodicamente para comunicados de lançamentos e recursos úteis.
- Navegue pelas informações das inclusões da API do Microsoft Graph e pelas atualizações de comportamento de API no [changelog](changelog.md).
- Encontre [destaques de versões anteriores](whats-new-earlier.md).
- Saiba mais sobre o [controle de versão, suporte e mudanças significativas de políticas do Microsoft Graph](versioning-and-support.md).

