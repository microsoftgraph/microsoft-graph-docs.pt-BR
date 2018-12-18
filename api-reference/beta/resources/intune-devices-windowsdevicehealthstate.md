---
title: tipo de enum windowsDeviceHealthState
description: Estado de proteção de ponto de extremidade do computador
author: tfitzmac
ms.openlocfilehash: b794f8121132e396459f9198c644084690fe95b4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326324"
---
# <a name="windowsdevicehealthstate-enum-type"></a>tipo de enum windowsDeviceHealthState

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

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





