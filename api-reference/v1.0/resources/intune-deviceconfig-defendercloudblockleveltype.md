---
title: tipo de enum defenderCloudBlockLevelType
description: Valores possíveis de nível de bloco de nuvem
author: tfitzmac
ms.openlocfilehash: 19c101cc82673009a39d6545f7340fabf65b287a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326611"
---
# <a name="defendercloudblockleveltype-enum-type"></a>tipo de enum defenderCloudBlockLevelType

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Valores possíveis de nível de bloco de nuvem
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|não-configuradas|0|Valor padrão, usa o padrão de bloqueio de antivírus do Windows Defender nível e fornece detecção forte sem aumentar o risco de detecção legítimos arquivos|
|high|1|Alta aplica um alto nível de detecção.|
|highPlus|2|Alta + usa o alto nível e aplica as medidas de proteção de adição|
|zeroTolerance|3|Zero tolerância bloqueia todos os executáveis desconhecidos|



