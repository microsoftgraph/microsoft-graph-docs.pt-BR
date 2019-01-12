---
title: tipo de enum defenderPromptForSampleSubmission
description: Valores possíveis para avisar o usuário para amostras de envio.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8dfc1a3aeb80a22041f799fb40ff9b2cc6e3870b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924822"
---
# <a name="defenderpromptforsamplesubmission-enum-type"></a>tipo de enum defenderPromptForSampleSubmission

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

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





