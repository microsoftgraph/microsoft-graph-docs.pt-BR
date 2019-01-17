---
title: tipo de enum defenderPromptForSampleSubmission
description: Valores possíveis para avisar o usuário para amostras de envio.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e103916bd55e6c2d505a85c379b80962ab9a0cac
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928084"
---
# <a name="defenderpromptforsamplesubmission-enum-type"></a>tipo de enum defenderPromptForSampleSubmission

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Valores possíveis para avisar o usuário para amostras de envio.
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|userDefined|0|Definido pelo usuário, valor padrão, sem intenção.|
|alwaysPrompt|1|Sempre avisar.|
|promptBeforeSendingPersonalData|2|Avisar antes de enviar dados pessoais.|
|neverSendData|3|Nunca envie dados.|
|sendAllDataWithoutPrompting|4|Envie todos os dados sem avisar.|



