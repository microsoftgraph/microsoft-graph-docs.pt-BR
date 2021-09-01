---
title: Tipo denum defenderCloudBlockLevelType
description: Valores possíveis do Nível de Bloqueio na Nuvem
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d5f3133f21d9da39cd3cd7bd6bb34f693b85889d
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58805749"
---
# <a name="defendercloudblockleveltype-enum-type"></a>Tipo denum defenderCloudBlockLevelType

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis do Nível de Bloqueio na Nuvem

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notConfigured|0|Valor padrão, usa o nível de bloqueio padrão Windows Defender Antivírus e fornece uma detecção forte sem aumentar o risco de detectar arquivos legítimos|
|high|1|Alto aplica um nível forte de detecção.|
|highPlus|2|High + usa o nível Alto e aplica medidas de proteção de adição|
|zeroTolerance|3|Tolerância zero bloqueia todos os executáveis desconhecidos|



