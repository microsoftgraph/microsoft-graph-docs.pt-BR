---
title: tipo de enumeração ManagementState
description: Estado de gerenciamento do dispositivo no Microsoft Intune.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0ce5fc93bfd48d4beaccac1552573c228f1e6f09
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725439"
---
# <a name="managementstate-enum-type"></a>tipo de enumeração ManagementState

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estado de gerenciamento do dispositivo no Microsoft Intune.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|Managed|,0|O dispositivo está sob gerenciamento|
|retirePending|1|Um comando de desativação está ocorrendo no dispositivo e no processo de cancelamento de registro de gerenciamento|
|retireFailed|duas|Falha no comando de desativação no dispositivo|
|wipePending|3D|Um comando de apagamento está ocorrendo no dispositivo e no processo de cancelamento de registro de gerenciamento|
|wipeFailed|4 |Falha no comando apagar no dispositivo|
|íntegro|5 |O dispositivo não está íntegro.|
|deletePending|6 |Um comando delete está ocorrendo no dispositivo |
|retireIssued|7 |Um comando de retirada foi emitido para o dispositivo|
|wipeIssued|8 |Um comando de apagamento foi emitido para o dispositivo|
|wipeCanceled|9 |Um comando de apagamento para este dispositivo foi cancelado|
|retireCanceled|10 |Um comando de desativação para este dispositivo foi cancelado|
|recém-descobertas|11|O dispositivo é descoberto, mas não está totalmente inscrito.|





