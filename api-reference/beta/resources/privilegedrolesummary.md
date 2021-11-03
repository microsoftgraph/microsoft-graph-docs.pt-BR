---
title: Tipo de recurso privilegedRoleSummary
description: O resumo de estatísticas para uma função específica.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: carolinetempleton
ms.openlocfilehash: e65179dcbccd6651bbfe51a314ea15a12a57da58
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60694147"
---
# <a name="privilegedrolesummary-resource-type"></a>Tipo de recurso privilegedRoleSummary

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O resumo de estatísticas para uma função específica.


## <a name="methods"></a>Methods

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get privilegedRoleSummary](../api/privilegedrolesummary-get.md) | [privilegedRoleSummary](privilegedrolesummary.md) |Ler propriedades e relações do objeto privilegedRoleSummary.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|elevatedCount|int32|O número de usuários que têm a função atribuída e a função é ativada.|
|id|cadeia de caracteres| O identificador exclusivo da função. Somente leitura.|
|managedCount|int32|O número de usuários que têm a função atribuída, mas a função é desativada.|
|mfaEnabled|booliano|`true` se a ativação de função exigir MFA. `false` se a ativação de função não exigir MFA.|
|status|roleSummaryStatus| Os valores possíveis são: `ok` e `bad`. O valor depende da taxa de (managedCount /usersCount). Se a taxa for menor que um limite predefinido, `ok` será retornado. Caso contrário, `bad` será retornado.|
|usersCount|int32|O número de usuários atribuídos à função.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRoleSummary"
}-->

```json
{
  "elevatedCount": 1024,
  "id": "string (identifier)",
  "managedCount": 1024,
  "mfaEnabled": true,
  "status": "string",
  "usersCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


