---
title: tipo de enumeração defenderCloudBlockLevelType
description: Possíveis valores de nível de bloco de nuvem
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: bd121a61106ae029ccacf2e393bd28ef34415045
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530897"
---
# <a name="defendercloudblockleveltype-enum-type"></a>tipo de enumeração defenderCloudBlockLevelType

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Possíveis valores de nível de bloco de nuvem

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notConfigured|,0|O valor padrão usa o nível de bloqueio antivírus padrão do Windows Defender e fornece uma detecção forte sem aumentar o risco de detectar arquivos legítimos|
|high|1 |Alto aplica um nível forte de detecção.|
|highPlus|2 |High + usa o alto nível e aplica medidas de proteção de adição|
|zeroTolerance|3 |Tolerância zero bloqueia todos os executáveis desconhecidos|




