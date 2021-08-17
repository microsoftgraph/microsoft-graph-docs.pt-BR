---
title: Tipo denum defenderAttackSurfaceType
description: Valores possíveis de Regras de Redução de Superfície de Ataque do Defender
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: fbec5597244c2cb95a3425ac6a94a07db65b14feb6389dd06542da960b8b878b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54209921"
---
# <a name="defenderattacksurfacetype-enum-type"></a>Tipo denum defenderAttackSurfaceType

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis de Regras de Redução de Superfície de Ataque do Defender

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|userDefined|0|Padrão, que desabilita a regra de redução de superfície de ataque.|
|block|1 |Habilita a regra de redução de superfície de ataque.|
|auditMode|2|Avalie como a regra ASR afetaria sua organização se estiver habilitada. Não altera a funcionalidade, mas gera logs.|
|warn|6 |Mensagem de aviso para o usuário final com capacidade de ignorar o bloco da regra de redução de superfície de ataque.|
|desabilitar|99|Desabilitar a regra de redução de superfície de ataque|




