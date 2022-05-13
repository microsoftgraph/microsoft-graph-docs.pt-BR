---
title: Tipo de recurso serviceUsage
description: Representa dados de uso ativos mensais para um serviço em um locatário gerenciado.
author: kylewirpel
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: f680af26313e38da441408f6a127b21c14a7a045
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2022
ms.locfileid: "65398946"
---
# <a name="serviceusage-resource-type"></a>Tipo de recurso serviceUsage

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa dados de uso ativos mensais para um serviço em um locatário gerenciado.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|monthlyActiveUsers|Int32|Número de usuários ativos mensais do serviço. Obrigatório. Somente leitura.|
|serviceName|Cadeia de caracteres|O nome do serviço Microsoft 365 que gerou o uso. Obrigatório. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.serviceUsage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.serviceUsage",
  "serviceName": "String",
  "monthlyActiveUsers": "Integer"
}
```

