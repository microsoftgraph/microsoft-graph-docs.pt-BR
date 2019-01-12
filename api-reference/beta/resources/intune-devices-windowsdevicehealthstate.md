---
title: tipo de enum windowsDeviceHealthState
description: Estado de proteção de ponto de extremidade do computador
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 628450b33a219e8408d5c5887c6902b78ae02bd0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923940"
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





