---
title: Visão geral da API de contatos pessoais do Outlook
description: Os contatos do Outlook permitem que você armazene dados de contatos pessoais e fazem parte de um hub de mensagens do Outlook no Microsoft 365. Pelo Outlook, você pode gerenciar emails, agendar reuniões, saber mais sobre os usuários de uma organização, iniciar conversas online, compartilhar arquivos e colaborar em grupos.
author: angelgolfer-ms
ms.localizationpriority: high
ms.prod: outlook
ms.custom: scenarios:getting-started
ms.openlocfilehash: 909c79069912375cb4397812350b8c6448d640b4
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59066853"
---
# <a name="outlook-personal-contacts-api-overview"></a>Visão geral da API de contatos pessoais do Outlook

Os contatos do Outlook permitem que você armazene dados de contatos pessoais e fazem parte de um hub de mensagens do Outlook no Microsoft 365. Pelo Outlook, você pode gerenciar emails, agendar reuniões, saber mais sobre os usuários de uma organização, iniciar conversas online, compartilhar arquivos e colaborar em grupos.

## <a name="why-integrate-with-outlook-personal-contacts"></a>Por que se integrar aos contatos pessoais do Outlook?

### <a name="complement-messaging-and-calendaring-scenarios-for-hundreds-of-millions-of-customers"></a>Complemente os cenários de envio de mensagens e criação de calendário para centenas de milhões de clientes

Centenas de milhões de clientes e dezenas de milhões de clientes organizacionais escolhem o Outlook como serviço de email. Os contatos oferecem uma função complementar para mensagens e calendários ao permitirem que os clientes mantenham um armazenamento conveniente e integrado dos dados dos contatos no Outlook. Para os desenvolvedores, poder aproveitar a funcionalidade avançada de [email](outlook-mail-concept-overview.md) ou de [calendário](outlook-calendar-concept-overview.md) significa ter acesso a cenários mais amplos com os dados dos contatos do usuário.

### <a name="automate-contact-organization"></a>Automatizar a organização dos contatos

A API de contatos permite manter os seus clientes organizados, muito parecido com o que os clientes fazem por conta própria no Outlook:

- De forma parecida com a experiência do cliente, você pode criar instâncias de [contact](/graph/api/resources/contact?view=graph-rest-1.0) e atribuí-las aos objetos de [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-1.0).
- A API de contatos permite atribuir contatos de categorias, bem como eventos, mensagens, tarefas e postagens de grupo de maneira consistente para aprimorar a organização e a descoberta. Além disso, você pode [definir a lista mestra de categorias de um usuário](/graph/api/outlookuser-post-mastercategories?view=graph-rest-1.0), que possibilita outros cenários de criação.
- Você pode definir um sinalizador em um [contact](/graph/api/resources/contact?view=graph-rest-1.0) para fins de acompanhamento. (No momento, a sinalização está [no modo de visualização](versioning-and-support.md#beta-version) no Microsoft Graph).

### <a name="share-contact-information"></a>Compartilhar informações de contato

A API de contatos permite que você obtenha os itens de contato do usuário conectado ou dos usuários que compartilharam ou delegaram seus contatos ao usuário conectado. Por exemplo, se Henrique tiver compartilhado uma pasta de contato com Paulo ou tiver delegado acesso a Paulo, as [permissões delegadas](auth/auth-concepts.md#microsoft-graph-permissions) de Paulo também concederão acesso de leitura ao calendário e ao conteúdo que Henrique compartilhou.

### <a name="leverage-people-api-in-microsoft-graph-to-make-better-use-of-all-people-data"></a>Utilize a API de pessoas no Microsoft Graph para fazer melhor uso de todos os dados de pessoas

Você pode usar as operações CRUD típicas de um [contact](/graph/api/resources/contact?view=graph-rest-1.0) do Outlook para criar e gerenciar contatos. Como parte do Microsoft Graph, você também pode usar a [API de pessoas](people-example.md), que analisa os contatos do Outlook e as redes sociais de um usuário, o diretório da organização e as pessoas envolvidas em comunicações recentes e retornar informações sobre pessoas de todas essas fontes que são mais relevantes para o usuário. Utilize essa inteligência adicional em cenários do seletor de pessoas.

### <a name="take-advantage-of-other-shared-features-and-conveniences-in-microsoft-graph"></a>Utilizar outros recursos compartilhados e conveniências no Microsoft Graph

- A entidade **contact** é compatível com uma foto de contato que é implementada como a mesma entidade [profilePhoto](/graph/api/resources/profilephoto?view=graph-rest-1.0) da foto de usuário armazenada no Exchange Online ou no Azure Active Directory. Isso elimina a sobrecarga na conversão entre as fotos de perfil de usuário e de contato.
- Mantenha a loja de aplicativos local sincronizada inscrevendo-se em [alterar notificações](/graph/api/resources/webhooks?view=graph-rest-1.0) e [controlar as alterações](delta-query-overview.md) nos contatos e pastas de contato.
- Você pode ampliar o armazenamento de aplicativos em uma instância de contato como uma [extensão aberta](extensibility-overview.md#open-extensions) ou adicionar dados personalizados fortemente tipados ao esquema de contatos como uma [extensão de esquema](extensibility-overview.md#schema-extensions).

## <a name="where-is-the-data"></a>Onde estão os dados?

[!INCLUDE [outlook-mailbox-type-support](../includes/outlook-mailbox-type-support.md)]

## <a name="api-reference"></a>Referência da API

Está procurando a referência de API para esse serviço?

- [API de Contatos do Outlook no Microsoft Graph v1.0](/graph/api/resources/contact?view=graph-rest-1.0)
- [API de Contatos do Outlook no Microsoft Graph beta](/graph/api/resources/contact?view=graph-rest-beta)

## <a name="next-steps"></a>Próximas etapas

- Escolha e experimente os exemplos de consulta dos contatos no [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fcontacts&version=v1.0). Escolha **Mostrar mais exemplos** na coluna à esquerda. Use o menu para ativar **Contatos pessoais**.
- Saiba mais:
  - [Obter identificadores imutáveis para recursos do Outlook](outlook-immutable-id.md)
  - [Obter contatos compartilhados](outlook-get-shared-contacts-folders.md)
- Examine a referência da [API de contatos](/graph/api/resources/contact?view=graph-rest-1.0) do Outlook.
