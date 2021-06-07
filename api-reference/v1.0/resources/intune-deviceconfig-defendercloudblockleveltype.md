---
title: Tipo denum defenderCloudBlockLevelType
description: Valores possíveis do Nível de Bloqueio na Nuvem
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: edc8f58be9c9bfdce904988503b42e20ed2d0bfb
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755886"
---
# <a name="defendercloudblockleveltype-enum-type"></a>Tipo denum defenderCloudBlockLevelType

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis do Nível de Bloqueio na Nuvem

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notConfigured|0|Valor padrão, usa o nível de bloqueio padrão Windows Defender Antivírus e fornece uma detecção forte sem aumentar o risco de detectar arquivos legítimos|
|high|1|Alto aplica um nível forte de detecção.|
|highPlus|2|High + usa o nível Alto e aplica medidas de proteção de adição|
|zeroTolerance|3|Tolerância zero bloqueia todos os executáveis desconhecidos|




