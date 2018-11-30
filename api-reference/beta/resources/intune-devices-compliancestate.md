---
title: tipo de enum complianceState
description: Estado de conformidade.
ms.openlocfilehash: c49c0ecc2511f612e743fb5d86a53d150d3fbf45
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039423"
---
# <a name="compliancestate-enum-type"></a>tipo de enum complianceState

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Estado de conformidade.
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|unknown|0|Desconhecido.|
|compatível com|1|Compatível com.|
|fora de conformidade|2|Dispositivo não está em conformidade e seja bloqueado para recursos corporativos.|
|conflito|3|Conflito com outras regras.|
|erro|4|Erro|
|inGracePeriod|254|Dispositivo não está em conformidade, mas ainda tem acesso aos recursos corporativos|
|configManager|255|Gerenciado pelo Gerenciador de configuração|





