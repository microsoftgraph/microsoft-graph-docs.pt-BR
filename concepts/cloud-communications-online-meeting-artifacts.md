---
title: Permissões e artefatos de reunião online
description: Saiba mais sobre artefatos de reunião online e o que é necessário para busca-los.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
ms.date: 09/20/2021
ms.openlocfilehash: e8c220254d0e587225c3de0f371a3dc642490345
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59777297"
---
# <a name="online-meeting-artifacts-and-permissions"></a>Permissões e artefatos de reunião online

Artefatos de reunião online são conteúdo produzido durante a duração de uma reunião online ou evento ao vivo. Você pode usar a [operação Get onlineMeeting](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true) para obter os seguintes artefatos de reunião: 

- Relatório de participação de uma reunião online, na forma de uma resposta JSON. Os relatórios de presença têm as seguintes características:
  - Disponível para reuniões que não são eventos ao vivo
  - Disponível somente quando a reunião for concluída
  - Somente o organizador da reunião pode acessar
- Gravações de um evento ao vivo, na forma de um link de download que expira em 60 segundos. As gravações têm as seguintes características:
  - Disponível apenas para eventos ao vivo
  - Disponível somente quando o evento ao vivo tiver concluído
  - Somente o organizador do evento ao vivo pode acessar
- Relatório do participante de um evento ao vivo, na forma de um link de download que expira em 60 segundos. Os relatórios do participante têm as seguintes características:
  - Disponível apenas para eventos ao vivo
  - Disponível somente quando o evento ao vivo tiver concluído
  - Somente o organizador do evento ao vivo pode acessar

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
