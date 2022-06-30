---
title: Escolha uma API no Microsoft Graph para criar e participar de reuniões online
description: Considere quando usar o recurso de evento da API de calendário ou o recurso onlineMeeting da API de comunicações na nuvem para reuniões do Teams e do Skype no calendário do Outlook.
author: angelgolfer-ms
ms.localizationpriority: high
ms.openlocfilehash: 8af02249b97eea35269cbcbf565cd75b74368d7f
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66436397"
---
# <a name="choose-an-api-in-microsoft-graph-to-create-and-join-online-meetings"></a>Escolha uma API no Microsoft Graph para criar e participar de reuniões online

O Microsoft Graph oferece dois conjuntos de APIs que organizam e participam de reuniões online no Microsoft Teams ou no Skype:

- [API do Calendário do Outlook](outlook-calendar-online-meetings.md): use o recurso [evento](/graph/api/resources/event).
- [API de Comunicações em Nuvem](cloud-communications-online-meetings.md): use o recurso [onlineMeeting](/graph/api/resources/onlineMeeting).

A escolha é entre:
- Uma maneira programática e conveniente de, no calendário do Outlook, configurar uma reunião on-line, onde os participantes clicam para ingressar na reunião e continuar sua experiência no Teams ou no Skype.
- Uma integração programática mais rica dos recursos do Teams ou do Skype em um aplicativo para uma experiência mais personalizada.

## <a name="considerations-when-choosing-an-api-for-your-scenario"></a>Considerações ao escolher uma API para o seu cenário

Escolha a API do calendário para uma integração otimizada e integrada ao calendário do Outlook, que resulta em um evento de reunião online no calendário do Outlook:
- Suporte programático:
  - Os aplicativos podem _criar ou atualizar diretamente um evento como uma reunião on-line no calendário do Outlook_, com um blob de ingresso na reunião do Teams inserido no evento de calendário do Outlook.
  - Os aplicativos obtêm propriedades para ingressar na reunião pela Internet ou discando.
- A experiência da interface do usuário dos participantes com o evento do calendário criado programaticamente está em paridade total com qualquer evento criado por meio da interface do usuário do Outlook:
  - Os participantes podem optar por se encontrar on-line ou pessoalmente.
  - Os participantes podem clicar no blob para juntar-se a reunião do Teams pela Internet ou discando.
  - Os participantes podem usar outros recursos avançados do Teams, incluindo videoconferência e lobby da reunião, se configurados.

> [!NOTE]
> A integração com o calendário do Outlook pressupõe que um administrador configurou o Outlook para reuniões online. [Verifique](/microsoftteams/exchange-teams-interact) o suporte antes de usar a API.

Escolha a API de comunicações na nuvem para flexibilidade e suporte programático mais amplo:
- Os aplicativos têm mais flexibilidade para integrar ainda mais os resultados da API com a linha de negócios e outros aplicativos. A API é desassociada de qualquer calendário específico e não cria um evento em nenhum calendário.
- Os aplicativos podem fornecer os seguintes recursos para os participantes:
  - Informações de junção baseadas em local.
  - Ingressando na reunião pela Internet ou discando.
  - Videoconferência.
  - Recursos adicionais de segurança, como lobby de reunião e automação da admissão de participante (visualização).
  - Associando uma reunião a um bate-papo do Microsoft Teams.

## <a name="comparing-the-apis"></a>Comparando as APIs

A tabela a seguir detalha as diferenças no nível da API. 


| Recurso de reunião online | API do Calendário (recurso de evento) | API de comunicação na nuvem (recurso onlineMeeting)             |
|:-----------------------|:------------------------------|:-------------------------------------------------------------|
| Membros principais da API | recurso de [evento](/graph/api/resources/event): <br>propriedade - **isOnlineMeeting**  <br>propriedade - **onlineMeeting** do tipo [onlineMeetingInfo](/graph/api/resources/onlinemeetinginfo) <br>propriedade - **onlineMeetingProvider** <br> recurso do [calendário](/graph/api/resources/calendar): <br>propriedade - **allowedOnlineMeetingProviders** <br>propriedade - **defaultOnlineMeetingProvider** <br> | recurso do [onlineMeeting](/graph/api/resources/onlinemeeting) <br> recurso do [audioConferencing](/graph/api/resources/audioconferencing)
| Integração com um item de calendário | <br>A API- [criar](/graph/api/user-post-events) ou [atualizar](/graph/api/event-update) **evento** define automaticamente o calendário resultante do [evento](/graph/api/resources/event) Outlook como uma reunião online.<br>- Use as propriedades **isOnlineMeeting**, **onlineMeeting**, e **onlineMeetingProvider** propriedades retornadas do **evento** do calendário Outlook.  | A API- [criar](/graph/api/application-post-onlinemeetings) retorna um recurso [onlineMeeting](/graph/api/resources/onlinemeeting) que é independente de um tipo de calendário específico. <br>- Não cria nem atualiza nenhum evento do Outlook. <br>- Integre as informações de recurso **onlineMeeting** retornadas em uma experiência de aplicativo apropriada para o seu cenário. <br>- Utilize [createOrGet](/graph/api/onlinemeeting-createorget) para retornar uma reunião on-line que tenha um valor especificado **externalId** ou crie um, se já não existir, para otimizar a incorporação da reunião resultante em um calendário de terceiros. |
| Alterando para reunião offline | - Não - depois de ativar um **evento** para ingressar online, você não poderá atualizar para torná-lo uma reunião offline.<br>- Não é possível alterar a propriedade **onlineMeetingProvider** nem definir **isOnlineMeeting** para `false` desativar a reunião online. | Não - Depois de criar um recurso **onlineMeeting** você poderá apenas excluí-lo, mas não poderá alterá-lo para uma reunião offline. |
| Informações de participação com base na localidade | Nenhuma integração direta da API. | - Use o cabeçalho HTTP `Accept-Language` ao criar uma reunião online. <br>- Veja o [exemplo](/graph/api/application-post-onlinemeetings#example-2-create-an-online-meeting-with-user-token). |
| Entrando na Internet (VoIP) | Por meio da propriedade **onlineMeeting** acesse **joinUrl**.  | Utilize a propriedade **joinWebUrl**. |
| Participando por discagem | Por meio da propriedade **onlineMeeting**, acesse: <br>- **conferenceId**, **quickDial**, **phones**, **tollFreeNumbers**, **tollNumber**. |Por meio da propriedade **audioConferencing** acesse: <br> - **conferenceId**, **tollFreeNumber**, **tollNumber**.<br> - **dialinUrl** propriedade para uma página da web acessível externamente que contém informações de discagem para facilitar a integração com aplicativos de terceiros. |
| Participar de videoconferência (áudio e vídeo) | Nenhuma integração direta da API. | Utilize a propriedade **videoTeleconferenceId**. |
| Lobby da reunião e automatização da admissão de participantes na reunião online | - Nenhuma integração direta da API.<br>- No blob injetado no evento da reunião do Teams, o participante pode clicar no link **Opções da reunião** para acessar o lobby da reunião, se ativado pelo administrador. |- A API diferencia os participantes das empresa do organizador e das empresas federadas, além de outros participantes, incluindo os anônimos.  <br>- Use a propriedade **autoAdmittedUsers** (visualização).  |
| Relacionando-se a um bate-papo do Teams | Nenhuma integração direta da API. | Utilize a propriedade **chatInfo**. |