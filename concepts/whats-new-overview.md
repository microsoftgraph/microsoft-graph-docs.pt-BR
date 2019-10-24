---
title: Novidades do Microsoft Graph
description: O que há de novo no Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: a851421ce76295bb2954621af9302b9eb420a8c0
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2019
ms.locfileid: "37622182"
---
# <a name="whats-new-in-microsoft-graph"></a>Novidades do Microsoft Graph

Você sabia que alguns dos novos recursos do Microsoft Graph se originam de solicitações populares da comunidade de desenvolvedores? 

A equipe do Microsoft Graph avalia regularmente as necessidades dos clientes e lança novos recursos na seguinte ordem:

1. Estreia no status de visualização **_prévia_**. As atualizações da API REST relacionadas estão no ponto de extremidade beta (`https://graph.microsoft.com/beta`).  

2. Promovido para o status de**_disponibilidade geral_ (GA)**, se um feedback suficiente indicar a viabilidade. Todas as atualizações da API REST relacionadas serão adicionadas ao ponto de extremidade do v 1.0 (`https://graph.microsoft.com/v1.0`). 

Abaixo, veja o que há de novo no Microsoft Graph e como você pode [compartilhar suas ideias](#want-to-stay-in-the-loop). Para detalhes sobre as atualizações da API, consulte as seções de [setembro](changelog.md#september-2019) e [agosto](changelog.md#august-2019) do log de alterações da API. 


## <a name="october-2019-new-and-generally-available"></a>Outubro de 2019: Novo e geralmente disponível

### <a name="mail"></a>Email
Use o novo parâmetro de **mensagem** para atualizar quaisquer propriedades de [mensagem](/graph/api/resources/message?view=graph-rest-1.0) graváveis ao [responder](/graph/api/message-reply?view=graph-rest-1.0) a uma mensagem, por exemplo, [adicionar um destinatário à resposta](/graph/api/message-reply#example?view=graph-rest-1.0).

### <a name="users"></a>Usuários
[Obtenha](/graph/api/user-get-mailboxsettings?view=graph-rest-1.0) ou [defina](/graph/api/user-update-mailboxsettings?view=graph-rest-1.0) as configurações preferenciais de formato de data e hora do usuário [para a caixa de correio do usuário](/graph/api/resources/mailboxsettings?view=graph-rest-1.0). 

## <a name="october-2019-new-in-preview"></a>Outubro de 2019: Novo em visualização

> [!IMPORTANT]
> Os recursos, incluindo APIs e ferramentas, no status de _visualização_, podem ser alterados sem aviso prévio e alguns talvez nunca sejam promovidos ao status GA. Não use-os em aplicativos de produção.

### <a name="calendar"></a>Calendário

Os organizadores de reuniões podem [permitir que os convidados proponham horários de reunião alternativos ](outlook-calendar-meeting-proposals.md). Ao receber uma resposta de reunião que inclua um horário alternativo proposto, o organizador pode decidir aceitar a proposta e [atualizar](/graph/api/event-update?view=graph-rest-beta) o horário da reunião.

### <a name="groups"></a>Grupos
Use as propriedades **hideFromAddressLists** e **hideFromOutlookClients** para controlar a visibilidade de um [grupo](/graph/api/resources/group?view=graph-rest-beta) em determinadas partes da interface do usuário do Outlook ou em um cliente do Outlook.

### <a name="mail"></a>Email

[Anexe arquivos grandes de até 150MB](outlook-large-attachments.md) a uma instância de [mensagem](/graph/api/resources/message?view=graph-rest-beta), criando uma [sessão de upload](/graph/api/resources/uploadsession?view=graph-rest-beta) e carregando iterativamente os intervalos do arquivo até que todos os bytes do arquivo tenham sido carregados. 

## <a name="september-2019-new-and-generally-available"></a>Setembro de 2019: novo e disponível para o público geral

### <a name="calendar-mail-and-group"></a>Calendário, email e grupo
[Obter o conteúdo bruto de um arquivo, ou o conteúdo MIME de um item](/graph/api/attachment-get?view=graph-rest-1.0#get-the-raw-contents-of-a-file-or-item-attachment) que foi adicionado como um [anexo](/graph/api/resources/attachment?view=graph-rest-1.0) a um[evento](/graph/api/resources/event?view=graph-rest-1.0), [ mensagem](/graph/api/resources/message?view=graph-rest-1.0)ou[ postagem](/graph/api/resources/post?view=graph-rest-1.0) de grupo.

### <a name="calendar-mail-outlook-task-personal-contact"></a>Calendário, email, tarefa do Outlook, contato pessoal
Use a função [translateExchange](/graph/api/user-translateexchangeids?view=graph-rest-1.0) para converter uma ID de item do Outlook [entre](/graph/api/user-translateexchangeids?view=graph-rest-1.0#exchangeidformat-values)formatos suportados, incluindo o formato de ID padrão do Microsoft Graph e o formato de ID imutável. 

Os recursos a seguir são compatíveis com a conversão de formato de ID:

- [attachment](/graph/api/resources/attachment?view=graph-rest-1.0)
- [contato](/graph/api/resources/contact?view=graph-rest-1.0)
- [event](/graph/api/resources/event?view=graph-rest-1.0)
- [eventMessage](/graph/api/resources/eventmessage?view=graph-rest-1.0)
- [message](/graph/api/resources/message?view=graph-rest-1.0)
- [outlookTask](/graph/api/resources/outlooktask?view=graph-rest-1.0)

### <a name="mail"></a>Email
[Obter conteúdo MIME de uma mensagem](outlook-get-mime-message.md).

### <a name="microsoft-graph-toolkit"></a>Microsoft Graph Toolkit
Use o [Microsoft Graph Toolkit](toolkit/overview.md) para desenvolver aplicativos de produção que ofereçam uma aparência consistente do Microsoft 365 e economize tempo na autenticação e acesso a dados do Microsoft Graph.

## <a name="september-2019-new-in-preview"></a>Setembro de 2019: novidades na versão prévia

> [!IMPORTANT]
> Os recursos, incluindo APIs e ferramentas, no status de _visualização_, podem ser alterados sem aviso prévio e alguns talvez nunca sejam promovidos ao status GA. Não use-os em aplicativos de produção.

### <a name="devices-and-apps"></a>Dispositivos e aplicativos
Atualizações de [Setembro](changelog.md#september-2019) do Intune

### <a name="files"></a>Arquivos
- Suporte aprimorado à sincronização:

  - Use a nova propriedade **pendingOperations** para identificar operações que podem afetar o conteúdo binário de um [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta).
  - [Restaure](/graph/api/driveitem-restore?view=graph-rest-beta) um **driveItem** excluído. 
- Use o Algoritmo de Hash Seguro (SHA-256) para aprimorar a segurança e a integridade dos [dados](/graph/api/resources/file?view=graph-rest-beta) do arquivo.
- Obtenha ou defina a orientação de uma [foto](/graph/api/resources/photo?view=graph-rest-beta). A configuração é compatível com o OneDrive Personal.

### <a name="identity-and-access"></a>Identidade e acesso
- Use a propriedade new **identities** e obtenha as identidades que um [usuário](/graph/api/resources/user?view=graph-rest-beta) pode usar para entrar em uma conta. As identidades podem ser fornecidas por organizações ou provedores de identidade social, como Facebook, Google e Microsoft.
- Aperfeiçoamentos incrementais para [sincronizar identidades](/graph/api/resources/synchronization-overview?view=graph-rest-beta) em um aplicativo de nuvem para um locatário:

  - Armazenar configurações para um [trabalho de sincronização](/graph/api/resources/synchronization-synchronizationjob?view=graph-rest-beta)
  - Especifique um motivo para impor a [quarentena](/graph/api/resources/synchronization-quarantine?view=graph-rest-beta) a um trabalho de sincronização

### <a name="teamwork"></a>Trabalho em equipe
Use o canal **Geral** de uma [equipe](/graph/api/resources/team?view=graph-rest-beta) ou personalize as [configurações de membros](/graph/api/resources/teammembersettings?view=graph-rest-beta) para permitir que eles criem canais privados na **equipe**.

### <a name="users"></a>Usuários
- Obtenha ou atualize as identidades com as quais um [usuário](/graph/api/resources/user?view=graph-rest-beta) pode entrar em uma conta. Essas identidades podem ser fornecidas por organizações de negócios ou por provedores de identidade social, como o Facebook, o Google e a Microsoft.
- Obtenha ou atualize as [configurações da caixa de correio](/graph/api/resources/mailboxsettings?view=graph-rest-beta) do formato de data e hora escolhidas pelo usuário.


## <a name="want-to-stay-in-the-loop"></a>Quer ficar por dentro?
- Existem cenários em que você gostaria que o Microsoft Graph oferecesse suporte? Sugira e vote em novos recursos no [Microsoft Graph User Voice](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).
- Seja um membro ativo da comunidade do Microsoft Graph! [Participe](https://aka.ms/microsoftgraphcall) da chamada mensal à comunidade do Microsoft Graph.
- Inscreva-se no [programa para desenvolvedores do Office 365](https://developer.microsoft.com/pt-BR/office/dev-program), obtenha uma assinatura gratuita do Office 365 e comece a desenvolver!


## <a name="see-also"></a>Confira também
- Confira o [blog de desenvolvedores do Microsoft Graph](https://developer.microsoft.com/pt-BR/graph/blogs/) periodicamente para comunicados de lançamentos e recursos úteis.
- Navegue pelas informações das inclusões da API do Microsoft Graph e pelas atualizações de comportamento de API no [changelog](changelog.md).
- Encontre [destaques de versões anteriores](whats-new-earlier.md).
- Saiba mais sobre o [controle de versão, suporte e mudanças significativas de políticas do Microsoft Graph](versioning-and-support.md).

