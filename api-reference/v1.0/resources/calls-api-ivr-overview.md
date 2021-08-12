---
title: Cenários ivr em chamadas
description: 'A seguir estão os cenários de IvR (Resposta interativa de Voz) que as APIs de chamada no Microsoft Graph suportam:'
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: conceptualPageType
ms.openlocfilehash: cbf46e81d537c704e6225a6d756140dd3ce8221fc70a7e86f188cead4ec9d3e2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54238185"
---
# <a name="ivr-scenarios-in-calls"></a>Cenários ivr em chamadas

Namespace: microsoft.graph

A seguir estão os cenários de IvR (Resposta interativa de Voz) que as APIs de chamada no Microsoft Graph suportam:

- Reprodução de um prompt de áudio - por exemplo, quando uma chamada é feita na fila de um agente de atendimento ao cliente.
- Gravando uma resposta - por exemplo, para gravar o áudio do chamador, geralmente depois de ouvir um prompt com opções.
- Assinatura de tons - por exemplo, quando você deseja saber o que a DTMF faz o chamador selecionado, geralmente depois de ouvir o prompt de áudio.
- Cancelar o processamento de mídia - por exemplo, quando você deseja cancelar qualquer operação playPrompt ou recordResponse que possa estar em processo.
