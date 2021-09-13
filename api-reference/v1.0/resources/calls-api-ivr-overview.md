---
title: Cenários ivr em chamadas
description: 'A seguir estão os cenários de IvR (Resposta interativa de Voz) que as APIs de chamada no Microsoft Graph suportam:'
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: conceptualPageType
ms.openlocfilehash: d8b08455e417b228fa22faf6083f721d342ee7ed
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59053136"
---
# <a name="ivr-scenarios-in-calls"></a>Cenários ivr em chamadas

Namespace: microsoft.graph

A seguir estão os cenários de IvR (Resposta interativa de Voz) que as APIs de chamada no Microsoft Graph suportam:

- Reprodução de um prompt de áudio - por exemplo, quando uma chamada é feita na fila de um agente de atendimento ao cliente.
- Gravando uma resposta - por exemplo, para gravar o áudio do chamador, geralmente depois de ouvir um prompt com opções.
- Assinatura de tons - por exemplo, quando você deseja saber o que a DTMF faz o chamador selecionado, geralmente depois de ouvir o prompt de áudio.
- Cancelar o processamento de mídia - por exemplo, quando você deseja cancelar qualquer operação playPrompt ou recordResponse que possa estar em processo.
