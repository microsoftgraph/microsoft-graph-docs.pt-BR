---
title: Cenários IVR em chamadas
description: 'Estes são os cenários de resposta de voz interativa (IVR) que as APIs de chamada no Microsoft Graph dão suporte:'
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: conceptualPageType
ms.openlocfilehash: 561f0097eae74ca3f5d36fc18ec62aef8bcca3d6
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913503"
---
# <a name="ivr-scenarios-in-calls"></a>Cenários IVR em chamadas

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Estes são os cenários de resposta de voz interativa (IVR) que as APIs de chamada no Microsoft Graph dão suporte:

- Reproduzir um prompt de áudio-por exemplo, quando uma chamada é colocada em uma fila de agente de atendimento ao cliente.
- Gravar uma resposta-por exemplo, para registrar o áudio do chamador, normalmente após ouvir um prompt com as opções.
- Inscrever-se em tons-por exemplo, quando você deseja saber quais tons de DTMF o chamador selecionou, geralmente após ouvir o prompt de áudio.
- Cancelar o processamento de mídia – por exemplo, quando você deseja cancelar qualquer operação do playPrompt ou do recordResponse que possa estar em processo.
