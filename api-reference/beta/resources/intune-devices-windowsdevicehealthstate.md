---
title: tipo de enumeração windowsDeviceHealthState
description: Estado de proteção do ponto de extremidade do computador
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7da8a7cc01cef7ff410611e819739e226a4baee1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549475"
---
# <a name="windowsdevicehealthstate-enum-type"></a>tipo de enumeração windowsDeviceHealthState

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estado de proteção do ponto de extremidade do computador

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|ordena|,0|O computador está limpo e nenhuma ação é necessária|
|fullScanPending|1 |O computador está em estado de verificação completa pendente|
|rebootPending|2 |O computador está em estado de reinicialização pendente|
|manualStepsPending|4 |O computador está em estado de etapas manuais pendentes|
|offlineScanPending|8 |O computador está em estado de verificação offline pendente|
|muito|16 |O computador está em um estado de falha crítico|





