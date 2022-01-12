---
title: Tipo de recurso managementTemplateDetailedInfo
description: Representa informações detalhadas para o modelo de gerenciamento.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 7ece5863f33f447a6e79ea75e1959ea7011b0c32
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61861348"
---
# <a name="managementtemplatedetailedinfo-resource-type"></a>Tipo de recurso managementTemplateDetailedInfo

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações detalhadas para o modelo de gerenciamento.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Ferramentas para desenvolvedores|managementCategory|A categoria de gerenciamento do modelo de gerenciamento. Os valores possíveis são: `custom`, `devices`, `identity`, `unknownFutureValue`. Obrigatório. Somente leitura.|
|displayName|String|O nome de exibição do modelo de gerenciamento. Obrigatório. Somente leitura.|
|managementTemplateId|String|O identificador exclusivo do modelo de gerenciamento. Obrigatório. Somente leitura.|

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
