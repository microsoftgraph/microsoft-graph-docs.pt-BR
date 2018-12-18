---
title: tipo de enum managementState
description: Estado de gerenciamento de dispositivo no Microsoft Intune.
author: tfitzmac
ms.openlocfilehash: 530c1fec4effeb83f6efb635cd44995d904dbdcf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361058"
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





