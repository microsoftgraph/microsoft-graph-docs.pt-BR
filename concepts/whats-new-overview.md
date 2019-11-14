---
title: Novidades do Microsoft Graph
description: O que há de novo no Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 7d7d48b807c484bcdc237bf78124fec10ce0a54f
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/13/2019
ms.locfileid: "38303143"
---
# <a name="whats-new-in-microsoft-graph"></a>Novidades do Microsoft Graph

Confira os destaques das novidades do Microsoft Graph e como você pode [compartilhar suas ideias](#want-to-stay-in-the-loop). Para obter uma lista completa de atualizações da API, confira as seções de [novembro](changelog.md#november-2019) e [outubro](changelog.md#october-2019) do log de alterações da API. 

> [!IMPORTANT]
> Os recursos, incluindo APIs e ferramentas, no status de _visualização_, podem ser alterados sem aviso prévio e alguns talvez nunca sejam promovidos ao status DG. Não use os recursos de visualização em aplicativos de produção.


## <a name="november-2019-new-and-generally-available"></a>Novembro de 2019: novo e disponível para o público geral

### <a name="identity-and-access"></a>Identidade e acesso

Registre [aplicativos](/graph/api/resources/application?view=graph-rest-1.0) que se autenticam com o Azure Active Directory (Azure AD). Use as [permissões](/graph/permissions-reference#application-resource-permissions) delegadas, Application.Read.All e Application.ReadWrite.All ou as permissões de aplicativos, Application.Read.All, conforme apropriado.


## <a name="november-2019-new-in-preview"></a>Novembro de 2019: Novidades na versão prévia

### <a name="calendar"></a>Calendário

[Defina as propriedades](/graph/api/place-update?view=graph-rest-beta) para os tipos de local avançado de[sala](/graph/api/resources/room?view=graph-rest-beta) e [lista de sala](/graph/api/resources/roomlist?view=graph-rest-beta).

### <a name="devices-and-apps"></a>Dispositivos e aplicativos
Atualizações de [novembro](changelog.md#november-2019) do Intune

### <a name="people-and-workplace-intelligence"></a>Inteligência de pessoas e local de trabalho

Estreia do recurso do [perfil](/graph/api/resources/profile?view=graph-rest-beta) que é uma representação avançada da próxima geração de entidades de pessoas nos serviços da Microsoft. Esse recurso se relaciona aos atributos comuns e práticos de pessoas, incluindo informações sobre datas significativas, como [aniversários](/graph/api/resources/personanniversary?view=graph-rest-beta), [escolaridade](/graph/api/resources/educationalactivity?view=graph-rest-beta), [cargos](/graph/api/resources/workposition?view=graph-rest-beta), [interesses](/graph/api/resources/personinterest?view=graph-rest-beta), [idioma](/graph/api/resources/languageproficiency?view=graph-rest-beta) e [habilidades](/graph/api/resources/skillproficiency?view=graph-rest-beta) e competências, [participação em projetos](/graph/api/resources/projectparticipation?view=graph-rest-beta), [associação em sites](/graph/api/resources/personwebsite?view=graph-rest-beta) e outras informações de contato e [conta](/graph/api/resources/useraccountinformation?view=graph-rest-beta).


### <a name="search"></a>Pesquisar
Estreia da [API de Pesquisa da Microsoft](search-concept-overview.md) que permite aos usuários do aplicativo obter os resultados de pesquisa mais atualizados, personalizados e relevantes com a plataforma Microsoft Graph. Use o recurso de [consulta](/graph/api/search-query?view=graph-rest-beta)por padrão, pesquisas mensagens e eventos do Outlook e arquivos do OneDrive e do SharePoint na nuvem da Microsoft. Use os conectores [disponíveis](/microsoftsearch/connectors-overview) na [galeria de conectores do Microsoft Graph](/microsoftsearch/connectors-gallery), para incluir dados de pesquisa fora do Microsoft Cloud. Como alternativa, [construa seus próprios conectores](/graph/api/resources/indexing-api-overview?view=graph-rest-beta#common-use-cases), indexe arquivos e itens personalizados externos e consulte fontes de dados externas específicas.


## <a name="october-2019-new-and-generally-available"></a>Outubro de 2019: Novo e geralmente disponível

### <a name="identity-and-access"></a>Identidade e acesso
- Use [contatos da organização](/graph/api/resources/orgcontact?view=graph-rest-1.0) em aplicativos de produção. Os contatos da organização são gerenciados por administradores da organização, sincronizados de um Active Directory local ou do Exchange Online.
- Configure a [autenticação baseada em certificado](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started) em uma [organização](/graph/api/resources/organization?view=graph-rest-1.0).
- Adicionar e remover [credenciais de senha](/graph/api/resources/passwordcredential?view=graph-rest-1.0) para [aplicativos](/graph/api/resources/application?view=graph-rest-1.0).

### <a name="mail"></a>Email
Use o novo parâmetro de **mensagem** para atualizar quaisquer propriedades de [mensagem](/graph/api/resources/message?view=graph-rest-1.0) graváveis ao [responder](/graph/api/message-reply?view=graph-rest-1.0) a uma mensagem, por exemplo, [adicionar um destinatário à resposta](/graph/api/message-reply#example?view=graph-rest-1.0).

### <a name="microsoft-graph-data-connect"></a>Conexão de dados do Microsoft Graph
Os desenvolvedores e os cientistas de dados agora podem usar [ferramentas para traduzir dados do Office 365 para o formato Modelo de Dados Comum](https://github.com/OfficeDev/MS-Graph-Data-Connect/blob/master/Common-Data-Model/README.md), tornando-o esquematicamente consistente com outros conjuntos de dados prontos da Open Data Initiative (ODI). 


### <a name="microsoft-graph-sdks"></a>SDKs do Microsoft Graph
- Use os manipuladores de caos no SDK do JavaScript para verificar se um aplicativo é resistente a falhas de servidor que são difíceis de iniciar.
- Ler sobre [fazer chamadas API usando os SDKs](/graph/sdks/create-requests).

### <a name="users"></a>Usuários
- [Obtenha](/graph/api/user-get-mailboxsettings?view=graph-rest-1.0) ou [defina](/graph/api/user-update-mailboxsettings?view=graph-rest-1.0) as configurações preferenciais de formato de data e hora do usuário [para a caixa de correio do usuário](/graph/api/resources/mailboxsettings?view=graph-rest-1.0). 
- Rastreie a data/hora da última alteração de senha de um [usuário](/graph/api/resources/user?view=graph-rest-1.0).

## <a name="october-2019-new-in-preview"></a>Outubro de 2019: Novo em visualização

### <a name="calendar"></a>Calendário
- Os organizadores de reuniões podem [permitir que os convidados proponham horários de reunião alternativos ](outlook-calendar-meeting-proposals.md). Ao receber uma resposta de reunião que inclua um horário alternativo proposto, o organizador pode decidir aceitar a proposta e [atualizar](/graph/api/event-update?view=graph-rest-beta) o horário da reunião.
- O compartilhamento de calendário programático está mais parecido com a experiência do usuário do Outlook. Além de controlar as permissões do usuário atual e o status de compartilhamento de um calendário:
  - Para cada [calendário](/graph/api/resources/calendar?view=graph-rest-beta), você pode gerenciar as [permissões](/graph/api/resources/calendarpermission?view=graph-rest-beta) de cada usuário com o qual o calendário é compartilhado. 
  - Para cada [caixa de correio](/graph/api/resources/mailboxsettings?view=graph-rest-beta), você pode especificar se um representante, proprietário de caixa de correio ou ambos receberão mensagens da reunião e respostas da reunião. 
- Suporte adicional para reuniões online:
  - Para cada **calendário**, especifique os provedores de reuniões online permitidos e padrão.
  - Crie ou atualize um [evento](/graph/api/resources/event?view=graph-rest-beta) que esteja disponível online e forneça detalhes para que os participantes possam ingressar na reunião online. 
  - Em particular, use as novas propriedades **onlineMeetingProvider** e **onlineMeeting** do **evento** para definir ou identificar o Microsoft Teams como um provedor de reuniões online, uma solução alternativa para um [problema conhecido](known-issues.md#onlinemeetingurl-property-support-for-microsoft-teams) com a propriedade **onlineMeetingUrl**.

### <a name="devices-and-apps"></a>Dispositivos e aplicativos
Atualizações de [outubro](changelog.md#october-2019) do Intune

### <a name="graph-explorer"></a>Graph Explorer
Experimente a [próxima versão do Graph Explorer](https://developer.microsoft.com/graph/graph-explorer/preview) e confira informações contextuais úteis, como permissões, tokens de acesso e trechos de código do SDK nas novas guias **Permissões**, **Autenticação** e **Trechos de código**. Use o controle deslizante **Visualizar** para alternar entre a [produção](https://developer.microsoft.com/graph/graph-explorer) e a nova versão de visualização do Graph Explorer.

### <a name="groups"></a>Grupos
- Use as propriedades **hideFromAddressLists** e **hideFromOutlookClients** para controlar a visibilidade de um [grupo](/graph/api/resources/group?view=graph-rest-beta) em determinadas partes da interface do usuário do Outlook ou em um cliente do Outlook.
- [Atribuir](/graph/api/group-assignlicense?view=graph-rest-beta) ou remover licenças de usuários em um [grupo](/graph/api/resources/group?view=graph-rest-beta).

### <a name="identity-and-access"></a>Identidade e acesso
- Use as [políticas de acesso condicional](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta) para personalizar regras de acesso para uma organização. Essas regras consideram sinais sobre uma identidade de um usuário ou dispositivo, como associação a um usuário ou grupo, localização do IP e comportamentos, como tentativas de acesso a aplicativos específicos e comportamentos arriscados de logon.
- Use o [gerenciamento de direitos](/graph/api/resources/entitlementmanagement-root?view=graph-rest-beta) para gerenciar o acesso a grupos, aplicativos e sites do SharePoint Online para usuários dentro e fora de uma organização.
- Adicione e remova [credenciais de senha](/graph/api/resources/passwordcredential?view=graph-rest-beta) para [aplicativos](/graph/api/resources/application?view=graph-rest-beta) e [entidades de serviço](/graph/api/resources/serviceprincipal?view=graph-rest-beta).
- Gerenciar a [política de estrutura confiável](/graph/api/resources/trustframeworkkeyset?view=graph-rest-beta) do Azure AD B2C.
- Defina as políticas de [fluxo de usuário](/graph/api/resources/identityuserflow?view=graph-rest-beta) do Azure AD B2C para entrar, inscrever-se, entrar e Inscrever-se combinados, redefinir senha e atualizar perfil.
- Configure [rótulos de proteção de informações](/graph/api/resources/informationprotectionlabel?view=graph-rest-beta) para classificar a confidencialidade de um usuário ou locatário.
- Aplicativos existentes usando as APIs para [eventos de risco de identidade](/graph/api/resources/identityriskevent?view=graph-rest-beta) devem fazer ar transição para [ detecção de risco](/graph/api/resources/riskdetection?view=graph-rest-beta) no Azure AD Identity Protection. Confira a postagem de blog [ postagem de blog](https://developer.microsoft.com/graph/blogs/deprecatation-of-the-identityriskevents-api/) relacionada para obter mais detalhes e cronograma de descontinuação.


### <a name="mail"></a>Email
[Anexe arquivos grandes de até 150MB](outlook-large-attachments.md) a uma instância de [mensagem](/graph/api/resources/message?view=graph-rest-beta), criando uma [sessão de upload](/graph/api/resources/uploadsession?view=graph-rest-beta) e carregando iterativamente os intervalos do arquivo até que todos os bytes do arquivo tenham sido carregados. 

### <a name="microsoft-graph-security-api"></a>API de Segurança do Microsoft Graph
- Visualize a integração com a RSA NetWitness, ServiceNow e Splunk, para correlacionar e sincronizar [alertas](/graph/api/resources/security-api-overview?view=graph-rest-beta#alerts)e melhorar a proteção contra ameaças e respostas.
- Novos disparadores adicionados ao [Conector de Segurança do Microsoft Graph](https://docs.microsoft.com/connectors/microsoftgraphsecurity/) e [guias estratégicos](https://docs.microsoft.com/azure/security-center/security-center-playbooks) para Aplicativos de Lógica e Fluxo. Confira [exemplos de guias estratégicos](https://github.com/microsoftgraph/security-api-solutions/tree/master/Playbooks).
- Suporte no envio de [indicadores ameaças](/graph/api/resources/security-api-overview?view=graph-rest-beta#threat-indicators-preview) para o Microsoft Defender ATP para bloquear ou alertar ameaças usando suas próprias fontes de inteligência. Integrações com parceiros como o ThreatConnect permitem que os clientes enviem indicadores diretamente das soluções de inteligência e automação contra ameaças. 

### <a name="notifications"></a>Notificações
- [Crie e envie notificações](/graph/api/user-post-notifications?view=graph-rest-beta) a todos os clientes de aplicativos em todos os pontos de extremidade do dispositivo que um usuário está conectado, sem ter que gerenciar as permissões de usuário delegadas.
- Use [os pontos de extremidade da política de destino](/graph/api/resources/targetpolicyendpoints?view=graph-rest-beta) em [notificações](/graph/api/resources/notification?view=graph-rest-beta) do usuário para direcionar especificamente notificações para as plataformas Windows, iOS, Android ou WebPush.
- Especificar uma [política de retirada](/graph/api/resources/fallbackpolicy?view=graph-rest-beta) nas notificações para pontos de extremidade iOS, enviar notificações brutas de alta prioridade que podem não ser entregues aos dispositivos, caso contrário, devido a restrições específicas da plataforma, como o modo de economia de bateria.
- Use os novos SDKs de notificação simples para Windows, iOS, Android e JavaScript, no lugar do[SKD do Project Rome](https://github.com/Microsoft/project-rome) para aproveitar as vantagens de um modelo de autenticação aperfeiçoado e o suporte a aplicativos Web usando o push da Web.
 
### <a name="powershell-sdk"></a>SDK do PowerShell 
Os desenvolvedores e profissionais de TI podem observar o lançamento da [SDK do Microsoft Graph PowerShell](https://github.com/microsoftgraph/msgraph-sdk-powershell), que criará módulos que contêm cmdlets para criar solicitações da API REST do Microsoft Graph.

## <a name="want-to-stay-in-the-loop"></a>Quer ficar por dentro?

Estas são algumas maneiras de se envolver:

- Existem cenários em que você gostaria que o Microsoft Graph oferecesse suporte? Sugira e vote em novos recursos no [Microsoft Graph User Voice](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).
    Alguns novos recursos são originados como solicitações populares da comunidade de desenvolvedores. A equipe do Microsoft Graph avalia regularmente as necessidades dos clientes e lança novos recursos na seguinte ordem:

    1. Estreia no status de visualização **_prévia_**. As atualizações da API REST relacionadas estão no ponto de extremidade beta (`https://graph.microsoft.com/beta`).  

    2. Promovido para o status de**_disponibilidade geral_ (GA)**, se um feedback suficiente indicar a viabilidade. Todas as atualizações da API REST relacionadas serão adicionadas ao ponto de extremidade do v 1.0 (`https://graph.microsoft.com/v1.0`). 
- Seja um membro ativo da comunidade do Microsoft Graph! [Participe](https://aka.ms/microsoftgraphcall) da chamada mensal à comunidade do Microsoft Graph.
- Inscreva-se no [programa para desenvolvedores do Office 365](https://developer.microsoft.com/office/dev-program), obtenha uma assinatura gratuita do Office 365 e comece a desenvolver!


## <a name="see-also"></a>Confira também
- Confira o [blog de desenvolvedores do Microsoft Graph](https://developer.microsoft.com/graph/blogs/) periodicamente para comunicados de lançamentos e recursos úteis.
- Navegue pelas informações das inclusões da API do Microsoft Graph e pelas atualizações de comportamento de API no [changelog](changelog.md).
- Encontre [destaques de versões anteriores](whats-new-earlier.md).
- Saiba mais sobre o [controle de versão, suporte e mudanças significativas de políticas do Microsoft Graph](versioning-and-support.md).

