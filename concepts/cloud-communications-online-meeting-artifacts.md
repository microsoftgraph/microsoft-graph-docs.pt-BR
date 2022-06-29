---
title: Permissões e artefatos de reunião online na API de comunicações na nuvem
description: Saiba mais sobre artefatos de reunião online, como relatórios de participação e gravações, e as permissões necessárias para busca-los usando a API de comunicações na nuvem do Microsoft Graph.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
ms.date: 09/20/2021
ms.openlocfilehash: 019e88a0d3f5fb046c94e7074644a3a01a94ae14
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66440986"
---
# <a name="online-meeting-artifacts-and-permissions"></a>Permissões e artefatos de reunião online

Artefatos de reunião online são conteúdo produzido durante uma reunião online ou evento ao vivo [do Microsoft Teams](/microsoftteams/teams-live-events/what-are-teams-live-events). Você pode usar a [operação Get onlineMeeting](/graph/api/onlinemeeting-get) para obter os seguintes artefatos de reunião:

- Relatório de participação de uma reunião online, na forma de uma resposta JSON. Os relatórios de participação têm as seguintes características:
  - Disponível para reuniões que não sejam eventos ao vivo do Teams
  - Disponível somente quando a reunião for concluída
  - Somente o organizador da reunião pode acessar
- Gravações de um evento ao vivo do Teams, na forma de um link de download que expira em 60 segundos. As gravações têm as seguintes características:
  - Disponível apenas para eventos ao vivo do Teams
  - Disponível somente quando o evento ao vivo do Teams for concluído
  - Somente o organizador de eventos ao vivo do Teams pode acessar
- Relatório de participantes de um evento ao vivo do Teams, na forma de um link de download que expira em 60 segundos. Os relatórios de participantes têm as seguintes características:
  - Disponível apenas para eventos ao vivo do Teams
  - Disponível somente quando o evento ao vivo do Teams for concluído
  - Somente o organizador de eventos ao vivo do Teams pode acessar

## <a name="permissions"></a>Permissões

As seguintes permissões estão disponíveis para gerenciar artefatos de reunião:

- Delegado (conta corporativa ou de estudante) – OnlineMeetingArtifact.Read.All
- Aplicativo – OnlineMeetingArtifact.Read.All

Somente as _permissões OnlineMeetingArtifact.Read.All_ são necessárias para buscar artefatos de reunião online. Até **15 de janeiro de 2022**, você pode usar as seguintes permissões para obter artefatos de reunião na versão beta:

- _OnlineMeeting.Read_
- _OnlineMeeting.ReadWrite_
- _OnlineMeeting.Read.All_
- _OnlineMeeting.ReadWrite.All_

Após essa data, as _permissões OnlineMeetingArtifact.Read.All_ serão necessárias para buscar artefatos de reunião; solicitações que não têm essas permissões serão rejeitadas.

## <a name="see-also"></a>Confira também

- [Visão geral da API de comunicações na nuvem](cloud-communications-concept-overview.md)