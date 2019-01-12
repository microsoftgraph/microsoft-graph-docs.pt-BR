---
title: Cenários IVR em chamadas
description: 'Estes são os cenários de resposta de voz interativa (IVR) que oferecem suporte a APIs chamadas no Microsoft Graph:'
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a3657d60344941de931e4f77bddde922d7d01f21
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936358"
---
# <a name="ivr-scenarios-in-calls"></a>Cenários IVR em chamadas

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Estes são os cenários de resposta de voz interativa (IVR) que oferecem suporte a APIs chamadas no Microsoft Graph:

- Reproduzir um prompt de áudio - por exemplo, quando uma chamada é colocada na fila de um agente serviço de cliente.
- Registre - por exemplo, para gravar o áudio do chamador, geralmente depois que eles ouviram um prompt com opções.
- Assine o tom - por exemplo, quando você deseja saber qual DTMF toques o chamador selecionado, geralmente após ouvir o prompt de áudio.
- Cancele o processamento de mídia - por exemplo, quando você deseja cancelar qualquer operação PlayPrompt ou o registro que pode ser no processo.
