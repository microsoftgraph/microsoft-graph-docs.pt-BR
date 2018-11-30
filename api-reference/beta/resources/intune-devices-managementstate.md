---
title: tipo de enum managementState
description: Estado de gerenciamento de dispositivo no Microsoft Intune.
ms.openlocfilehash: 554e06ff32102285d4851a19350c7c44d11d1fb4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039215"
---
# <a name="managementstate-enum-type"></a>tipo de enum managementState

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Estado de gerenciamento de dispositivo no Microsoft Intune.
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|gerenciados|0|O dispositivo está sob gerenciamento|
|retirePending|1|Um comando de aposentadoria está ocorrendo no dispositivo e no processo de unenrolling de gerenciamento|
|retireFailed|2|Desative o comando falha no dispositivo|
|wipePending|3|Um comando de apagamento está ocorrendo no dispositivo e no processo de unenrolling de gerenciamento|
|wipeFailed|4|Falha do comando de apagamento do dispositivo|
|não íntegro|5|O dispositivo não está íntegro.|
|deletePending|6|Um comando Excluir está ocorrendo no dispositivo |
|retireIssued|7|Um comando de aposentadoria foi emitido para o dispositivo|
|wipeIssued|8|Foi emitido um comando de apagamento do dispositivo|
|wipeCanceled|9|Um comando de apagamento para este dispositivo foi cancelado|
|retireCanceled|10|Um comando de aposentadoria para este dispositivo foi cancelado|
|descoberto|11|O dispositivo é descoberto, mas não totalmente registrado.|





