---
title: Permissões e artefatos de reunião online
description: Saiba mais sobre artefatos de reunião online e o que é necessário para busca-los.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
ms.date: 09/20/2021
ms.openlocfilehash: 59d5bca4e8484d7965eeef44e44c08b7c67b09fb
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60685524"
---
# <a name="online-meeting-artifacts-and-permissions"></a>Permissões e artefatos de reunião online

Artefatos de reunião online são conteúdo produzido durante a duração de uma reunião online ou Microsoft Teams [evento ao vivo.](/microsoftteams/teams-live-events/what-are-teams-live-events) Você pode usar a [operação Get onlineMeeting](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true) para obter os seguintes artefatos de reunião:

- Relatório de participação de uma reunião online, na forma de uma resposta JSON. Os relatórios de presença têm as seguintes características:
  - Disponível para reuniões que não Teams eventos ao vivo
  - Disponível somente quando a reunião for concluída
  - Somente o organizador da reunião pode acessar
- Gravações de um evento Teams ao vivo, na forma de um link de download que expira em 60 segundos. As gravações têm as seguintes características:
  - Disponível somente para eventos Teams ao vivo
  - Disponível somente quando o evento Teams ao vivo tiver concluído
  - Somente o Teams organizador de eventos ao vivo pode acessar
- Relatório do participante de um evento Teams ao vivo, na forma de um link de download que expira em 60 segundos. Os relatórios do participante têm as seguintes características:
  - Disponível somente para eventos Teams ao vivo
  - Disponível somente quando o evento Teams ao vivo tiver concluído
  - Somente o Teams organizador de eventos ao vivo pode acessar

## <a name="permissions"></a>Permissões

As permissões a seguir estão disponíveis para gerenciar artefatos de reunião.

- Delegada (conta de trabalho ou de estudante) - OnlineMeetingArtifact.Read.All
- Aplicativo - OnlineMeetingArtifact.Read.All

Somente as _permissões OnlineMeetingArtifact.Read.All_ são necessárias para buscar artefatos de reunião online. Até **15 de janeiro de 2022**, você pode usar as seguintes permissões para obter artefatos de reunião no beta:

- _OnlineMeeting.Read_
- _OnlineMeeting.ReadWrite_
- _OnlineMeeting.Read.All_
- _OnlineMeeting.ReadWrite.All_

Após essa data, as _permissões OnlineMeetingArtifact.Read.All_ serão necessárias para buscar artefatos de reunião; solicitações que não têm essas permissões serão rejeitadas.
