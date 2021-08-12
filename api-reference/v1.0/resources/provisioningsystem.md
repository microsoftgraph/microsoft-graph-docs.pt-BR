---
title: Tipo de recurso provisioningSystem
description: Representa o sistema de onde um usuário foi provisionado.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 4676a5010b71b7bec5ab01350bb84a69b9dd00158c6622bf208e82a479fab868
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54184512"
---
# <a name="provisioningsystem-resource-type"></a>Tipo de recurso provisioningSystem

Namespace: microsoft.graph


Representa o sistema de onde um usuário foi provisionado. Por exemplo, ao provisionar um usuário do Azure Active Directory (Azure AD) para ServiceNow, o sistema de origem é o Azure AD e o sistema de destino é ServiceNow.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|detalhes|[detailsInfo](detailsinfo.md)|Detalhes do sistema.|
|displayName|Cadeia de caracteres|Nome do sistema de onde um usuário foi provisionado.|
|id|Cadeia de caracteres|Identificador do sistema de onde um usuário foi provisionado.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningSystem",
  "baseType": null
}-->

```json
{
  "details": {"@odata.type": "microsoft.graph.detailsInfo"},
  "displayName": "String",
  "id": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisioningSystem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


