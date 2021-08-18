---
title: Tipo denum defenderCloudBlockLevelType
description: Valores possíveis do Nível de Bloqueio na Nuvem
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 807dccf28eb0c3de713f36dafcfc753405f069cceb45ff3351278f59e8ef8bc3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54226424"
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
|high|1 |Alto aplica um nível forte de detecção.|
|highPlus|2|High + usa o nível Alto e aplica medidas de proteção de adição|
|zeroTolerance|3 |Tolerância zero bloqueia todos os executáveis desconhecidos|




