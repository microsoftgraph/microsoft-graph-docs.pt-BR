---
title: Tipo de enumeração complianceState
description: Estado de conformidade.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 20d0c049a8274bbedf4c618c54cdf003b9fbfb63
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66736073"
---
# <a name="compliancestate-enum-type"></a>Tipo de enumeração complianceState

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estado de conformidade.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|0|Desconhecido.|
|Compatível|1|Compatível.|
|Incompatível|2|O dispositivo não está em conformidade e está bloqueado de recursos corporativos.|
|Conflito|3|Conflito com outras regras.|
|erro|4|Erro|
|inGracePeriod|254|O dispositivo não está em conformidade, mas ainda tem acesso a recursos corporativos|
|configManager|255|Gerenciado pelo Gerenciador de Configurações|





