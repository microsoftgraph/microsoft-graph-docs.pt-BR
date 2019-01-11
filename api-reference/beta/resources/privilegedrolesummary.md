---
title: tipo de recurso de privilegedRoleSummary
description: As estatísticas de resumida de uma determinada função.
localization_priority: Normal
ms.openlocfilehash: b74b562a992f7795f3ae8e317608f1e370bc2a4e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858615"
---
# <a name="privilegedrolesummary-resource-type"></a>tipo de recurso de privilegedRoleSummary

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

As estatísticas de resumida de uma determinada função.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter privilegedRoleSummary](../api/privilegedrolesummary-get.md) | [privilegedRoleSummary](privilegedrolesummary.md) |Leia as propriedades e os relacionamentos do objeto privilegedRoleSummary.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|elevatedCount|int32|O número de usuários que possuem a função atribuída e a função está ativado.|
|id|string| O identificador exclusivo para a função. Somente leitura.|
|managedCount|int32|O número de usuários que possuem a função atribuída, mas a função é desativado.|
|mfaEnabled|booliano|**true** se a ativação de função requer MFA. **false** se a ativação de função não exige MFA.|
|status|string| Os valores possíveis são: `ok` e `bad`. O valor depende a proporção entre (managedCount / usersCount). Se a taxa for menor que um limite predefinido, `ok` é retornado. Caso contrário, `bad` é retornado.|
|usersCount|int32|O número de usuários que são atribuídos com a função.|

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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
