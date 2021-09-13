---
title: Tipo denum defenderAttackSurfaceType
description: Valores possíveis de Regras de Redução de Superfície de Ataque do Defender
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: bcb68a1c52389a47cabada211cca98975b24b347
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59033732"
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
|block|1|Habilita a regra de redução de superfície de ataque.|
|auditMode|2|Avalie como a regra ASR afetaria sua organização se estiver habilitada. Não altera a funcionalidade, mas gera logs.|
|warn|6 |Mensagem de aviso para o usuário final com capacidade de ignorar o bloco da regra de redução de superfície de ataque.|
|desabilitar|99|Desabilitar a regra de redução de superfície de ataque|



