---
title: tipo de recurso de onPremisesProvisioningError
description: Representa os erros de sincronização de diretório para as entidades de usuário e grupo durante a sincronização de diretórios no local com o Windows Azure Active Directory.
localization_priority: Normal
ms.openlocfilehash: c8989a78dfb60a6c7c25a66a9f1e619dcbdca15d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830664"
---
# <a name="onpremisesprovisioningerror-resource-type"></a>tipo de recurso de onPremisesProvisioningError

Representa os erros de sincronização de diretório para as entidades de [usuário](user.md) e [grupo](group.md) quando a sincronização local diretórios no Windows Azure Active Directory.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|Ferramentas para desenvolvedores|Cadeia de caracteres| Categoria do erro provisionamento. Observação: No momento, há apenas um valor possível. Valores possíveis: *PropertyConflict* - indica um valor de propriedade não é exclusivo. Outros objetos contenham o mesmo valor da propriedade. |
|occurredDateTime|DateTimeOffset| A data e hora em que o erro ocorreu. |
|propertyCausingError|Cadeia de caracteres| Nome da propriedade diretório que causou o erro. Valores possíveis atuais: *UserPrincipalName* ou *ProxyAddress* |
|valor|Cadeia de caracteres| Valor da propriedade que causou o erro. |

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesProvisioningError"
}-->

```json
{
  "category": "String",
  "occurredDateTime": "String (timestamp)",
  "propertyCausingError": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesProvisioningError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
