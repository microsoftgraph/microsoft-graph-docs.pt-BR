---
title: Tipo de recurso onPremisesProvisioningError
description: Representa erros de sincronização de diretório para o grupo de usuários e recursos de contato ao sincronizar diretórios locais com o Azure Active Directory.
localization_priority: Normal
author: japere
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 2647e32653d26793b4f875bb47ce43e83a294c4a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133327"
---
# <a name="onpremisesprovisioningerror-resource-type"></a>Tipo de recurso onPremisesProvisioningError

Namespace: microsoft.graph

Representa erros de sincronização de [](group.md) diretório para o [usuário,](user.md)grupo e [recursos orgContact](orgcontact.md) ao sincronizar diretórios locais com o Azure Active Directory.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|category|String| Categoria do erro de provisionamento. Observação: Atualmente, há apenas um valor possível. Valor possível: *PropertyConflict* – indica que um valor de propriedade não é exclusivo. Outros objetos contêm o mesmo valor para a propriedade. |
|occurredDateTime|DateTimeOffset| A data e a hora em que o erro ocorreu. |
|propertyCausingError|String| Nome da propriedade do diretório que está causando o erro. Valores atuais possíveis: *UserPrincipalName* ou *ProxyAddress* |
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
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesProvisioningError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

