---
title: tipo de enumeração windowsDeviceHealthState
description: Estado de proteção do ponto de extremidade do computador
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c5b4c042b93271632df933892ff8296c19c0585b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528420"
---
# <a name="windowsdevicehealthstate-enum-type"></a>tipo de enumeração windowsDeviceHealthState

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

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



