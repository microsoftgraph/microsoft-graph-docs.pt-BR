---
title: tipo de enumeração windowsDeviceHealthState
description: Estado de proteção do ponto de extremidade do computador
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 69d20e06ba23390ff912251bb99980c4a945704c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783708"
---
# <a name="windowsdevicehealthstate-enum-type"></a>tipo de enumeração windowsDeviceHealthState

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estado de proteção do ponto de extremidade do computador

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|ordena|,0|O computador está limpo e nenhuma ação é necessária|
|fullScanPending|1|O computador está em estado de verificação completa pendente|
|rebootPending|duas|O computador está em estado de reinicialização pendente|
|manualStepsPending|4 |O computador está em estado de etapas manuais pendentes|
|offlineScanPending|8 |O computador está em estado de verificação offline pendente|
|muito|16 |O computador está em um estado de falha crítico|



