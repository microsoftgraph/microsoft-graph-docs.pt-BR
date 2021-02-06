---
title: Tipo de recurso onPremisesProvisioningError
description: Representa erros de sincronização de diretório para as entidades de usuário, grupo ou contato organizacional ao sincronizar diretórios locais com o Azure Active Directory.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: japere
ms.openlocfilehash: e4e3469ae371568ac9010d1d3879f68c92340460
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133975"
---
# <a name="onpremisesprovisioningerror-resource-type"></a>Tipo de recurso onPremisesProvisioningError

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa erros de sincronização de [](group.md)diretório [](orgcontact.md) para o [usuário,](user.md)grupo ou entidades de contato organizacional ao sincronizar diretórios locais com o Azure Active Directory.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|category|String| Categoria do erro de provisionamento. Observação: Atualmente, há apenas um valor possível. Valor possível: *PropertyConflict* – indica que um valor de propriedade não é exclusivo. Outros objetos contêm o mesmo valor para a propriedade. |
|occurredDateTime|DateTimeOffset| A data e a hora em que o erro ocorreu. |
|propertyCausingError|String| Nome da propriedade de diretório que está causando o erro. Valores atuais possíveis: *UserPrincipalName* ou *ProxyAddress* |
|value|Cadeia de caracteres| Valor da propriedade que está causando o erro. |

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
<!--
{
  "type": "#page.annotation",
  "description": "onPremisesProvisioningError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


