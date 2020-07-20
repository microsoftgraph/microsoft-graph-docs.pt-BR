---
author: learafa
description: O recurso Adicionadostorageplaninformation fornece informações sobre os planos de cota de armazenamento da unidade.
title: Adicionadostorageplaninformation
localization_priority: Normal
doc_type: resourcePageType
ms.prod: files
ms.openlocfilehash: a5e6c10bdbc8a68230a223501844d0ee121014c2
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863772"
---
# <a name="storageplaninformation-resource-type"></a>tipo de recurso Adicionadostorageplaninformation

Namespace: microsoft.graph

Fornece informações sobre os planos de cota de armazenamento da unidade.

## <a name="properties"></a>Propriedades

| Nome da propriedade     | Tipo      | Descrição                                                             |
|:------------------|:----------|:----------------------------------------------------------------------- |
| **upgradeAvailable**  | Booliano   | Indica se há planos de cota de armazenamento mais altos disponíveis. Somente leitura. |

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
   "@odata.type": "microsoft.graph.storagePlanInformation",
} -->

```json
{
  "upgradeAvailable": true
}

```

<!--
{
  "type": "#page.annotation",
  "description": "storagePlanInformation resource contains information about storage quota plans that make up the drive's storage space quota.",
  "keywords": "quota,plans,upgradeAvailable",
  "section": "documentation",
  "tocPath": "Resources/StoragePlanInformation",
  "suppressions": []
}
-->

