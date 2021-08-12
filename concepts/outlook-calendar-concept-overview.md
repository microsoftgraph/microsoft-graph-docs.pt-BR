---
title: Visão geral da API do calendário do Outlook
description: O calendário do Outlook faz parte do hub de mensagens do Outlook no Microsoft 365 que também permite gerenciar emails e contatos, encontrar informações sobre usuários em uma organização,
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.custom: scenarios:getting-started
ms.openlocfilehash: 163ad507c924076e16cc5db83100e62a68dfe98850930bbd0fe7a36ab18945e3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54218314"
---
# <a name="outlook-calendar-api-overview"></a>Visão geral da API do calendário do Outlook

O calendário do Outlook faz parte do hub de mensagens do Outlook no Microsoft 365 que também permite gerenciar emails e contatos, encontrar informações sobre usuários em uma organização, iniciar conversas online, compartilhar arquivos e colaborar em grupos.

> [!VIDEO https://www.youtube-nocookie.com/embed/_ST4nyz4g9E]

## <a name="why-integrate-with-outlook-calendar"></a>Por que integrar-se com o calendário do Outlook?
Os recursos avançados do calendário do Outlook e sua API trazem várias oportunidades de aplicativos. As seções a seguir listam algumas delas.

## <a name="reach-hundreds-of-millions-of-customers-and-build-rich-scenarios"></a>Alcance centenas de milhões de clientes e crie cenários sofisticados

Muitos milhões de clientes usam o calendário do Outlook como parte de um hub integrado que permite que eles se comuniquem e realizem tarefas com eficiência. Eles podem configurar reuniões, gerenciar emails, encontrar informações sobre contatos e outros usuários e iniciar conversas ou reuniões online, tudo em um único lugar, na Web, em dispositivos móveis ou na área de trabalho. O Microsoft Graph não só conecta os aplicativos aos dados do calendário, email e contatos desses clientes, permite que os aplicativos [se integrem ao melhor do Microsoft 365](overview-major-services.md) e ofereçam suporte a uma ampla variedade de cenários que aumentam a produtividade e a colaboração.

A maioria dos recursos da API do calendário do Outlook se aplica a calendários em contas pessoais da Microsoft e contas corporativas ou de estudante.

<sup>**</sup> Indica recursos a seguir especificamente aplicáveis aos calendários do Outlook em contas corporativas ou de estudante.

## <a name="automate-appointment-organization-and-calendaring"></a>Automatizar a organização de compromissos e o calendário

Os clientes gostam da forma como o Outlook permite que eles organizem seu tempo dedicado ao trabalho, família e atividades pessoais. A API REST do Microsoft Graph mantém uma estreita paridade com a experiência do cliente, permitindo que os aplicativos criem, gerenciem e respondam a eventos com a mesma naturalidade:

- No Outlook, os clientes podem criar calendários individuais para fins profissionais, familiares e outros e organizá-los em grupos do calendário. Eles podem ativar o calendário gratuito de **Aniversários** e **Feriados** para lembrá-los dos aniversários e dos feriados locais dos contatos. Eles podem adicionar calendários que correspondam aos seus interesses, como calendários de times esportivos e programas de TV. Os clientes podem escolher e sobrepor calendários e ver seus eventos na mesma visualização. Com a API de calendário, seu aplicativo pode organizar [calendários](/graph/api/resources/calendar?view=graph-rest-1.0) em [grupos de calendários](/graph/api/resources/calendargroup?view=graph-rest-1.0) e interagir com calendários interessantes como qualquer outro **calendário** na caixa de correio do usuário.

- Os clientes do Outlook podem aplicar categorias a eventos, mensagens, contatos, tarefas e postagens de grupo de maneira consistente para aprimorar a organização e a descoberta. A API de calendário permite acessar e [definir uma lista mestra de categorias de usuários](/graph/api/outlookuser-post-mastercategories?view=graph-rest-1.0) que abre outros cenários de criação. Por exemplo, um clube de atletismo pode organizar um torneio esportivo e oferecer um aplicativo que diferencia emails e eventos de cada esporte com sua própria categoria de cor. Para saber as últimas notícias, como alterações de horários imprevistas, o aplicativo também pode definir a propriedade **importance** desses eventos e emails para alertar os clientes.

- Em uma pasta de calendário, você pode [criar](/graph/api/user-post-events?view=graph-rest-1.0) e [atualizar](/graph/api/event-update?view=graph-rest-1.0) [eventos](/graph/api/resources/event?view=graph-rest-1.0) de instância única ou [agendar e manter eventos recorrentes](outlook-schedule-recurring-events.md). Você pode deixar seus clientes responderem a [solicitações de reunião](/graph/api/resources/eventmessage?view=graph-rest-1.0) e [adiar](/graph/api/event-snoozereminder?view=graph-rest-1.0) ou [dispensar](/graph/api/event-dismissreminder?view=graph-rest-1.0) [lembretes](/graph/api/resources/reminder?view=graph-rest-1.0) usando a propriedade de navegação **event**.

## <a name="help-customers-stay-synchronized-and-navigate-their-day"></a>Ajude os clientes a manterem-se sincronizados e a orientar seu dia de trabalho

A API de calendário ajuda os clientes a orientar seu dia de trabalho e aumentar a produtividade. Com ela, você pode:

<!-- change link to notifications to the concept topic once it's created. In general, try staying in the conceptual level in these overview topics, if conceptual topics are available for the link destination.
-->

- Manter a loja de aplicativos local sincronizada inscrevendo-se em [alterar notificações](/graph/api/resources/webhooks?view=graph-rest-1.0) e [controlar as alterações em eventos](delta-query-events.md) no calendário de um usuário.
- Exibir a agenda do usuário com base em um [modo de exibição lembrete](/graph/api/user-reminderview?view=graph-rest-1.0).
- Você pode deixar que o usuário convenientemente [aceite](/graph/api/event-accept?view=graph-rest-1.0) e participe de uma reunião online usando a propriedade **webLink**, que abre a reunião no Outlook na Web.
- Os usuários também podem [aceitar provisoriamente](/graph/api/event-tentativelyaccept?view=graph-rest-1.0) ou [recusar](/graph/api/event-decline?view=graph-rest-1.0) uma reunião quando estiverem em trânsito.

## <a name="enhance-collaboration"></a>Melhorar a colaboração

- No Outlook, os clientes podem compartilhar calendários com entre eles e conceder permissões para ler, gravar ou excluir conteúdo do calendário. Ou podem delegar um calendário para que outro cliente responda a solicitações de reunião em nome deles. De forma programática, embora não seja possível iniciar uma ação de compartilhamento ou delegação em nome de um usuário, você pode usar um conjunto de propriedades para verificar o status de compartilhamento e habilitar cenários em torno de calendários compartilhados ou delegados: **canEdit**, **canShare**, **canViewPrivateItems**, **isShared** e **isSharedWithMe**.
- A API de calendário permite que você receba itens de calendário do usuário conectado ou de usuários que compartilharam ou delegaram seus calendários ao usuário conectado. Por exemplo, se Henrique tiver compartilhado um calendário com Davi ou tiver delegado acesso a Davi, as [permissões delegadas](auth/auth-concepts.md#microsoft-graph-permissions) de Davi também concederão acesso de leitura ao calendário e ao conteúdo que Henrique compartilhou.
- Os grupos do Microsoft 365 permitem que os membros do grupo colaborem e acessem conversas e calendários de grupo diretamente no Outlook de forma prática. Além de algumas pequenas diferenças entre os calendários de grupo e os calendários de usuários, a API de calendário permite que você interaja com os calendários de grupo da mesma forma que interagiria com os calendários de usuários. Confira o recurso de [calendário](/graph/api/resources/calendar?view=graph-rest-1.0) para obter mais informações<sup>**</sup>.

## <a name="schedule-smart"></a>Agendar de forma inteligente

O Outlook e a API de calendário oferecem muitas conveniências inteligentes para agendar eventos:

- Com as configurações do aplicativo de calendário do Outlook, os clientes podem ativar a adição automática de eventos nos emails, como reservas de voos, hotéis ou restaurantes, e cobrar faturas. Após a adição dessas configurações, você poderá interagir com esses eventos da mesma maneira que interagiria com outros objetos [events](/graph/api/resources/event?view=graph-rest-1.0) na caixa de correio do usuário e criar cenários criativos sobre esse recurso do Outlook.
- No Outlook, reservar uma sala de reunião é tão simples quanto adicionar um participante ao **evento**. A API de calendário representa uma sala de reunião como um objeto [emailAddress](/graph/api/resources/emailaddress?view=graph-rest-1.0). Você pode [obter salas](/graph/api/place-list#example-1-list-all-the-rooms-defined-in-the-tenant) e [obter listas de salas](/graph/api/place-list#example-2-list-all-the-room-lists-defined-in-the-tenant) disponíveis em um locatário. Para organizar uma reunião em uma sala específica, atribua-a à propriedade **local** do **evento**.<sup>**</sup>
- Você pode [consultar informações de disponibilidade de usuários e recurso](outlook-get-free-busy-schedule.md) por um período de tempo específico. Depois, pode aplicar esses dados a cenários diferentes, incluindo o planejamento de recursos e agendamento de eventos. <sup>**</sup>
- Se o seu cenário envolver o agendamento de reuniões em horários ideais, considere o [uso de findMeetingTimes para identificar horários ou locais possíveis para a reunião](findmeetingtimes-example.md). A função [findMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-1.0) considera o status de disponibilidade dos participantes e as salas, horários e outras restrições que você tenha marcado como preferencial. Se a primeira tentativa não retornar um horário de reunião comum, verifique o motivo, ajuste seus critérios e chame **findMeetingTimes** novamente.<sup>**</sup>

## <a name="teleconference-across-multiple-locations-and-time-zones"></a>Teleconferência em vários locais e fusos horários

Com a globalização, as atuais reuniões de negócios geralmente envolvem participantes de diferentes locais e fusos horários. Veja aqui como você pode usar o API de calendário para gerenciar essas reuniões:

- Como exemplo no Outlook, os clientes podem organizar uma reunião e incluir participantes de uma sala de conferências em Seattle, uma cafeteria em Paris e um escritório doméstico na China. De forma programática, a propriedade **locations** do evento, que é uma coleção de objetos [location](/graph/api/resources/location?view=graph-rest-1.0), pode refletir esse nível de detalhes em **displayName** e **locationType** para cada **location**. Veja um [exemplo](/graph/api/event-get?view=graph-rest-1.0#request-2).
- O Outlook oferece aos clientes a flexibilidade de organizar eventos e especificar um fuso horário para cada um dos horários de início e término de um evento. Para oferecer suporte a essa flexibilidade, por padrão, a API de calendário retorna os horários de **início** e **término** de um **evento** em UTC e oferece as propriedades **originalStartTimeZone** e **originalEndTimeZone** para observar os fusos horários usados quando o evento foi criado.
- Como alternativa, você pode especificar o cabeçalho `Prefer: outlook.timezone="{time zone name}"` para que uma operação de evento GET retorne **início** e **término** no fuso horário especificado. O nome do fuso horário pode ser qualquer um dos nomes compatíveis com o Windows e, também, os nomes nesta [lista](/graph/api/resources/datetimetimezone?view=graph-rest-1.0). Confira um [exemplo](/graph/api/event-get?view=graph-rest-1.0#request-1) de cabeçalho `Prefer` em uso.
- As organizações que oferecem suporte para provedores de reuniões online, como o Microsoft Teams e o Skype, podem configurar calendários do Outlook para usar esses serviços. Você pode facilmente [organizar os eventos nesses calendários como reuniões online](outlook-calendar-online-meetings.md).

## <a name="build-apps-with-location-awareness-and-provide-intelligent-context"></a>Crie aplicativos com reconhecimento de localização e forneça contexto inteligente

Use a [API de locais](/graph/api/resources/place) para ajudar os usuários a navegar em um local ou fornecer uma solução inteligente baseada no local do usuário. A seguir estão alguns cenários de exemplo:

- Incorporar detalhes do lugar em eventos de calendário para ajudar os usuários a orientarem o dia e melhorar a produtividade.<sup>**</sup>
- Atender aos aplicativos pode usar a API de locais para ajudar a se orientar no local e a configuração.<sup>**</sup>
- Automatizar detalhes de pré-lançamento de email para os participantes e incluir um mapa sobre como chegar a uma sala..<sup>**</sup>
- Configurar que os assistentes de bot de recepção forneçam informações sobre as salas em um prédio.<sup>**</sup> 

Dependendo do cenário do aplicativo, você pode usar a API locais no contexto do Outlook ou independente do Outlook.

## <a name="take-advantage-of-social-intelligence-and-other-developer-conveniences-in-microsoft-graph"></a>Aproveite a inteligência social e outras conveniências de desenvolvedor no Microsoft Graph

Use a [API de pessoas](people-example.md) no Microsoft Graph para conectar-se a [dados de pessoas](/graph/api/resources/person?view=graph-rest-1.0) que são baseados nos padrões de comunicação e colaboração de um usuário e nas relações comerciais. Você pode implementar controles, como um seletor de pessoas, e sugerir pessoas relevantes para o usuário ao organizar reuniões em nome do usuário.

Economize custos indiretos ao armazenar e gerenciar dados de aplicativos em armazenamentos de dados externos. Com o Microsoft Graph, você pode armazenar dados de aplicativos personalizados como [extensões abertas](extensibility-overview.md#open-extensions) em instâncias de recursos individuais. Se você precisar que os dados sejam digitados ou gostaria de poder compartilhar o esquema digitado, poderá armazenar dados de aplicativos personalizados em [extensões de esquema](extensibility-overview.md#schema-extensions).

## <a name="where-is-the-data"></a>Onde estão os dados?

[!INCLUDE [outlook-mailbox-type-support](../includes/outlook-mailbox-type-support.md)]

## <a name="api-reference"></a>Referência da API

Está procurando a referência de API para esse serviço?

- [API do Calendário do Outlook no Microsoft Graph v1.0](/graph/api/resources/calendar?view=graph-rest-1.0)
- [API do Calendário do Outlook no Microsoft Graph beta](/graph/api/resources/calendar?view=graph-rest-beta)

## <a name="next-steps"></a>Próximas etapas

- Escolha e experimente consultas de exemplo de calendários no [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fevents&version=v1.0).
- Saiba mais:
  - [Encontrar possíveis horários de reunião no calendário do Outlook](findmeetingtimes-example.md)
  - [Obter informações de disponibilidade de usuários e recursos](outlook-get-free-busy-schedule.md)
  - [Propor horários de reunião em um calendário do Outlook (versão prévia)](outlook-calendar-meeting-proposals.md)
  - [Usar o Outlook para organizar e participar de reuniões online (versão prévia)](outlook-calendar-online-meetings.md)
  - [Agendar compromissos repetidos como eventos recorrentes no Outlook](outlook-schedule-recurring-events.md)
  - [Obter eventos compartilhados](outlook-get-shared-events-calendars.md)
  - [Anexar arquivos grandes a mensagens ou eventos do Outlook](outlook-large-attachments.md)
  - [Obter identificadores imutáveis para recursos do Outlook](outlook-immutable-id.md)
- Examine a referência da [API de calendário](/graph/api/resources/calendar?view=graph-rest-1.0) do Outlook.

<!-- Replace the last item with the calendar API overview when it's published.
-->
