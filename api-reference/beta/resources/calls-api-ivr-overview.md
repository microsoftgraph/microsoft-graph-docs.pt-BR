---
title: Cenários IVR em chamadas
description: 'Estes são os cenários de resposta de voz interativa (IVR) que oferecem suporte a APIs chamadas no Microsoft Graph:'
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 014fd2169678617043a5a540f625479e68302b34
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855808"
---
# <a name="ivr-scenarios-in-calls"></a>Cenários IVR em chamadas

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Estes são os cenários de resposta de voz interativa (IVR) que oferecem suporte a APIs chamadas no Microsoft Graph:

- Reproduzir um prompt de áudio - por exemplo, quando uma chamada é colocada na fila de um agente serviço de cliente.
- Registre - por exemplo, para gravar o áudio do chamador, geralmente depois que eles ouviram um prompt com opções.
- Assine o tom - por exemplo, quando você deseja saber qual DTMF toques o chamador selecionado, geralmente após ouvir o prompt de áudio.
- Cancele o processamento de mídia - por exemplo, quando você deseja cancelar qualquer operação PlayPrompt ou o registro que pode ser no processo.
