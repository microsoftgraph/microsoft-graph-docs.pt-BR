---
title: tipo de enumeração defenderCloudBlockLevelType
description: Possíveis valores de nível de bloco de nuvem
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 928a39e25a02286159ba886bed9c1415b038edbf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001786"
---
# <a name="defendercloudblockleveltype-enum-type"></a>tipo de enumeração defenderCloudBlockLevelType

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Possíveis valores de nível de bloco de nuvem

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notConfigured|,0|O valor padrão usa o nível de bloqueio antivírus padrão do Windows Defender e fornece uma detecção forte sem aumentar o risco de detectar arquivos legítimos|
|high|1|Alto aplica um nível forte de detecção.|
|highPlus|duas|High + usa o alto nível e aplica medidas de proteção de adição|
|zeroTolerance|3D|Tolerância zero bloqueia todos os executáveis desconhecidos|





