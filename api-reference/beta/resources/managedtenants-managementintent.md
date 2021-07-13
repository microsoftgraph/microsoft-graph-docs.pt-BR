---
title: tipo de recurso managementIntent
description: Representa metadados para uma linha de base e quais modelos de gerenciamento estão incluídos.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 7648da23e5d49a9bd2910c2ccbde7e676a1d7cd0
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401998"
---
# <a name="managementintent-resource-type"></a>tipo de recurso managementIntent

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa metadados para uma linha de base e quais modelos de gerenciamento estão incluídos.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Gerenciamento de listaIntents](../api/managedtenants-managedtenant-list-managementintents.md)|[coleção microsoft.graph.managedTenants.managementIntent](../resources/managedtenants-managementintent.md)|Obter uma lista dos [objetos managementIntent](../resources/managedtenants-managementintent.md) e suas propriedades.|
|[Obter managementIntent](../api/managedtenants-managementintent-get.md)|[microsoft.graph.managedTenants.managementIntent](../resources/managedtenants-managementintent.md)|Leia as propriedades e as relações de um [objeto managementIntent.](../resources/managedtenants-managementintent.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|O nome de exibição para a intenção de gerenciamento. Opcional. Somente leitura.|
|id|Cadeia de caracteres|O identificador exclusivo para a intenção de gerenciamento. Obrigatório. Somente leitura.|
|isGlobal|Boolean|Um sinalizador que indica se a intenção de gerenciamento é global. Obrigatório. Somente leitura.|
|managementTemplates|[coleção microsoft.graph.managedTenants.managementTemplateDetailedInfo](../resources/managedtenants-managementtemplatedetailedinfo.md)|A coleção de modelos de gerenciamento associados à intenção de gerenciamento. Opcional. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.managementIntent",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementIntent",
  "id": "String (identifier)",
  "displayName": "String",
  "isGlobal": "Boolean",
  "managementTemplates": [
    {
      "@odata.type": "microsoft.graph.managedTenants.managementTemplateDetailedInfo"
    }
  ]
}
```
