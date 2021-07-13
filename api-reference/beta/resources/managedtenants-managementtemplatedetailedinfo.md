---
title: Tipo de recurso managementTemplateDetailedInfo
description: Representa informações detalhadas para o modelo de gerenciamento.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: e98d2ca41bc972a5dca33c575363b1bac27d87a5
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402107"
---
# <a name="managementtemplatedetailedinfo-resource-type"></a>Tipo de recurso managementTemplateDetailedInfo

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações detalhadas para o modelo de gerenciamento.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Ferramentas para desenvolvedores|managementCategory|A categoria de gerenciamento do modelo de gerenciamento. Os valores possíveis são: `custom`, `devices`, `identity`, `unknownFutureValue`. Obrigatório. Somente leitura.|
|displayName|Cadeia de caracteres|O nome de exibição do modelo de gerenciamento. Obrigatório. Somente leitura.|
|managementTemplateId|Cadeia de caracteres|O identificador exclusivo do modelo de gerenciamento. Obrigatório. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.managementTemplateDetailedInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementTemplateDetailedInfo",
  "managementTemplateId": "String",
  "displayName": "String",
  "category": "String"
}
```
