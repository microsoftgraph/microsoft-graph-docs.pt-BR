---
title: tipo de enum windowsDeviceHealthState
description: Estado de proteção de ponto de extremidade do computador
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 91869502d0d61c25c6eb8dd67ba4e8e32d28fbb2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885922"
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





