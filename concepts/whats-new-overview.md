---
title: Novidades do Microsoft Graph
description: O que há de novo no Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 6104775b7e5f73785f013c55f3bbc07352ec02b0
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2021
ms.locfileid: "52645329"
---
# <a name="whats-new-in-microsoft-graph"></a>Novidades do Microsoft Graph

Veja os destaques das novidades nos dois últimos meses do Microsoft Graph, [o que foi adicionado anteriormente](whats-new-earlier.md) e como você pode [compartilhar suas ideias](#want-to-stay-in-the-loop). Para obter uma lista detalhada de atualizações no nível da API, consulte o [registro de alterações da API](https://developer.microsoft.com/graph/changelog/). 

> [!IMPORTANT]
> Recursos, incluindo APIs e ferramentas, no status de _visualização_ podem mudar sem aviso prévio e alguns podem nunca ser promovidos ao status de disponibilidade geral (GA). Não utilize recursos de visualização em aplicativos de produção.

## <a name="may-2021-new-and-generally-available"></a>Maio de 2021: Novo e disponível para o público geral

### <a name="devices-and-apps--cloud-printing"></a>Dispositivos e aplicativos | Impressão na nuvem
Descubra quando uma impressora interagiu pela última vez com a Impressão Universal, usando a propriedade **lastSeenDateTime** da [impressora](/graph/api/resources/printer).

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e login
Obtenha ou atualize a função de um usuário convidado usando a propriedade **guestUserRoleId** de [AuthorPolicy](/graph/api/resources/authorizationpolicy).

### <a name="mail"></a>Email
- [Crie rascunhos e envie mensagens do Outlook no formato MIME](outlook-send-mime-message.md), anexe assinaturas digitais S/MIME e criptografe o conteúdo da mensagem em S/MIME.
- Criar um [mailFolder](/graph/api/resources/mailfolder) como uma [pasta oculta](/graph/api/resources/mailfolder#hidden-mail-folders) ao [configurar a propriedade isHidden](/graph/api/user-post-mailfolders#example).

### <a name="microsoft-graph-toolkit"></a>Kit de ferramentas do Microsoft Graph
Experimente os seguintes novos recursos do Kit de Ferramentas do Microsoft Graph 2.2:
- Componentes de[arquivos](/graph/toolkit/components/file) e [lista de arquivos](/graph/toolkit/components/file-list)
- [Provedor de autenticação MSAL 2.0](/graph/toolkit/providers/msal2)
- [Biblioteca da Estrutura do SharePoint](/graph/toolkit/get-started/mgt-spfx)

### <a name="reports--azure-ad-activity-reports"></a>Relatórios | Relatórios de atividade do Microsoft Azure AD
GA da API de relatório para [listar](/graph/api/provisioningobjectsummary-list) as ações realizadas pelo serviço de provisionamento do Microsoft Azure AD e suas propriedades associadas. Alinhou a versão beta anterior à versão v1.0 da API.

## <a name="may-2021-new-in-preview-only"></a>Maio de 2021: Novo somente para visualização

### <a name="connecting-external-content"></a>Conectando conteúdo externo
- Esteja ciente dos [limites operacionais e à implementação](connecting-external-content-api-limits.md) durante a criação de conectores.
- Experimente a [API de conectores com o Postman](connecting-external-content-connectors-api-postman.md).

### <a name="devices-and-apps--cloud-pc"></a>Dispositivos e aplicativos | Computador na nuvem
Solicite as permissões de aplicativos com menos privilégios, `CloudPC.Read.All` ou `CloudPC.ReadWrite.All`, para acessar os métodos dos seguintes recursos:
  - Operações de leitura e gravação, e do método de [reprovision](/graph/api/cloudpc-reprovision?view=graph-rest-beta&preserve-view=true) de [cloudPC](/graph/api/resources/cloudpc?view=graph-rest-beta&preserve-view=true).
  - Operações de leitura e gravação, e do método [getSourceImages](/graph/api/cloudpcdeviceimage-getsourceimages?view=graph-rest-beta&preserve-view=true) de [cloudPcDeviceImage](/graph/api/resources/cloudpcdeviceimage?view=graph-rest-beta&preserve-view=true).
  - Operações de leitura e gravação, e do método [updateAdDomainPassword](/graph/api/cloudpconpremisesconnection-updateaddomainpassword?view=graph-rest-beta&preserve-view=true) de [cloudPcOnPremisesConnection](/graph/api/resources/cloudpconpremisesconnection?view=graph-rest-beta&preserve-view=true).
  - Operações de leitura e gravação, e do método [assign](/graph/api/cloudpcprovisioningpolicy-assign?view=graph-rest-beta&preserve-view=true) de [cloudPcProvisioningPolicy](/graph/api/resources/cloudpcprovisioningpolicy?view=graph-rest-beta&preserve-view=true).

### <a name="education"></a>Educação
- [Configurar uma pasta de recursos do SharePoint](/graph/api/educationAssignment-setupresourcesfolder?view=graph-rest-beta&preserve-view=true) carregar e armazenar todos os recursos baseados em arquivo no mesmo local para um [educationAssignment](/graph/api/resources/educationAssignment?view=graph-rest-beta&preserve-view=true).
- [Configurar uma pasta de recursos do SharePoint](/graph/api/educationsubmission-setupresourcesfolder?view=graph-rest-beta&preserve-view=true) para carregar e armazenar todos os recursos baseados em arquivo como um arquivo Word e Excel no mesmo local para um [educationAssignment](/graph/api/resources/educationsubmission?view=graph-rest-beta&preserve-view=true).

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
- Obtenha uma coleção de recursos de [accessPackageAssignment](/graph/api/resources/accessPackageAssignment?view=graph-rest-beta&preserve-view=true) ao [filtrar no usuário conectado](/graph/api/accesspackageassignment-filterbycurrentuser?view=graph-rest-beta&preserve-view=true).
- Obtenha uma coleção de recursos de [accessPackageAssignmentRequest](/graph/api/resources/accessPackageAssignmentRequest?view=graph-rest-beta&preserve-view=true) ao [filtrar no usuário conectado](/graph/api/accesspackageassignmentrequest-filterbycurrentuser?view=graph-rest-beta&preserve-view=true).

### <a name="use-sdks"></a>Usar SDKs
Experimente a versão de visualização do [Microsoft Graph .NET SDK v4](https://www.nuget.org/packages/Microsoft.Graph/4.0.0-preview.4) e aproveite as seguintes melhorias:
- Use uma única API para autenticação em clientes do Microsoft Graph e Azure .NET.
- Novo suporte para serialização e desserialização JSON.
- Fácil acesso às informações de resposta.
- Melhor experiência de atualização de dependências.

## <a name="april-2021-new-and-generally-available"></a>Abril de 2021: novo e disponível para o público geral

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e login
- Gerenciar uma [política de autenticação](/graph/api/resources/authenticationflowspolicy) no nível de locatário para ativar ou desativar um [serviço autoatendimento de cadastramento](/graph/api/resources/selfservicesignupauthenticationflowconfiguration) para usuários externos.
- Os administradores podem associar fluxos de usuários a aplicativos que são compartilhados com usuários externos e permitir a [inscrição de autoatendimento](/azure/active-directory/external-identities/self-service-sign-up-overview) nesses aplicativos. Eles podem personalizar um fluxo de usuário de inscrição de autoatendimento e criar uma experiência de inscrição personalizada. Depois que um aplicativo é associado ao fluxo do usuário, os usuários que acessam esse aplicativo poderão iniciar um fluxo de inscrição que provisiona uma conta de convidado.
- Configurar os [atributos de fluxo de usuário](/graph/api/resources/identityuserflowattribute) no seu locatário do Azure AD permite que você colete informações sobre um usuário durante a inscrição. Você também pode coletar um conjunto embutido de atributos ou configurar atributos de fluxo de usuário personalizado para coletar informações de um usuário que não está integrado ao diretório. 
- Em um [fluxo de usuário do Azure Active Directory](/graph/api/resources/b2xidentityuserflow), você pode gerenciar os padrões de idioma e [personalizar o idioma e as cadeias de caracteres exibidas para os usuários no fluxo do usuário](/graph/api/resources/userflowlanguageconfiguration).
- Use um [conector de API](/graph/api/resources/identityapiconnector) em fluxos de usuário para inscrição de autoatendimento do Azure Active Directory e inscrição do Azure Active Directory B2C, para chamar uma API em uma etapa específica para afetar a execução do fluxo de usuário.

### <a name="teamwork"></a>Trabalho em equipe
- Identifique o canal pela propriedade **channelIdentity**, se uma [chatMessage](/graph/api/resources/chatmessage) estiver em um [canal](/graph/api/resources/channel).
- Identifique o chat pela propriedade **chatId**, se o **[chatMessage](/graph/api/resources/chatmessage)** estiver em um [chat](/graph/api/resources/chat).
- Use o relacionamento de **mensagens** para obter todos os recursos [chatMessage](/graph/api/resources/chatmessage) em um [chat](/graph/api/resources/chat).
- Use as permissões do aplicativo [obter](/graph/api/chat-get) propriedades de um [chat](/graph/api/resources/chat) específico.
- Use as permissões do aplicativo para [receber um membro específico do chat](/graph/api/chat-get-members) ou [todos os membros do chat](/graph/api/chat-list-members) incluídos em um chat. Como os dados dos usuários como membros do chat são confidenciais, além de obter permissões do aplicativo, [solicite acesso adicional](teams-protected-apis.md) para essas operações.

### <a name="use-the-toolkit"></a>Usar o kit de ferramentas
Novo no [Kit de ferramentas do Microsoft Graph](/graph/toolkit/overview)? Experimente o novo [caminho de aprendizagem do Kit de ferramentas ](/learn/paths/m365-msgraph-toolkit/?WT.mc_id=m365-19989-cxa), utilize o conjunto de componentes da web e provedores de autenticação do Kit de ferramentas para conectar um aplicativo da web ao Microsoft Graph e carregar dados do Microsoft 365.

## <a name="april-2021-new-in-preview-only"></a>Abril de 2021: Novo somente para visualização

### <a name="cloud-communications--online-meetings"></a>Comunicações na nuvem | Reuniões online
- Receba um [relatório](/graph/api/resources/meetingattendancereport?view=graph-rest-beta&preserve-view=true) da [participação de cada participante](/graph/api/resources/attendancerecord?view=graph-rest-beta&preserve-view=true) em uma reunião online agendada, por meio da propriedade **meetingAttendanceReport** de [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true).
- Habilitar, desabilitar ou limitar a duração do chat de uma reunião online usando a propriedade **allowMeetingChat**.
- Habilitar ou desabilitar reações a uma reunião online usando a propriedade **allowTeamworkReactions**.

### <a name="compliance"></a>Conformidade
[Obter](/graph/api/ediscovery-settings-get?view=graph-rest-beta&preserve-view=true), [atualizar](/graph/api/ediscovery-settings-update?view=graph-rest-beta&preserve-view=true)ou [redefinir para padrão](/graph/api/ediscovery-settings-resettodefault?view=graph-rest-beta&preserve-view=true) as seguintes [configurações ](/graph/api/resources/ediscovery-settings?view=graph-rest-beta&preserve-view=true) para um [caso](/graph/api/resources/ediscovery-case?view=graph-rest-beta&preserve-view=true) de Descoberta Eletrônica:
- [Detecção de duplicatas, quase duplicatas](/microsoft-365/compliance/near-duplicate-detection-in-advanced-ediscovery?view=o365-worldwide&preserve-view=true), e [thread de email](/microsoft-365/compliance/email-threading-in-advanced-ediscovery?view=o365-worldwide&preserve-view=true), por meio da propriedade **redundancyDetection**.
- [Identificar os temas](/microsoft-365/compliance/themes-in-advanced-ediscovery?view=o365-worldwide&preserve-view=true) que são ideias predominantes em documentos de um conjunto de revisão, por meio da propriedade **topicModeling** área de trabalho.
- [Extração de texto de arquivos de imagens por reconhecimento óptico de caracteres (OCR)](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery?view=o365-worldwide&preserve-view=true#optical-character-recognition-ocr), por meio da propriedade **ocr**.

Essas configurações fornecem funcionalidade de análise que [seleciona dados de forma inteligente](/microsoft-365/compliance/overview-ediscovery-20?view=o365-worldwide&preserve-view=true#cull-data-intelligently) no fluxo de trabalho de ponta a ponta da [Descoberta Eletrônica Avançada](/microsoft-365/compliance/overview-ediscovery-20?view=o365-worldwide&preserve-view=true).

### <a name="devices-and-apps--device-updates"></a>Dispositivos e aplicativos | Atualizações do dispositivo
Serviço de inicialização de APIs para a implantação do Windows Update para Empresas. O serviço dá suporte à implantação de atualizações de recursos do Windows 10 e à acelerar as atualizações de segurança do Windows 10 em dispositivos. Para saber mais, comece com a visão geral [da API de atualizações do Windows](windowsupdates-concept-overview.md).

### <a name="education"></a>Educação
- Associe uma pasta a um [educationAssignment](/graph/api/resources/educationAssignment?view=graph-rest-beta&preserve-view=true) para armazenar todos os recursos de arquivo relacionados, por meio da propriedade **resourcesFolderUrl**.
- Vínculo profundo em um [EducationAssignment](/graph/api/resources/educationAssignment?view=graph-rest-beta&preserve-view=true) por meio da propriedade **WebUrl**.

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
Os administradores podem [obter](/graph/api/accessreviewpolicy-get?view=graph-rest-beta&preserve-view=true) ou [atualizar](/graph/api/accessreviewpolicy-update?view=graph-rest-beta&preserve-view=true) políticas no nível de diretório para revisar o acesso, usando o recurso [accessReviewPolicy](/graph/api/resources/accessreviewpolicy?view=graph-rest-beta&preserve-view=true). Por exemplo, os administradores podem usar uma política de revisão do acesso para habilitar ou desabilitar os proprietários do grupo que estão avaliando o acesso em grupos que eles possuem.

### <a name="search"></a>Pesquisar
[Habilitar sugestões de ortografia ou correções](search-concept-speller.md) para uma consulta de usuário. Isso é útil quando uma consulta de usuário contém erros de digitação ou quando os erros não renderam nenhum resultado de pesquisa.

### <a name="teamwork"></a>Trabalho em equipe
- Use a [concessão de permissão específica do recurso](/graph/api/resources/resourcespecificpermissiongrant?view=graph-rest-beta&preserve-view=true) para listar os aplicativos com acesso a um determinado [grupo](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) ou [chat](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true).
- [Obter](/graph/api/teamsappicon-get?view=graph-rest-beta&preserve-view=true) as propriedades de um [ícone](/graph/api/resources/teamsAppIcon?view=graph-rest-beta&preserve-view=true) associado a um aplicativo do Teams. Para obter a imagem real do ícone, use [obter conteúdo hospedado](/graph/api/teamworkhostedcontent-get?view=graph-rest-beta&preserve-view=true).

### <a name="use-sdks"></a>Usar SDKs
- Experimente a [prévia da versão da biblioteca do cliente JavaScript do Microsoft Graph, versão 3.0.0](https://www.npmjs.com/package/@microsoft/microsoft-graph-client/v/3.0.0-Preview.1). Esta versão permite vários fluxos de autenticação, autenticação do lado do servidor, Stream Node.js de carregamento de arquivos grandes e acompanhamento de progresso e muito mais. Consulte o [guia de atualização](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/changelogs/v3-upgrade-guide.md) para obter detalhes.
- Experimente um novo caminho de aprendizagem para [explorar os cenários do Microsoft Graph para desenvolvimento do JavaScript](/learn/paths/m365-msgraph-scenarios/?WT.mc_id=m365-16105-cxa).


## <a name="want-to-stay-in-the-loop"></a>Quer ficar por dentro?

Estas são algumas maneiras de se envolver:

- Existem cenários em que você gostaria que o Microsoft Graph oferecesse suporte? Sugira e vote em novos recursos no [Microsoft Tech Community](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph).
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