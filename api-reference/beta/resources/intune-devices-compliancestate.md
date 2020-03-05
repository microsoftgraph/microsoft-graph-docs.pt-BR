---
title: tipo de enumeração compliancestate
description: Estado de conformidade.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 78dc7dfee02a1b1670a2259d20465d4660e73a08
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525149"
---
# <a name="compliancestate-enum-type"></a>tipo de enumeração compliancestate

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estado de conformidade.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|Unknown.|
|com|1 |Com.|
|incompatível|2 |O dispositivo não está em conformidade e é bloqueado de recursos corporativos.|
|apresentar|3 |Conflito com outras regras.|
|erro|4 |Erro|
|inGracePeriod|254|O dispositivo não está em conformidade, mas ainda tem acesso aos recursos corporativos|
|configmanager|255|Gerenciado pelo Gerenciador de configuração|



