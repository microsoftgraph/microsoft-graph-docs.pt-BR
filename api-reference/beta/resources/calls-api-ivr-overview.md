---
title: Cenários IVR em chamadas
description: 'Estes são os cenários de resposta de voz interativa (IVR) que as APIs de chamada no Microsoft Graph dão suporte:'
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: conceptualPageType
ms.openlocfilehash: 62872c07dcf8072a9a5e471c53950a0b77b96814
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507786"
---
# <a name="ivr-scenarios-in-calls"></a>Cenários IVR em chamadas

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Estes são os cenários de resposta de voz interativa (IVR) que as APIs de chamada no Microsoft Graph dão suporte:

- Reproduzir um prompt de áudio-por exemplo, quando uma chamada é colocada em uma fila de agente de atendimento ao cliente.
- Gravar uma resposta-por exemplo, para registrar o áudio do chamador, normalmente após ouvir um prompt com as opções.
- Inscrever-se em tons-por exemplo, quando você deseja saber quais tons de DTMF o chamador selecionou, geralmente após ouvir o prompt de áudio.
- Cancelar o processamento de mídia – por exemplo, quando você deseja cancelar qualquer operação do playPrompt ou do recordResponse que possa estar em processo.
