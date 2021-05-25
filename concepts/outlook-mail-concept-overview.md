---
title: Visão geral da API de email do Outlook
description: O Outlook é um hub de comunicação de mensagens do Microsoft 365. Ele também permite gerenciar contatos, agendar reuniões, encontrar informações sobre usuários em uma organização,
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.custom: scenarios:getting-started
ms.openlocfilehash: 0fcfb1a56e811d7ba63dcd1daed83122132c32bc
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2021
ms.locfileid: "52645623"
---
# <a name="outlook-mail-api-overview"></a>Visão geral da API de email do Outlook

O Outlook faz parte do hub de mensagens do Microsoft 365 que também permite gerenciar contatos, agendar reuniões, encontrar informações sobre usuários em uma organização, iniciar conversas online, compartilhar arquivos e colaborar em grupos.

> [!VIDEO https://www.youtube-nocookie.com/embed/L-gm25wusIQ]

## <a name="why-integrate-with-outlook-mail"></a>Por que integrar-se ao email do Outlook?

### <a name="integrate-with-rich-features-and-reach-hundreds-of-millions-of-customers"></a>Integrar recursos avançados e alcançar centenas de milhões de clientes

Integrar-se ao Outlook significa embarcar na experiência avançada que os clientes adoram, uma experiência consistente e intuitiva com emails, [contatos](outlook-contacts-concept-overview.md) e [calendário](outlook-calendar-concept-overview.md) que está disponível em todos os dispositivos: celular, web e desktop.

Ao usar o [Microsoft Graph](overview.md), você pode integrar-se ao Outlook escrevendo um aplicativo apenas uma vez e assim alcançar centenas de milhões de consumidores e dezenas de milhões de clientes empresariais que escolhem o Outlook como o cliente de email deles. Você pode escrever aplicativos que se concentrem em cenários de email ou que se conectem a uma grande variedade de outras inteligências, recursos e relações do Outlook ou fora dele, e criar cenários que têm suporte da nuvem da Microsoft.

### <a name="automate-message-organization-and-processing"></a>Automatizar o processamento e a organização de mensagens

Clientes gostam de como o Outlook os ajuda a se manterem organizados. O Microsoft Graph leva esses recursos para os desenvolvedores de aplicativos, permitindo que eles criem fluxos de trabalho de clientes que otimizam a descoberta e melhoram a eficiência e a produtividade:

- Os clientes organizam suas mensagens de várias maneiras - alguns deixam todas as mensagens na Caixa de Entrada e simplesmente buscam por elas; outros arquivam suas mensagens em pastas. Essas pessoas gostam da abordagem flexível e intuitiva do Outlook que oferece suporte a essas duas organizações: simples e com pastas. Os aplicativos podem, de forma conveniente, [filtrar, buscar ou classificar](query-parameters.md) as mensagem em pastas específicas ou em toda a caixa de correio do usuário.

- As categorias do Outlook são diferenciadas por nome e cor. As categorias permitem aos clientes classificarem as mensagens para aumentar a organização e a descoberta. Os aplicativos podem acessar e [definir a lista de categorias mestra do usuário](/graph/api/outlookuser-post-mastercategories). Além disso, essa lista é compartilhada entre mensagens do Outlook, assim como entre eventos, contatos, tarefas e postagens em grupo e ainda permitem cenários criativos para os desenvolvedores de aplicativo. Por exemplo, um provedor de treinamento online pode codificar por cor os emails, os eventos do curso e as atribuições de acompanhamento de cada curso que o usuário esteja inscrito.

- Além disso, os usuários do aplicativo podem alterar a prioridade de uma mensagem (evento ou tarefas) ou sinalizar uma mensagem para acompanhamento. (No momento, a sinalização está [no modo de visualização](versioning-and-support.md#beta-version) no Microsoft Graph).

- A API de regras transporta a organização de mensagens para um nível superior. Os aplicativos podem definir as [regras de Caixa de Entrada](/graph/api/resources/messagerule) para tratar imediatamente as mensagens que chegam e reduzir emails secundários. Por exemplo, um aplicativo pode mover automaticamente as mensagens para outra pasta se as linhas do assunto contiverem determinadas palavras-chave e atribuir categorias e prioridades para facilitar o acompanhamento posterior.

- Muitos clientes usam clientes de email que enviam e recebem mensagens no formato MIME. Embora o Outlook não salve mensagens no formato MIME, os aplicativos podem [obter o corpo de uma mensagem do Outlook no formato MIME](outlook-get-mime-message.md), [enviar mensagens do Outlook no formato MIME](outlook-send-mime-message.md), anexar assinaturas digitais S/MIME e criptografar o conteúdo da mensagem em S/MIME.

### <a name="write-smarter-apps-that-leverage-intelligence"></a>Escrever aplicativos mais inteligentes que potencializam a inteligência

Use o Microsoft Graph para sugerir dados contextuais aos usuários de seu aplicativo:

- Integrar-se à [Caixa de Entrada Destaques](/graph/api/resources/manage-focused-inbox) e [menções @ (prévia)](/graph/api/message-get?view=graph-rest-beta&preserve-view=true#example-2-get-all-mentions-in-a-specific-message) e permitir que os usuários de seu aplicativo leiam e respondam primeiro ao que é relevante para eles.

- Verificar as [dicas de email](/graph/api/resources/mailtips) ao redigir uma mensagem para obter informações úteis de status sobre um destinatário (por exemplo, se o destinatário enviou uma resposta automática ou se a caixa de correio está cheia). As dicas de email podem alertar os aplicativos a respeito de determinadas condições para permitir que se tomem ações de acompanhamento mais eficientes.

- Utilizar a [API de pessoas](people-example.md) para fornecer controles interativos, como o seletor de pessoas em seu aplicativo. A API de pessoas pode sugerir as pessoas mais relevantes para um usuário, tendo como base as comunicações, os padrões de colaboração e as relações comerciais desse usuário.

- Oferecer aos usuários do aplicativo um seletor de arquivos inteligente e sugerir arquivos com os quais eles tenham interagido recentemente para serem adicionados como anexos quando estiverem escrevendo uma mensagem. Os [Insights](/graph/api/resources/officegraphinsights) usam a análise avançada para sugerir arquivos que são familiares a um usuário, aqueles que tenham sido editados ou vistos pelo usuário ou compartilhados recentemente com ele.


### <a name="store-app-data-in-a-resource-or-resource-instance"></a>Armazenar os dados do aplicativo em um recurso ou em uma instância do recurso

Muitas vezes os aplicativos precisam armazenar os dados em um repositório de dados externo e acarretam sobrecarga no gerenciamento e no acesso dos dados. O Microsoft Graph permite que você simplesmente inclua dados de aplicativos como cabeçalhos de mensagens da Internet quando [criar](/graph/api/user-post-messages#example-2-create-message-draft-that-includes-custom-message-headers) ou [enviar](/graph/api/user-sendmail#example-2-create-a-message-with-custom-internet-message-headers-and-send-the-message) uma nova mensagem ou uma resposta a uma mensagem.

Se você precisar adicionar e atualizar dados personalizados subsequentemente, poderá [armazenar os dados em instâncias de recursos individuais](extensibility-overview.md#open-extensions). Se apropriado, como alternativa, você pode estender o esquema, adicionar propriedades personalizadas e armazenar dados digitados nos recursos do Microsoft Graph. Você pode fazer com que essas [extensões de esquema](extensibility-overview.md#schema-extensions) sejam passíveis de ser descobertas e compartilhadas.

## <a name="where-is-the-data"></a>Onde estão os dados?

[!INCLUDE [outlook-mailbox-type-support](../includes/outlook-mailbox-type-support.md)]

## <a name="api-reference"></a>Referência da API
Está procurando a referência de API para esse serviço?

- [API do email do Outlook no Microsoft Graph v1.0](/graph/api/resources/mail-api-overview)
- [API do email do Outlook no Microsoft Graph beta](/graph/api/resources/mail-api-overview?view=graph-rest-beta&preserve-view=true)


## <a name="next-steps"></a>Próximas etapas

- Selecione e experimente as consultas de exemplos de email do Outlook no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fmessages&version=v1.0). Escolha **Mostrar mais exemplos** na coluna à esquerda. Use o menu para habilitar o **Email do Outlook**.
- Saiba mais:

  - [Criar e enviar mensagens](outlook-create-send-messages.md)
  - Formas de [organizar mensagens](outlook-organize-messages.md)
  - [Obter conteúdo MIME de uma mensagem](outlook-get-mime-message.md)
  - [Anexar arquivos grandes a mensagens ou eventos do Outlook](outlook-large-attachments.md)
  - [Receber mensagens compartilhadas](outlook-share-messages-folders.md)
  - Como [enviar email de outro usuário](outlook-send-mail-from-other-user.md)
  - [Obter identificadores imutáveis para recursos do Outlook](outlook-immutable-id.md)
  - [Enviar emails com conteúdo MIME](outlook-send-mime-message.md)

- Saiba mais sobre como [usar a API de email](/graph/api/resources/mail-api-overview) e seus [casos de uso](/graph/api/resources/mail-api-overview#common-use-cases) no Microsoft Graph v1.0.


