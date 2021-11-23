---
title: Novidades do Microsoft Graph
description: O que há de novo no Microsoft Graph
author: angelgolfer-ms
ms.localizationpriority: high
ms.openlocfilehash: 37f80e951ea71d5847e0c793053c3a1bc9cd42dc
ms.sourcegitcommit: c6bbba6cb9aaa7ad35374d1b5d4466c49878ab43
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/22/2021
ms.locfileid: "61135169"
---
# <a name="whats-new-in-microsoft-graph"></a>Novidades do Microsoft Graph

Veja os destaques das novidades nos dois últimos meses do Microsoft Graph, [o que foi adicionado anteriormente](whats-new-earlier.md) e como você pode [compartilhar suas ideias](#want-to-stay-in-the-loop). Para obter uma lista detalhada de atualizações no nível da API, consulte o [registro de alterações da API](https://developer.microsoft.com/graph/changelog/). 

> [!IMPORTANT]
> Recursos, incluindo APIs e ferramentas, no status de _visualização_ podem mudar sem aviso prévio e alguns podem nunca ser promovidos ao status de disponibilidade geral (GA). Não utilize recursos de visualização em aplicativos de produção.


## <a name="november-2021-new-and-generally-available"></a>Novembro de 2021: Novo e geralmente disponível ao público

### <a name="files"></a>Arquivos
Obtenha o estado de uma unidade a partir de um horário específico especificando o carimbo de data/hora codificado no URL correspondente. Veja um [exemplo](/graph/api/driveitem-delta#example-4-retrieving-delta-results-using-a-timestamp).

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e login
- Execute [campanhas](/graph/api/resources/authenticationMethodsRegistrationCampaign) e [imponha os usuários a se registrarem](/graph/api/resources/registrationEnforcement) no momento da entrada para configurar os métodos de autenticação direcionados.
-  Configurar um [provedor de identidade Apple](/graph/api/resources/applemanagedidentityprovider) em um locatário do Azure AD B2C.

## <a name="november-2021-new-in-preview-only"></a>Novembro de 2021: Novo somente na pré-visualização

### <a name="cloud-communications--online-meeting"></a>Comunicações na nuvem | Reunião online
Admita automaticamente novos tipos de participantes em uma reunião online e ignore o lobby da reunião:
- Somente pessoas convidadas pelo organizador.
- Somente os participantes da mesma empresa.

### <a name="devices-and-apps--cloud-pc"></a>Dispositivos e aplicativos | Computador na nuvem
- Defina uma [configuração](/graph/api/resources/cloudPcDomainJoinConfiguration?view=graph-rest-beta&preserve-view=true) de como um dispositivo de PC na nuvem provisionado pode ingressar no Azure Active Directory (Microsoft Azure AD): somente nuvem e ingressar somente no Microsoft Azure AD, ou híbrido e ingressar no Active Directory local e no Microsoft Azure AD.
- Obtenha o [recurso de imagem da galeria](/graph/api/resources/cloudPcGalleryImage?view=graph-rest-beta&preserve-view=true) da organização atual que pode ser usado para provisionar um PC na nuvem.

### <a name="devices-and-apps--device-updates"></a>Dispositivos e aplicativos | Atualizações do dispositivo
- Use as [configurações de salvaguarda](/graph/api/resources/windowsupdates-safeguardSettings?view=graph-rest-beta&preserve-view=true) para recusar as proteções contra prováveis problemas em uma implantação.
- Suporte para um [estado de implantação](/graph/api/resources/windowsupdates-deploymentState?view=graph-rest-beta&preserve-view=true) em que uma implantação está com defeito devido ao conteúdo não ser mais implantável, por exemplo, no fim do serviço.

### <a name="identity-and-access--directory-management"></a>Identidade e acesso | Gerenciamento do diretório
- Defina e atribua [atributos de segurança personalizado ](/graph/api/resources/custom-security-attributes-overview?view=graph-rest-beta&preserve-view=true) aos objetos do Microsoft Azure AD. Use esses atributos para armazenar informações, categorizar objetos ou impor um controle de acesso refinado sobre recursos específicos do Azure. Use esses atributos com o [Controle de acesso baseado em atributo do Azure](/azure/role-based-access-control/conditions-overview) (Azure ABAC).
- [Crie um grupo dentro de uma unidade administrativa](/graph/api/administrativeunit-post-members?view=graph-rest-beta&preserve-view=true).

### <a name="reports--microsoft-365-usage-reports"></a>Relatórios | Relatórios de uso do Microsoft 365
[Os relatórios de uso do Microsoft 365](/graph/api/resources/report?view=graph-rest-beta&preserve-view=true) no tipo de saída JSON não são mais fortemente tipados e são do tipo `Edm.Stream`. Para obter mais informações, consulte [Alterações da propriedade OData na API de relatórios de uso do Microsoft 365 no Microsoft Graph](https://devblogs.microsoft.com/microsoft365dev/odata-property-changes-to-microsoft-365-usage-reports-api-in-microsoft-graph/).

### <a name="teamwork"></a>Trabalho em equipe
Marque um chat como [lido](/graph/api/chat-markChatReadForUser?view=graph-rest-beta&preserve-view=true) ou [não lido](/graph/api/chat-markchatunreadforuser?view=graph-rest-beta&preserve-view=true) para um usuário.

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
Suporta um arquivo de [mídia](/graph/api/resources/educationMediaResource) ou algum outro [recurso genérico externo](/graph/api/resources/educationExternalResource) como um [recurso de atribuição](/graph/api/resources/educationassignmentresource).

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
As licenças de usuário dos serviços Azure Active Directory (Azure AD) agora suportam um data/hora para quando o [estado da atribuição de licença](/graph/api/resources/licenseassignmentstate) for atualizado pela última vez. 

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
[Valide uma senha](/graph/api/user-validatePassword?view=graph-rest-beta&preserve-view=true) em tempo real em relação à política de validação de senha de uma organização, à medida que um usuário digita a senha. Obtenha [informações detalhadas da validação](/graph/api/resources/passwordValidationInformation?view=graph-rest-beta&preserve-view=true) de acordo com as regras da política.



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
