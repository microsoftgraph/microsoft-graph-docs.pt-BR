---
title: tipo de enum defenderCloudBlockLevelType
description: Valores possíveis de nível de bloco de nuvem
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 51ed838b6abaaf36a69230b566c01b8d496c2a70
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872069"
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





