---
title: Tipo de recurso acl
description: Uma entrada de controle de acesso para um item indexado por um Pesquisa da Microsoft externalConnection.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 171b53adc815638546bbdf71411c58d293c05de4
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467204"
---
# <a name="acl-resource-type"></a>Tipo de recurso acl

Namespace: microsoft.graph.externalConnectors

Uma entrada de controle de acesso para um item indexado por um Pesquisa da Microsoft externalConnection.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|accessType|microsoft.graph.externalConnectors.accessType|O acesso concedido à identidade. Os valores possíveis são: `grant`, `deny`, `unknownFutureValue`.|
|tipo|microsoft.graph.externalConnectors.aclType|O tipo de identidade. Os possíveis valores são: `user`, `group`, `everyone`, `everyoneExceptGuests`, `externalGroup`, `unknownFutureValue`.|
|value|Cadeia de caracteres|O identificador exclusivo da identidade. No caso de Azure Active Directory identidades, é definido como o identificador de objeto do usuário, grupo ou locatário para tipos de usuário, grupo e todos `value` (e todosExceptGuests), respectivamente. No caso de grupos `value` externos ser definido como a ID do externalGroup |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.externalConnectors.acl"
}
-->
``` json
{
  "type": "String",
  "value": "String",
  "accessType": "String"
}
```

