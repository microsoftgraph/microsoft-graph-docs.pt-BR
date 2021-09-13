---
title: Tipo de recurso onPremisesProvisioningError
description: Representa erros de sincronização de diretório para o grupo de usuários e recursos de contato ao sincronizar diretórios locais com Azure Active Directory.
ms.localizationpriority: medium
author: japere
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 9f95b454b37913c407e949cc76cd01e48299e785
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59071991"
---
# <a name="onpremisesprovisioningerror-resource-type"></a>Tipo de recurso onPremisesProvisioningError

Namespace: microsoft.graph

Representa erros de sincronização de diretório para os recursos [user](user.md), [group](group.md) e [orgContact](orgcontact.md) ao sincronizar diretórios locais com Azure Active Directory.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|category|Cadeia de caracteres| Categoria do erro de provisionamento. Observação: Atualmente, há apenas um valor possível. Valor possível: *PropertyConflict* - indica que um valor de propriedade não é exclusivo. Outros objetos contêm o mesmo valor para a propriedade. |
|occurredDateTime|DateTimeOffset| A data e a hora em que o erro ocorreu. |
|propertyCausingError|Cadeia de caracteres| Nome da propriedade directory causando o erro. Valores possíveis atuais: *UserPrincipalName* ou *ProxyAddress* |
|value|Cadeia de caracteres| Valor da propriedade que causa o erro. |

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

