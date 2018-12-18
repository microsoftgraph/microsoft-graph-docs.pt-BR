---
title: tipo de enum complianceState
description: Estado de conformidade.
author: tfitzmac
ms.openlocfilehash: 3fa0548c2a67aa5def5f859014f52e97bdda815b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321228"
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





