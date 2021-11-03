---
title: Novidades do Microsoft Graph
description: O que há de novo no Microsoft Graph
author: angelgolfer-ms
ms.localizationpriority: high
ms.openlocfilehash: 22deb547eda4301d1b8bb3f2830516aa2e3be682
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60688637"
---
# <a name="whats-new-in-microsoft-graph"></a>Novidades do Microsoft Graph

Veja os destaques das novidades nos dois últimos meses do Microsoft Graph, [o que foi adicionado anteriormente](whats-new-earlier.md) e como você pode [compartilhar suas ideias](#want-to-stay-in-the-loop). Para obter uma lista detalhada de atualizações no nível da API, consulte o [registro de alterações da API](https://developer.microsoft.com/graph/changelog/). 

> [!IMPORTANT]
> Recursos, incluindo APIs e ferramentas, no status de _visualização_ podem mudar sem aviso prévio e alguns podem nunca ser promovidos ao status de disponibilidade geral (GA). Não utilize recursos de visualização em aplicativos de produção.


## <a name="october-2021-new-and-generally-available"></a>Outubro de 2021: novo e em disponibilidade geral

### <a name="cloud-communications--calls"></a>Comunicações na nuvem | Chamadas
- [Transferir](/graph/api/call-transfer) uma chamada ponto a ponto ativa.
- Transferir uma chamada em grupo para um determinado participante (beneficiário).

### <a name="cloud-communications--online-meetings"></a>Comunicações na nuvem | Reuniões online
Oferece suporte a vários números de chamada tarifada e de chamada gratuita para acesso telefônico ([audioconferência](/graph/api/resources/audioConferencing)) de uma [reunião online](/graph/api/resources/onlinemeeting).

<!-- Hold off until permissions are deployed
As part of [privacy management in Microsoft 365](/privacy/solutions/privacymanagement/privacy-management?view=o365-worldwide&preserve-view=true), subject rights request now debuts in both v1 and beta endpoints of Microsoft Graph. The [subject rights request API](/graph/api/resources/subjectrightsrequest) lets users make requests to review or manage their personal data in their organizations. It also lets organizations automate and scale managing these requests, helping them to meet industry regulations more efficiently.
-->

### <a name="education"></a>Educação
Oferece suporte a arquivos de [mídia](/graph/api/resources/educationMediaResource) ou outros [recursos genéricos externos](/graph/api/resources/educationExternalResource) como um [recurso de atribuição](/graph/api/resources/educationassignmentresource).

### <a name="identity-and-access--applications"></a>Identidade e acesso | Aplicativos
- Para direcionar a experiência de consentimento de um [aplicativo](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true), especifique os [recursos do que o aplicativo precisa para acessar](/graph/api/resources/requiredresourceaccess?view=graph-rest-beta&preserve-view=true), incluindo o conjunto de permissões delegadas do OAuth 2.0 e funções de aplicativo que o aplicativo exige.
- Limite o número de APIs necessárias a 50 e as permissões necessárias a 400 por aplicativo.

### <a name="identity-and-access--directory-management"></a>Identidade e acesso | Gerenciamento do diretório
- Defina os [atributos de extensão](/graph/api/resources/onpremisesextensionattributes) para um [dispositivo](/graph/api/resources/device) e gerencie-os no Azure Active Directory na [criação](/graph/api/device-post-devices) ou [atualização](/graph/api/device-update) do dispositivo.
- [Obtenha uma chave de recuperação do BitLocker](/graph/api/bitlockerrecoverykey-get) em nome do usuário conectado que é o proprietário do dispositivo ou em uma função adequada. Obter uma chave de recuperação gera um [log de auditoria](/azure/active-directory/reports-monitoring/concept-audit-logs), em paridade com a experiência do usuário final.

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
Especifique uma lista de usuários adicionais ou membros do grupo a serem notificados sobre o andamento da análise de acesso, na propriedade **additionalNotificationRecipients** de um [accessReviewScheduleDefinition](/graph/api/resources/accessreviewscheduledefinition?view=graph-rest-beta&preserve-view=true).

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e entrada
Especifique os dispositivos em uma [política de acesso condicional](/graph/api/resources/conditionalaccesspolicy), como parte das [condições](/graph/api/resources/conditionalAccessConditionSet) que regem quando a política se aplica.

### <a name="personal-contacts"></a>Contatos pessoais
Habilite o suporte para permissões delegadas (`Contacts.Read` ou `Contacts.ReadWrite`) para recursos de [profilePhoto](/graph/api/resources/profilephoto?view=graph-rest-beta&preserve-view=true) em contas Microsoft pessoais.

### <a name="teamwork"></a>Trabalho em equipe
- [Obtenha todas as mensagens de chat em todos os canais](/graph/api/channel-getallmessages) em uma [equipe](/graph/api/resources/team).
- [Obtenha todas mensagens de todos os chats](/graph/api/chats-getallmessages) em que um usuário participa, incluindo chats individuais, chats em grupo e chats de reunião.
- Confira os [modelos de licenciamento e pagamento](teams-licenses.md) que se aplicam às APIs do Microsoft Teams no Microsoft Graph.

### <a name="users"></a>Usuários
As licenças de usuário para serviços do Azure Active Directory (Azure AD) agora oferecem suporte a um carimbo de data/hora para quando o [estado da atribuição de licença](/graph/api/resources/licenseassignmentstate) é atualizado pela última vez. 

## <a name="october-2021-new-in-preview-only"></a>Outubro de 2021: novo apenas na pré-visualização

### <a name="applications"></a>Aplicativos
Use [credenciais de identidade federada](/graph/api/resources/federatedidentitycredential?view=graph-rest-beta&preserve-view=true) para gerenciar as credenciais de um aplicativo e permitir que os aplicativos de nuvem de uma organização acessem o Azure AD sem usar segredos e certificados.

### <a name="cloud-communications--calls"></a>Comunicações na nuvem | Chamadas
Identifique um [participante](/graph/api/resources/participantInfo?view=graph-rest-beta&preserve-view=true) da chamada, usando a propriedade **participantId** do tipo de recurso [participantInfo](/graph/api/resources/participantInfo?view=graph-rest-beta&preserve-view=true).

### <a name="cloud-communications--online-meetings"></a>Comunicações na nuvem | Reuniões online
Habilite o [registro de reunião](/graph/api/resources/meetingregistration?view=graph-rest-beta&preserve-view=true) e organize reuniões online como um [webinar](/office/get-started-with-teams-webinars-42f3f874-22dc-4289-b53f-bbc1a69013e3). Associe a reunião a uma página de registro e escolha inscrever todos ou apenas os membros da organização como [inscritos da reunião](/graph/api/resources/meetingregistrant?view=graph-rest-beta&preserve-view=true). 

### <a name="customer-booking"></a>Reserva de clientes
- Oferece suporte aos seguintes atributos para um [serviço de reserva](/graph/api/resources/bookingService?view=graph-rest-beta&preserve-view=true):
  - Habilite o envio de notificações por SMS aos clientes para os compromissos (propriedade **smsNotificationsEnabled**).
  - A URL que os clientes podem usar para acessar o serviço (propriedade **webUrl**).
- Reserve um [compromisso](/graph/api/resources/bookingappointment?view=graph-rest-beta&preserve-view=true) com um ou mais dos seguintes atributos:
  - Especifique o fuso horário do cliente (propriedade **customerTimeZone**).
  - Especifique a URL para um compromisso online (propriedade **joinWebUrl**).
  - Habilite as notificações por SMS para o cliente para o compromisso (propriedade **smsNotificationsEnabled**).
- Especifique um ou mais endereços e números de telefone para um [cliente](/graph/api/resources/bookingcustomer?view=graph-rest-beta&preserve-view=true).
- Especifique o fuso horário para um [membro da equipe](/graph/api/resources/bookingStaffMember?view=graph-rest-beta&preserve-view=true).

### <a name="devices-and-apps--cloud-pc"></a>Dispositivos e aplicativos | Cloud PC
[Liste](/graph/api/virtualendpoint-list-serviceplans?view=graph-rest-beta&preserve-view=true) os [planos de serviço do Windows 365](/graph/api/resources/cloudPcServicePlan?view=graph-rest-beta&preserve-view=true) que uma organização assina para seus PCs na nuvem. Em cada [tipo de plano de serviço](/graph/api/resources/cloudPcServicePlan?view=graph-rest-beta&preserve-view=true#cloudpcserviceplantype-values) (business ou enterprise), uma organização pode optar por assinar de uma variedade de configurações de plano que variam de acordo com atributos como vCPU, RAM e armazenamento.

### <a name="identity-and-access--directory-management"></a>Identidade e acesso | Gerenciamento do diretório
Especifique as [principais definições de configuração de credenciais](/graph/api/resources/keycredentialconfiguration?view=graph-rest-beta&preserve-view=true) que podem ser [configuradas para permitir restrições a um aplicativo ou entidade de serviço](/graph/api/resources/appmanagementconfiguration?view=graph-rest-beta&preserve-view=true).

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
Habilite as seguintes [configurações](/graph/api/resources/assignmentReviewSettings?view=graph-rest-beta&preserve-view=true) adicionais para revisar uma [política de atribuição de pacote de acesso](/graph/api/resources/accesspackageassignmentpolicy?view=graph-rest-beta&preserve-view=true):
- Comportamento padrão se a solicitação não for revisada em uma determinado período (propriedade **accessReviewTimeoutBehavior**).
- Exibir recomendações ao revisor (propriedade **isAccessRecommendationEnabled**).
- Exigir que o revisor forneça justificativa para a aprovação (propriedade **isApprovalJustificationRequired** ).

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e entrada
- Especifique se as configurações de [política de avaliação de acesso contínuo](/graph/api/resources/continuousAccessEvaluationPolicy?view=graph-rest-beta&preserve-view=true) devem ser ou foram migradas para a [política de acesso condicional](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta&preserve-view=true).
- Como parte de um [acesso condicional](/azure/active-directory/conditional-access/overview) do Azure Active Directory, use um novo controle de sessão, [continuousAccessEvaluationSessionControl](/graph/api/resources/continuousAccessEvaluationSessionControl?view=graph-rest-beta&preserve-view=true), para avaliar continuamente o acesso e tomar decisões de acesso. 

### <a name="search--index"></a>Pesquisa | Índice
- Especifique as [configurações](/graph/api/resources/externalconnectors-searchsettings?view=graph-rest-beta&preserve-view=true) para a experiência de pesquisa de conteúdo em uma [conexão externa](/graph/api/resources/externalconnectors-externalconnection?view=graph-rest-beta&preserve-view=true). Por exemplo, um [modelo de exibição](/graph/api/resources/externalconnectors-displaytemplate?view=graph-rest-beta&preserve-view=true) para resultados de pesquisa e uma [regra](/graph/api/resources/externalconnectors-propertyRule?view=graph-rest-beta&preserve-view=true) para selecionar o modelo de exibição.
- Relacionar um ou mais [grupos externos](/graph/api/resources/externalconnectors-externalgroup?view=graph-rest-beta&preserve-view=true) a uma [conexão externa](/graph/api/resources/externalconnectors-externalconnection?view=graph-rest-beta&preserve-view=true). Por exemplo, um grupo externo, como uma unidade de negócio ou uma equipe de trabalho, pode determinar as permissões para o conteúdo na fonte de dados representada pela conexão externa.
- Opcionalmente, pode especificar a ID de um aplicativo do Teams em uma [conexão externa](/graph/api/resources/externalconnectors-externalconnection?view=graph-rest-beta&preserve-view=true) na propriedade **connectorId**.

### <a name="users"></a>Usuários
[Valide uma senha](/graph/api/user-validatePassword?view=graph-rest-beta&preserve-view=true) em tempo real em relação à política de validação de senha de uma organização, conforme um usuário digita a senha. Obtenha [informações detalhadas da validação](/graph/api/resources/passwordValidationInformation?view=graph-rest-beta&preserve-view=true) de acordo com as regras da política.


## <a name="september-2021-new-and-generally-available"></a>Setembro de 2021: novo e disponível para o público em geral

### <a name="cloud-communications--calls"></a>Comunicações na nuvem | Chamadas
- Colocar um [participante](/graph/api/resources/participant) em espera e tocar música em segundo plano usando a ação [startHoldMusic](/graph/api/participant-startHoldMusic).
- Reincorporar um participante colocado em espera em uma chamada anteriormente usando a ação [stopHoldMusic](/graph/api/participant-stopHoldMusic).

### <a name="cloud-communications--online-meetings"></a>Comunicações na nuvem | Reuniões on-line
- Obtenha o fluxo de conteúdos de um relatório de participante de um [evento ao vivo do Teams](/microsoftteams/teams-live-events/what-are-teams-live-events).
- Obtenha ou defina a opção para gravar automaticamente uma [reunião online](/graph/api/resources/onlineMeeting).
- Use `OnlineMeetingArtifact.Read.All` como delegada ou permissão de aplicativo para ler artefatos de reuniões on-line. Para obter mais informações, consulte [permissões de reuniões on-line](permissions-reference.md#online-meetings-permissions).

### <a name="devices-and-apps--cloud-printing"></a>Dispositivos e aplicativos | Impressão na nuvem
O status da impressora em nuvem inclui todos os valores padrão [Internet Printing Protocol (IPP)](https://www.iana.org/assignments/ipp-registrations/ipp-registrations.xhtml).

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gerenciamento corporativo
Atualizações mensais do Intune para a versão v1.0. No [log de mudanças](https://developer.microsoft.com/graph/changelog), defina o filtro de **Data** para setembro de 2021 e procure uma seção com esse mesmo título.

### <a name="files"></a>Arquivos
- Obtenha os detalhes de qualquer vírus detectado em um [driveItem](/graph/api/resources/driveItem) por meio de uma propriedade de **malware**.
- Use a função [delta](/graph/api/driveitem-delta) para acompanhar as alterações não apenas no diretório raiz, mas também em outras pastas dentro de uma unidade.

### <a name="identity-and-access--directory-management"></a>Identidade e acesso | Gerenciamento do diretório
Os provedores de controle de acesso baseado em função (RBAC) podem [gerenciar funções](/graph/api/resources/rolemanagement) do Azure Active Directory, [definindo ações de funções](/graph/api/resources/unifiedroledefinition)que podem ser realizadas em recursos específicos e [atribuindo funções](/graph/api/resources/unifiedroleassignment) aos usuários com base em tais definições de função, fornecendo o acesso correspondente a esses recursos.

### <a name="search--query"></a>Pesquisa | Consulta
- Agregar resultados de pesquisa do tipo numérico ou cadeia de caracteres que são importados pelos [conectores do Microsoft Graph](/microsoftsearch/connectors-overview) e que estão configurados no [esquema](/graph/api/resources/schema) para serem refináveis. Veja mais informações sobre [como refinar resultados de pesquisa usando agregações](search-concept-aggregation.md).
- [Classifique](/graph/api/resources/search-api-overview#sort-search-results) os resultados de pesquisa do OneDrive e do SharePoint em qualquer propriedade classificável. Para obter mais informações, consulte [Uso da API de Pesquisa da Microsoft para classificar resultados da pesquisa](search-concept-sort.md).

### <a name="teamwork"></a>Trabalho em equipe
Usar uma única ação [provisionEmail](/graph/api/channel-provisionemail) para obter o endereço de email de um [canal](/graph/api/resources/channel), se houver, ou criar um, se não houver. Usar a ação [removeEmail](/graph/api/channel-removeemail) para remover o endereço de email.

### <a name="workbooks-and-charts"></a>Pastas de trabalho e gráficos
Criar linhas de tabela de forma assíncrona. Para um melhor desempenho, uma boa prática para criar várias linhas de tabela é agrupá-las em uma operação do tipo [criar tableRow](/graph/api/table-post-rows) e realizar a operação de forma assíncrona. Prossiga com a operação [GET workbookOperation](/graph/api/workbookoperation-get) e a função [tableRowOperationResult](/graph/api/workbook-tableRowOperationResult) para obter o novo recurso [workbookTableRow](/graph/api/resources/workbooktablerow).


## <a name="september-2021-new-in-preview-only"></a>Setembro de 2021: novos somente em versão prévia

### <a name="applications"></a>Aplicativos
Os aplicativos que usam fluxos de logon único do Security Assertion Markup Language (SAML) podem especificar um URI de redirecionamento padrão (propriedade **defaultRedirectUri** do [aplicativo](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true)) ou identificar um URI de redirecionamento específico no qual os usuários são enviados para fazer logon (propriedade **redirectUriSettings** do [webApplication](/graph/api/resources/webapplication?view=graph-rest-beta&preserve-view=true)). 

### <a name="cloud-communications--online-meetings"></a>Comunicações na nuvem | Reuniões on-line
Obter o número total de participantes em um [relatório de presença de reunião](/graph/api/resources/meetingattendancereport?view=graph-rest-beta&preserve-view=true) de uma [reunião on-line](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true).

### <a name="compliance--ediscovery"></a>Conformidade | Descoberta eletrônica
A operação [criar caso](/graph/api/ediscovery-case-post?view=graph-rest-beta&preserve-view=true) sempre cria casos em formato grande. Isso expande o limite do tamanho de caso para acomodar um volume total de dados e um número total de itens mais altos. Para obter mais detalhes, consulte [vantagens de casos grandes](/microsoft-365/compliance/advanced-ediscovery-large-cases?view=o365-worldwide&preserve-view=true#benefits-of-large-cases).

### <a name="devices-and-apps--cloud-pc"></a>Dispositivos e aplicativos | Computador na nuvem
- [Reprovisionar um computador na nuvem](/graph/api/manageddevice-reprovisioncloudpc?view=graph-rest-beta&preserve-view=true) como uma área de trabalho virtual gerenciada na nuvem registrada no Intune.
- [Redimensionar um computador na nuvem](/graph/api/manageddevice-resizecloudpc?view=graph-rest-beta&preserve-view=true) atualizando-o ou rebaixando-o para outra configuração com uma CPU virtual (vCPU) e um tamanho de armazenamento novos.
- [Configurar](/graph/api/virtualendpoint-post-onpremisesconnections?view=graph-rest-beta&preserve-view=true), [listar](/graph/api/virtualendpoint-list-onpremisesconnections?view=graph-rest-beta&preserve-view=true) e [executar verificações de integridade](/graph/api/cloudpconpremisesconnection-runhealthcheck?view=graph-rest-beta&preserve-view=true) em [conexões de rede locais](/graph/api/resources/cloudpconpremisesconnection?view=graph-rest-beta&preserve-view=true) para provisionar PCs na nuvem.

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gerenciamento corporativo
Atualizações mensais do Intune para a versão beta. No [log de mudanças](https://developer.microsoft.com/graph/changelog), defina o filtro de **Data** para setembro de 2021 e procure uma seção com esse mesmo título.

### <a name="education"></a>Educação
- Permitir que os professores [reatribuam](/graph/api/educationsubmission-reassign?view=graph-rest-beta&preserve-view=true) o [envio](/graph/api/resources/educationsubmission?view=graph-rest-beta&preserve-view=true) de uma tarefa ao aluno com comentários para revisão.
- Suporte para adicionar tarefas apenas aos calendários dos alunos se você usar o cabeçalho de solicitação `Prefer: include-unknown-enum-members` para operações nos recursos [educationAssignment](/graph/api/resources/educationassignment?view=graph-rest-beta&preserve-view=true) ou [educationAssignmentDefaults](/graph/api/resources/educationassignmentdefaults?view=graph-rest-beta&preserve-view=true).

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
[Excluir](/graph/api/accesspackageassignmentrequest-delete?view=graph-rest-beta&preserve-view=true) um [accessPackageAssignmentRequest](/graph/api/resources/accesspackageassignmentrequest?view=graph-rest-beta&preserve-view=true) para remover uma solicitação negada ou concluída.

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e login
- Permitir que os usuários executem a autenticação multifatorial usando um [token de software OATH](/graph/api/resources/softwareOathAuthenticationMethod?view=graph-rest-beta&preserve-view=true). Um token de software OATH é um gerador de números baseado em software que usa a Senha de Uso Único Baseada em Tempo (TOTP) padrão OATH.
- Identifique se a correspondência de números está habilitada ou desabilitada para autenticação multifator pela política no Azure AD, usando a propriedade **numberMatchingRequiredState** do [microsoftAuthenticatorAuthenticationMethodTarget](/graph/api/resources/microsoftAuthenticatorAuthenticationMethodTarget?view=graph-rest-beta&preserve-view=true).
- Identifique se um contexto adicional do usuário deve ser mostrado na notificação do aplicativo autenticador, usando a propriedade **displayAppInformationRequiredState** do [microsoftAuthenticatorAuthenticationMethodTarget](/graph/api/resources/microsoftAuthenticatorAuthenticationMethodTarget?view=graph-rest-beta&preserve-view=true).
- Use o [fluxo de usuário B2C](/graph/api/resources/b2cidentityuserflow?view=graph-rest-beta&preserve-view=true) e o [fluxo de usuário de inscrição de autoatendimento](/graph/api/resources/b2xidentityuserflow?view=graph-rest-beta&preserve-view=true) em favor da API de [fluxo de usuário](/graph/api/resources/identityuserflow?view=graph-rest-beta&preserve-view=true) anterior, que foi preterida.

### <a name="security--attack-simulation-and-training"></a>Segurança | Treinamento e simulação de ataque
O lançamento da API para [treinamento e simulação de ataque](/microsoft-365/security/office-365-security/attack-simulation-training?view=o365-worldwide&preserve-view=true), que é um serviço disponível como parte do [Microsoft Defender para Office 365](/microsoft-365/security/office-365-security/defender-for-office-365?view=o365-worldwide&preserve-view=true). A API permite que os administradores de locatários [listem os exercícios e treinamentos de simulação lançados](/graph/api/attacksimulationroot-list-simulations?view=graph-rest-beta&preserve-view=true) e obtenham [relatórios](/graph/api/resources/report-m365defender-reports-overview?view=graph-rest-beta&preserve-view=true) sobre os insights derivados dos comportamentos online dos usuários nas simulações de phishing.

## <a name="want-to-stay-in-the-loop"></a>Quer ficar por dentro?

Estas são algumas maneiras de se envolver:

- Existem cenários em que você gostaria que o Microsoft Graph oferecesse suporte? Sugira e vote nos novos recursos na [Comunidade Microsoft Tech](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph).
    Alguns novos recursos são originados como solicitações populares da comunidade de desenvolvedores. A equipe do Microsoft Graph avalia regularmente as necessidades dos clientes e lança novos recursos na seguinte ordem:

    1. Estreia no status de **_visualização_**. Todas as atualizações da API REST relacionadas estão no ponto de extremidade beta (`https://graph.microsoft.com/beta`).  

    2. Promovido para o status de **_disponibilidade geral_ (GA)**, se um feedback suficiente indicar a viabilidade. Todas as atualizações da API REST relacionadas serão adicionadas ao ponto de extremidade do v 1.0 (`https://graph.microsoft.com/v1.0`). 
- Seja um membro ativo da comunidade do Microsoft Graph! [Participe](https://aka.ms/microsoftgraphcall) da chamada mensal à comunidade do Microsoft Graph.
- Inscreva-se no [programa para desenvolvedores do Microsoft 365](https://developer.microsoft.com/office/dev-program), ganhe uma assinatura gratuita do Microsoft 365 e comece a desenvolver!


## <a name="see-also"></a>Confira também
- Confira o [blog de desenvolvedores do Microsoft Graph](https://developer.microsoft.com/graph/blogs/) periodicamente para comunicados de lançamentos e recursos úteis.
- Navegue pelas informações das inclusões da API do Microsoft Graph e pelas atualizações de comportamento de API no [changelog](https://developer.microsoft.com/graph/changelog/).
- Encontre [destaques de versões anteriores](whats-new-earlier.md).
- Saiba mais sobre o [controle de versão, suporte e mudanças significativas de políticas do Microsoft Graph](versioning-and-support.md).
