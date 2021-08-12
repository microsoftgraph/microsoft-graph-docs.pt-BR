---
title: tipo de número de complianceState
description: Estado de conformidade.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d2b33b8d82f3b6683617247c702219928c2ff2fde7f9fdd73f7b193325e432ae
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54218580"
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




