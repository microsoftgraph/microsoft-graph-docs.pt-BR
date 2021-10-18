---
title: tipo de número de complianceState
description: Estado de conformidade.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b371969e349340264b2a3ccd81ce008a1716b0c3
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2021
ms.locfileid: "60450204"
---
# <a name="compliancestate-enum-type"></a>tipo de número de complianceState

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estado de conformidade.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|0|Desconhecido.|
|compatível|1|Compatível.|
|noncompliant|2|O dispositivo não é compatível e é bloqueado de recursos corporativos.|
|conflict|3|Conflita com outras regras.|
|erro|4 |Erro|
|inGracePeriod|254|O dispositivo não é compatível, mas ainda tem acesso a recursos corporativos|
|configManager|255|Gerenciado pelo Gerenciador de Configurações|



