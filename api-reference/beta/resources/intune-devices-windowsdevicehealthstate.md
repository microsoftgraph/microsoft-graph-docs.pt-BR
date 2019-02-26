---
title: tipo de enumeração windowsDeviceHealthState
description: Estado de proteção do ponto de extremidade do computador
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bb335cd39e6cbcd00f754faae8f7784001c424b4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156165"
---
# <a name="windowsdevicehealthstate-enum-type"></a>tipo de enumeração windowsDeviceHealthState

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estado de proteção do ponto de extremidade do computador

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|clean|,0|O computador está limpo e nenhuma ação é necessária|
|fullScanPending|1|O computador está em estado de verificação completa pendente|
|rebootPending|duas|O computador está em estado de reinicialização pendente|
|manualStepsPending|quatro|O computador está em estado de etapas manuais pendentes|
|offlineScanPending|8|O computador está em estado de verificação offline pendente|
|muito|dezesseis|O computador está em um estado de falha crítico|




