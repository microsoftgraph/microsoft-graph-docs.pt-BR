---
title: tipo de enumeração ManagementState
description: Estado de gerenciamento do dispositivo no Microsoft Intune.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7ceb46d11042c0e6d879bf0708a5f64807ce5fe3
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941855"
---
# <a name="managementstate-enum-type"></a>tipo de enumeração ManagementState

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estado de gerenciamento do dispositivo no Microsoft Intune.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|Managed|,0|O dispositivo está sob gerenciamento|
|retirePending|1|Um comando de desativação está ocorrendo no dispositivo e no processo de cancelamento de registro de gerenciamento|
|retireFailed|duas|Falha no comando de desativação no dispositivo|
|wipePending|3D|Um comando de apagamento está ocorrendo no dispositivo e no processo de cancelamento de registro de gerenciamento|
|wipeFailed|quatro|Falha no comando apagar no dispositivo|
|íntegro|0,5|O dispositivo não está íntegro.|
|deletePending|6|Um comando delete está ocorrendo no dispositivo |
|retireIssued|178|Um comando de retirada foi emitido para o dispositivo|
|wipeIssued|8 |Um comando de apagamento foi emitido para o dispositivo|
|wipeCanceled|9 |Um comando de apagamento para este dispositivo foi cancelado|
|retireCanceled|10 |Um comando de desativação para este dispositivo foi cancelado|
|recém-descobertas|11|O dispositivo é descoberto, mas não está totalmente inscrito.|




