---
title: Tipo de recurso acl
description: Uma entrada de controle de acesso para um item indexado por um Pesquisa da Microsoft externalConnection.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 339b5ab51fd604cae2dd42e2ec853ede8d27ef5b
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467573"
---
# <a name="acl-resource-type"></a>Tipo de recurso acl

Namespace: microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma entrada de controle de acesso para um item indexado por um Pesquisa da Microsoft [externalConnection](externalconnectors-externalconnection.md).

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo   | Descrição                                        |
|:---------------|:-------|:---------------------------------------------------|
| accessType     | String | O acesso concedido à identidade. Os valores possíveis são: `grant` e `deny`. |
| identitySource | String | A origem da identidade. Os valores possíveis são: `azureActiveDirectory` ou `external`.           |
| tipo           | String | O tipo de identidade. Os valores possíveis são: `user` , , , se a `group` `everyone` `everyoneExceptGuests` identitySource for `azureActiveDirectory` e apenas se a `group` identitySource for `external` . |
| value          | Cadeia de caracteres | O identificador exclusivo da identidade. No caso de Azure Active Directory identidades, é definido como o identificador de objeto do usuário, grupo ou locatário para tipos de usuário, grupo e todos `value` (e todosExceptGuests), respectivamente. No caso de grupos `value` externos ser definido como a ID do [externalGroup](externalconnectors-externalgroup.md).|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnectors.acl",
  "baseType": null
}-->

```json
{
  "accessType": "String",
  "identitySource": "String",
  "type": "String",
  "value": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "acl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
