---
author: learafa
description: O recurso storagePlanInformation fornece informações sobre os planos de cota de armazenamento da unidade.
title: StoragePlanInformation
localization_priority: Normal
doc_type: resourcePageType
ms.prod: files
ms.openlocfilehash: 0000275139bef3765b7be2e44c26c5e6c12c3e73d04d52b009bfad558081202c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54163653"
---
# <a name="storageplaninformation-resource-type"></a>Tipo de recurso storagePlanInformation

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


