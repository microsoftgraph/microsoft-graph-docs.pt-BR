---
title: Tipo denum defenderCloudBlockLevelType
description: Valores possíveis do Nível de Bloqueio na Nuvem
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f5c600eceaa5f19ab9358906cd6c85f1226e0ad3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59033725"
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



