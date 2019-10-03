---
title: tipo de enumeração defenderCloudBlockLevelType
description: Possíveis valores de nível de bloco de nuvem
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 658a484a29ebed8cb111ded81ef439a560c87ac0
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37366626"
---
# <a name="defendercloudblockleveltype-enum-type"></a>tipo de enumeração defenderCloudBlockLevelType

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Possíveis valores de nível de bloco de nuvem

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notConfigured|,0|O valor padrão usa o nível de bloqueio antivírus padrão do Windows Defender e fornece uma detecção forte sem aumentar o risco de detectar arquivos legítimos|
|high|1|Alto aplica um nível forte de detecção.|
|highPlus|duas|High + usa o alto nível e aplica medidas de proteção de adição|
|zeroTolerance|3D|Tolerância zero bloqueia todos os executáveis desconhecidos|




