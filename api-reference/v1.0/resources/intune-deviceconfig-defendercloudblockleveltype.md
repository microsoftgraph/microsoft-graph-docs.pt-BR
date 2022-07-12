---
title: Tipo de enumeração defenderCloudBlockLevelType
description: Valores possíveis do nível de bloco de nuvem
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 14b991b0b00541306a47c56f8c2914c68bff07e4
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66734351"
---
# <a name="defendercloudblockleveltype-enum-type"></a>Tipo de enumeração defenderCloudBlockLevelType

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis do nível de bloco de nuvem

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notConfigured|0|Valor padrão, usa o nível de Windows Defender Antivírus padrão e fornece detecção forte sem aumentar o risco de detectar arquivos legítimos|
|high|1|Alta aplica-se a um nível forte de detecção.|
|highPlus|2|Alto + usa o alto nível e aplica medidas de proteção de adição|
|zeroTolerance|3|A tolerância zero bloqueia todos os executáveis desconhecidos|





