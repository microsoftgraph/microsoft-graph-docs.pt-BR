---
title: Tipo de recurso managementIntentInfo
description: Representa informações de relação para uma intenção de gerenciamento.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 05442959aaa64ddc0fa1059ff599b18d421dcd7b
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61789982"
---
# <a name="managementintentinfo-resource-type"></a>Tipo de recurso managementIntentInfo

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações de relação para uma intenção de gerenciamento.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|managementIntentDisplayName|String|O nome de exibição para a intenção de gerenciamento. Opcional. Somente leitura.|
|managementIntentId|String|O identificador da intenção de gerenciamento. Obrigatório. Somente leitura.|
|managementTemplates|[coleção microsoft.graph.managedTenants.managementTemplateDetailedInfo](../resources/managedtenants-managementtemplatedetailedinfo.md)|A coleção de informações do modelo de gerenciamento associadas à intenção de gerenciamento. Opcional. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.managementIntentInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementIntentInfo",
  "managementIntentId": "String",
  "managementIntentDisplayName": "String",
  "managementTemplates": [
    {
      "@odata.type": "microsoft.graph.managedTenants.managementTemplateDetailedInfo"
    }
  ]
}
```
