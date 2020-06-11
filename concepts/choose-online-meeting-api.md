---
title: Escolher uma API no Microsoft Graph para criar e ingressar em reuniões online
description: Você terá a flexibilidade de criar uma reunião que ocorra no futuro ou instantaneamente
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 4d446340ff1316bdb8b760920742bc3997c6d64a
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681918"
---
# <a name="choose-an-api-in-microsoft-graph-to-create-and-join-online-meetings"></a>Escolher uma API no Microsoft Graph para criar e ingressar em reuniões online

O Microsoft Graph oferece dois conjuntos de API que organizam e participam de reuniões online no Microsoft Teams ou no Skype:

- [API de calendário](outlook-calendar-online-meetings.md): Use o recurso de [evento](/graph/api/resources/event) .
- [API de comunicações em nuvem](cloud-communications-online-meetings.md): Use o recurso [onlineMeeting](/graph/api/resources/onlineMeeting) .

A opção está entre:
- Um modo de programação conveniente de configurar uma reunião online no calendário do Outlook onde os participantes clicam para ingressar na reunião e continuar a experiência no Microsoft Teams ou no Skype.
- E uma integração programática avançada de equipes ou recursos do Skype em um aplicativo para uma experiência mais personalizada.

## <a name="considerations-when-choosing-an-api-for-your-scenario"></a>Considerações ao escolher uma API para o seu cenário

Escolha a API de calendário para uma integração integrada e simplificada com o calendário do Outlook, que resulta em um evento de reunião online no calendário do Outlook:
- Suporte de programação:
  - Os aplicativos podem _criar ou atualizar diretamente um evento como uma reunião online no calendário do Outlook_, com um blob Join-Teams-Meeting inserido no evento de calendário do Outlook.
  - Os aplicativos obtêm as propriedades para ingressar na reunião pela Internet ou discando para o.
- A experiência de interface do usuário dos participantes com o evento de calendário criado programaticamente está em paridade total com qualquer evento que tenha sido criado através da interface do usuário do Outlook:
  - Os participantes podem optar por atender online ou pessoalmente.
  - Os participantes podem clicar no blob Join-Teams-Meeting para participar da reunião pela Internet ou discando para o.
  - Os participantes podem usar outros recursos avançados do Teams, incluindo conferência de vídeo e lobby de reunião, se estiverem configurados.

> **Observação:** A integração com o calendário do Outlook presume que um administrador configurou o Outlook para reuniões online. [Verifique](/microsoftteams/exchange-teams-interact) o suporte antes de usar a API.

Escolha a API de comunicações em nuvem para flexibilidade e suporte programático mais amplo:
- Os aplicativos têm mais flexibilidade para integrar mais os resultados da API com linha de negócios e outros aplicativos. A API é desassociada a qualquer calendário específico e não cria um evento em nenhum calendário.
- Os aplicativos podem fornecer os seguintes recursos para os participantes:
  - Informações de junção baseadas em localidade.
  - Ingresso na reunião pela Internet ou discagem.
  - Vídeo de conferência.
  - Recursos de segurança adicionais, como sala de reunião e automatização de admissão de participantes (visualização).
  - Associando reuniões a um chat do Microsoft Teams.

## <a name="comparing-the-apis"></a>Comparando as APIs

A tabela a seguir detalha as diferenças no nível da API. 


| Recurso de reunião online | API de calendário (recurso de evento) | API de comunicação em nuvem (recurso onlineMeeting)             |
|:-----------------------|:------------------------------|:-------------------------------------------------------------|
| Membros da API principal | recurso de [evento](/graph/api/resources/event) : <br>- Propriedade **isOnlineMeeting** <br>- Propriedade **onlineMeeting** do tipo [onlineMeetingInfo](/graph/api/resources/onlinemeetinginfo) <br>- Propriedade **onlineMeetingProvider** <br> recurso de [calendário](/graph/api/resources/calendar) : <br>- Propriedade **allowedOnlineMeetingProviders** <br>- Propriedade **defaultOnlineMeetingProvider** <br> | recurso [onlineMeeting](/graph/api/resources/onlinemeeting) <br> recurso [audioConferencing](/graph/api/resources/audioconferencing)
| Integração com um item de calendário | <br>- [Criar](/graph/api/user-post-events) ou [Atualizar](/graph/api/event-update) a API de **eventos** define automaticamente o [evento](/graph/api/resources/event) de calendário do Outlook resultante como uma reunião online.<br>– Use as propriedades **isOnlineMeeting**, **onlineMeeting**e **onlineMeetingProvider** do **evento**de calendário do Outlook retornado.  | - [Criar](/graph/api/application-post-onlinemeetings) API retorna um recurso [onlineMeeting](/graph/api/resources/onlinemeeting) que é independente de um determinado tipo de calendário. <br>-Não cria ou atualiza qualquer evento do Outlook. <br>– Integre as informações de recurso **onlineMeeting** retornadas em uma experiência de aplicativo apropriada para seu cenário. <br>– Use [createOrGet](/graph/api/onlinemeeting-createorget?view=graph-rest-beta) para retornar uma reunião online que tenha um valor **externalId** especificado ou crie um se nenhum já existir, para simplificar a incorporação da reunião resultante em um calendário de terceiros. |
| Alterando para reunião offline | -Não quando você habilitar um **evento** para ingressar online, não será possível atualizá-lo para torná-lo uma reunião offline.<br>– Não é possível alterar a propriedade **onlineMeetingProvider** , nem definir **isOnlineMeeting** para `false` desabilitar a reunião online. | Não depois de criar um recurso do **onlineMeeting** , você só pode excluí-lo, mas não pode alterá-lo para uma reunião offline. |
| Informações de junção baseadas em localidade | Nenhuma integração direta da API. | – Use o `Accept-Language` cabeçalho HTTP ao criar uma reunião online. <br>– Confira o [exemplo](/graph/api/application-post-onlinemeetings?view=graph-rest-beta#example-2-create-an-online-meeting-with-user-token). |
| Ingressar na Internet (VoIP) | Por meio da propriedade **onlineMeeting** , acesse **joinUrl**.  | Use a propriedade **joinWebUrl** . |
| Ingressando por discagem | Por meio da propriedade **onlineMeeting** , acesse: <br>- **conferenceid**, **quickDial**, **telefones**, **tollFreeNumbers**, **tollNumber**. |Por meio da propriedade **audioConferencing** , acesse: <br> - **conferenceid**, **tollFreeNumber**, **tollNumber**.<br> - Propriedade **dialinUrl** para uma página da Web acessível externamente que contém informações de discagem para facilitar a integração com aplicativos de terceiros. |
| Ingressar por vídeo audioconferência (áudio e vídeo) | Nenhuma integração direta da API. | Use a propriedade **videoTeleconferenceId** . |
| Reunião de reuniões e automatização de admissão de participantes na reunião online | -Nenhuma integração direta da API.<br>-No blob de reunião de ingresso injetado-Teams do evento, o participante pode clicar em um link de **Opções de reunião** para acessar o lobby da reunião, se habilitado pelo administrador. |-API diferencia os participantes da empresa e das empresas federadas do organizador e outros participantes, incluindo aqueles anônimos.  <br>– Use a propriedade **autoAdmittedUsers** (visualização).  |
| Relacionadas a um chat do Microsoft Teams | Nenhuma integração direta da API. | Use a propriedade **chatInfo** . |


## <a name="see-also"></a>Confira também
- [Use o Outlook para organizar ou participar de reuniões online](outlook-calendar-online-meetings.md)
- [Usar a API de comunicações em nuvem para criar ou ingressar em reuniões online](cloud-communications-online-meetings.md)