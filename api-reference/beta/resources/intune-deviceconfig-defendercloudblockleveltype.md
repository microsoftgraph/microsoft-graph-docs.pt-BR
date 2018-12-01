---
title: tipo de enum defenderCloudBlockLevelType
description: Valores possíveis de nível de bloco de nuvem
ms.openlocfilehash: 70e43e9659e7dd7be1d3c0a190e21d80d7b8dc41
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038649"
---
# <a name="defendercloudblockleveltype-enum-type"></a>tipo de enum defenderCloudBlockLevelType

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Valores possíveis de nível de bloco de nuvem
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|não-configuradas|0|Valor padrão, usa o padrão de bloqueio de antivírus do Windows Defender nível e fornece detecção forte sem aumentar o risco de detecção legítimos arquivos|
|high|1|Alta aplica um alto nível de detecção.|
|highPlus|2|Alta + usa o alto nível e aplica as medidas de proteção de adição|
|zeroTolerance|3|Zero tolerância bloqueia todos os executáveis desconhecidos|





