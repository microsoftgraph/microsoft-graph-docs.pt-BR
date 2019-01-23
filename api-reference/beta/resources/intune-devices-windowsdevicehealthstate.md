---
title: tipo de enum windowsDeviceHealthState
description: Estado de proteção de ponto de extremidade do computador
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2d971de9b20780bb51a19c3417384a0ca0563452
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416346"
---
# <a name="windowsdevicehealthstate-enum-type"></a>tipo de enum windowsDeviceHealthState

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Estado de proteção de ponto de extremidade do computador

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|clean|0|Computador é limpa e nenhuma ação é necessária|
|fullScanPending|1|Computador está pendente estado de verificação completa|
|rebootPending|2|Computador está pendente estado de reinicialização|
|manualStepsPending|4|Computador está pendente estado etapas manuais|
|offlineScanPending|8|Computador está pendente estado de verificação offline|
|crítico|16|Computador estiver em estado de falha grave|




