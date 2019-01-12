---
title: tipo de enum complianceState
description: Estado de conformidade.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5a4f4c359665eb1a0087f64802b5e7c829002fd6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940194"
---
# <a name="compliancestate-enum-type"></a>tipo de enum complianceState

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



