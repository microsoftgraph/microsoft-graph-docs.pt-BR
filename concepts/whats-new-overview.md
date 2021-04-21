---
title: Novidades do Microsoft Graph
description: O que há de novo no Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: e5e8e8ba5c67e81abe9bf108be5f72bacfe2739f
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921928"
---
# <a name="whats-new-in-microsoft-graph"></a>Novidades do Microsoft Graph

Veja os destaques das novidades nos dois últimos meses do Microsoft Graph, [o que foi adicionado anteriormente](whats-new-earlier.md) e como você pode [compartilhar suas ideias](#want-to-stay-in-the-loop). Para obter uma lista detalhada de atualizações no nível da API, consulte o [registro de alterações da API](https://developer.microsoft.com/graph/changelog/). 

> [!IMPORTANT]
> Os recursos, incluindo APIs e ferramentas, no status de _visualização_, podem ser alterados sem aviso prévio e alguns talvez nunca sejam promovidos ao status DG. Não use os recursos de visualização em aplicativos de produção.

## <a name="april-2021-new-and-generally-available"></a>Abril de 2021: novo e disponível para o público geral

### <a name="teamwork"></a>Trabalho em equipe
- Identifique o canal pela propriedade **channelIdentity**, se uma [chatMessage](/graph/api/resources/chatmessage) estiver em um [canal](/graph/api/resources/channel).
- Identifique o chat pela propriedade **chatId**, se o **[chatMessage](/graph/api/resources/chatmessage)** estiver em um [chat](/graph/api/resources/chat).
- Use o relacionamento de **mensagens** para obter todos os recursos [chatMessage](/graph/api/resources/chatmessage) em um [chat](/graph/api/resources/chat).

## <a name="april-2021-new-in-preview-only"></a>Abril de 2021: Novo somente para visualização

### <a name="teamwork"></a>Trabalho em equipe
Use a [concessão de permissão específica do recurso](/graph/api/resources/resourcespecificpermissiongrant?view=graph-rest-beta&preserve-view=true) para listar os aplicativos com acesso a um determinado [grupo](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) ou [chat](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true).

## <a name="march-2021-new-and-generally-available"></a>Março de 2021: novo e disponível para o público geral

### <a name="applications"></a>Aplicativos
- GA do recurso [applicationTemplate](/graph/api/resources/applicationtemplate) que suporta a [listagem](/graph/api/applicationtemplate-list) de aplicativos na galeria de aplicativos do Azure AD e a [adição](/graph/api/applicationtemplate-instantiate) de uma instância desse aplicativo a um diretório.
- Use a permissão somente para aplicativo `Application.ReadWrite.OwnedBy`ao[adicionar](/graph/api/applicationtemplate-instantiate) tal instância.
- Use a propriedade **signInAudience** do [servicePrincipal](/graph/api/resources/serviceprincipal) para obter as contas de usuário compatíveis com o aplicativo atual.

### <a name="devices-and-apps--cloud-printing"></a>Dispositivos e aplicativos | Impressão na nuvem
- GA da [API de impressão em nuvem](universal-print-concept-overview.md) para Impressão Universal! Veja o [comunicado](https://techcommunity.microsoft.com/t5/windows-it-pro-blog/universal-print-is-ready-for-business/ba-p/2176778) e confira como [começar com a Impressão Universal](/universal-print/fundamentals/universal-print-license).
- [Inscreva-se para alterar as notificações](universal-print-webhook-notifications.md) em uma [definição de tarefa de impressão](/graph/api/resources/printtaskdefinition) ou recurso [impressora](/graph/api/resources/printer).

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
- Use as [solicitações de consentimento](/graph/api/resources/consentrequests-root) do Azure Active Directory (Azure AD) para gerenciar o fluxo de trabalho da solicitação para usuários que tentam acessar aplicativos que exigem aprovação de administrador. A API usa os seguintes recursos:
  - O recurso [adminConsentRequestPolicy](/graph/api/resources/adminconsentrequestpolicy) para criar e gerenciar solicitações de acesso ao aplicativo para a organização.
  - O recurso [appConsentRequest](/graph/api/resources/appconsentrequest) para agregar e gerenciar solicitações de usuário para acessar um aplicativo específico.
  - O recurso [userConsentRequest](/graph/api/resources/userConsentRequest) para usuários que solicitam acesso a um aplicativo que requer autorização de administrador. 
  - O recurso [accessReviewReviewerScope](/graph/api/resources/accessReviewReviewerScope)define quem é indicado em **adminConsentRequestPolicy** para revisar os objetos **appConsentRequest** e **userConsentRequest**.
  - O recurso de [aprovação](/graph/api/resources/approval) representa uma decisão de aprovação para uma solicitação.
- GA da API de Termos de Uso que oferece suporte a um [contrato de Termos de Uso](/graph/api/resources/agreement) personalizável de um locatário no Azure AD.

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e login
- GA dos [métodos de autenticação](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta&preserve-view=true), incluindo as [chaves de segurança FIDO2](/graph/api/resources/fido2authenticationmethod),o [aplicativo Microsoft Authenticator](/graph/api/resources/microsoftauthenticatorauthenticationmethod) e o [Windows Hello para Empresas](/graph/api/resources/windowshelloforbusinessauthenticationmethod).
- GA das [políticas de método de autenticação](/graph/api/resources/authenticationmethodspolicies-overview) que definem os métodos de autenticação e os usuários que têm permissão para usá-los para se conectar e executar a autenticação multifator (MFA) no Azure AD. As políticas de métodos de autenticação que podem ser gerenciadas no Microsoft Graph incluem as [chaves de segurança FIDO2](/graph/api/resources/fido2authenticationmethodconfiguration), a Entrada por Telefone sem Senha com o [aplicativo Microsoft Authenticator](/graph/api/resources/microsoftauthenticatorauthenticationmethodconfiguration) e a [política de métodos de autenticação OTP de email](/graph/api/resources/emailauthenticationmethodconfiguration) do locatário.
- GA da [política de distribuição de recursos](/graph/api/resources/featureRolloutPolicy) que ajuda os administradores de locatários a ter recursos piloto para grupos específicos antes de habilitá-los para toda a organização.
- GA das [propriedades de identidade visual da organização](/graph/api/resources/organizationalbrandingproperties) que permite uma aparência personalizada das telas de entrada do Azure Active Directory. As organizações podem personalizar com base na localidade para usuários específicos.

### <a name="tasks-and-plans"></a>Tarefas e planos
- Use a permissão delegada de `Tasks.Read` para ler as operações de todos os recursos do Planner.
- Use a permissão delegada de `Tasks.ReadWrite` para ler e gravar as operações de todos os recursos do Planner.

### <a name="teamwork"></a>Trabalho em equipe
- GA de operações de [chat](/graph/api/resources/chat), chat [conversationMember](/graph/api/resources/conversationmember), [aplicativo](/graph/api/resources/teamsappinstallation) de chat, [guia](/graph/api/resources/teamstab) de chat e os seus métodos.
- GA de mais algumas propriedades de [teamsAppDefinition](/graph/api/resources/teamsAppDefinition), que representam detalhes de uma versão de um aplicativo no catálogo de aplicativos do Microsoft Teams, incluindo o seguinte:
  - **createdBy**, **description**, **shortDescription**, **lastModifiedDateTime**
  - **publishingState**, que pode ser `submitted` e em revisão, `published` ou `rejected` pelo administrador
  - Relação de **bot** do tipo [teamworkBot](/graph/api/resources/teamworkbot), representando os detalhes do bot especificado no manifesto do aplicativo Teams.
- Use a API de notificações de feed de atividades para envolver melhor os usuários em três contextos:
  - [Enviar notificação ao usuário em um chat](/graph/api/chat-sendactivitynotification)
  - [Enviar notificação ao usuário em uma equipe](/graph/api/team-sendactivitynotification)
  - [Enviar notificação ao usuário](/graph/api/userteamwork-sendactivitynotification)
- Migre o histórico de mensagens e dados dos usuários de um sistema externo para um canal do Teams, permitindo que os usuários continuem as suas comunicações facilmente. Use os seguintes métodos que oferecem suporte para o cenário de migração:
  - [Criar equipe](/graph/api/team-post)
  - [Criar canal](/graph/api/channel-post)
  - [Criar chatMessage em um canal](/graph/api/channel-post-messages)
  - [Responder a uma mensagem em um canal](/graph/api/channel-post-messagereply)
  - [Concluir a migração de mensagens em uma equipe](/graph/api/team-completemigration)
  - [Concluir a migração de mensagens em um canal](/graph/api/channel-completemigration)
- [Liste](/graph/api/chatmessage-list-chatmessagehostedcontents) ou [obtenha](/graph/api/chatmessagehostedcontent-get) conteúdo avançado hospedado em uma [chatMessage](/graph/api/resources/chatmessage), como imagens ou trechos de código.
- Suporte de permissões delegadas de `ChannelMessage.Read.All` para subscrever notificações de mudança em recursos [chatMessage](/graph/api/resources/chatmessage).

## <a name="march-2021-new-in-preview-only"></a>Março de 2021: Novo somente para visualização

### <a name="applications"></a>Aplicativos
[Crie e adicione certificados autoassinados](/graph/api/servicePrincipal-addTokenSigningCertificate?view=graph-rest-beta&preserve-view=true) aos seus aplicativos SAML. Use isso para ajudar a habilitar o logon único para aplicativos da galeria do Azure AD em seu locatário, permitindo que o Azure AD assine as respostas com o SAML.

### <a name="devices-and-apps--cloud-pc"></a>Dispositivos e aplicativos | Computador na nuvem
Adicionados ao recurso [cloudPcDeviceImage](/graph/api/resources/cloudpcdeviceimage?view=graph-rest-beta&preserve-view=true) mais dois motivos para falha no upload de uma imagem de origem do dispositivo: sistema operacional não compatível (`osVersionNotSupported`) ou uma imagem de origem inválida para provisionar uma VM do Windows (`sourceImageInvalid`).

### <a name="devices-and-apps--cloud-printing"></a>Dispositivos e aplicativos | Impressão na nuvem
Obtenha a data/hora mais recente (propriedade **lastSeenDateTime**) em que uma impressora interagiu com a Impressão Universal.

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gerenciamento corporativo
As atualizações de [março](https://developer.microsoft.com/graph/changelog/?from=2021-03-01&to=2021-03-31&filterBy=Corporate%20management) do Intune para a versão beta.

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
Aplique o novo modelo de [revisões de acesso](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) a associações de grupo e todos os outros tipos de recursos suportados. Substitua o [modelo legado de revisões de acesso](/graph/api/resources/accessreviews-root?view=graph-rest-beta&preserve-view=true).

### <a name="sites-and-lists"></a>Sites e listas
- Suporta um tipo ou modelo de conteúdo específico para documentos ou conjuntos de documentos em conjuntos de sites específicos, por meio de um conjunto de novas propriedades e métodos na entidade [contentType](/graph/api/resources/contentType?view=graph-rest-beta&preserve-view=true). Os métodos incluem o seguinte:
  - [addCopy](/graph/api/contenttype-addcopy?view=graph-rest-beta&preserve-view=true)
  - [associateWithHubSites](/graph/api/contenttype-associatewithhubsites?view=graph-rest-beta&preserve-view=true)
  - [copyToDefaultContentLocation](/graph/api/contenttype-copytodefaultcontentlocation?view=graph-rest-beta&preserve-view=true)
  - [isPublished](/graph/api/contenttype-ispublished?view=graph-rest-beta&preserve-view=true)
  - [publish](/graph/api/contenttype-publish?view=graph-rest-beta&preserve-view=true)
  - [unpublish](/graph/api/contenttype-unpublish?view=graph-rest-beta&preserve-view=true)
- Personalize os tipos de conteúdo de acordo com as colunas. As colunas são representadas pela entidade [columnDefinition](/graph/api/resources/columndefinition?view=graph-rest-beta&preserve-view=true) e suportam o conjunto completo de operações CRUD.
- [Obtenha os tipos de conteúdo de um site que podem ser aplicados a uma lista](/graph/api/site-getApplicableContentTypesForList?view=graph-rest-beta&preserve-view=true).
- Diferencie os tipos de coluna pelas seguintes propriedades na entidade **columnDefinition**: booliana, calculada, escolha, moeda, dateTime, pesquisa, número, personOrGroup, texto. Essas categorias são mutuamente exclusivas.

### <a name="sites-and-lists--taxonomy"></a>Sites e listas | Taxonomia
- Navegue de um [site](/graph/api/resources/site?view=graph-rest-beta&preserve-view=true) para um [repositório de termos de taxonomia](/graph/api/resources/termstore-store?view=graph-rest-beta&preserve-view=true) usando a relação **termStore**.
- Na direção inversa, obtenha a ID do site pai de um repositório de termos usando a propriedade **parentSiteId**.

### <a name="users"></a>Usuários
- [Obtenha](/graph/api/regionalandlanguagesettings-get?view=graph-rest-beta&preserve-view=true) ou [atualize](/graph/api/regionalandlanguagesettings-update?view=graph-rest-beta&preserve-view=true) as [preferências de um usuário para traduzir idiomas](/graph/api/resources/translationpreferences?view=graph-rest-beta&preserve-view=true). Por exemplo, se deve ou não traduzir, traduzir automaticamente ou solicitar antes de traduzir idiomas específicos em mensagens, chats e páginas da Web e qualquer [substituição de tradução](/graph/api/resources/translationlanguageoverride?view=graph-rest-beta&preserve-view=true).
- [Ative um plano de serviço](/graph/api/user-activateServicePlan?view=graph-rest-beta&preserve-view=true) para um usuário.

## <a name="want-to-stay-in-the-loop"></a>Quer ficar por dentro?

Estas são algumas maneiras de se envolver:

- Existem cenários em que você gostaria que o Microsoft Graph oferecesse suporte? Sugira e vote em novos recursos no [Microsoft Tech Community](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph).
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