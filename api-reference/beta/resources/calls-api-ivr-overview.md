---
title: Cenários IVR em chamadas
description: 'Estes são os cenários de resposta de voz interativa (IVR) que as APIs de chamada no Microsoft Graph dão suporte:'
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: aed30bc5ad109dc3f21d381f4d6b04e087a779a3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535550"
---
# <a name="ivr-scenarios-in-calls"></a>Cenários IVR em chamadas

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Estes são os cenários de resposta de voz interativa (IVR) que as APIs de chamada no Microsoft Graph dão suporte:

- Reproduzir um prompt de áudio-por exemplo, quando uma chamada é colocada em uma fila de agente de atendimento ao cliente.
- Record-por exemplo, para registrar o áudio do chamador, normalmente depois de ouvir um prompt com as opções.
- Assine o Tom por exemplo, quando você deseja saber quais tons de DTMF o chamador selecionou, geralmente após ouvir o prompt de áudio.
- Cancelar o processamento de mídia – por exemplo, quando você deseja cancelar qualquer operação de PlayPrompt ou registro que possa estar em andamento.
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/calls-api-ivr-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
