---
title: tipo de recurso credentialUsageSummary
description: Representa o estado atual de quantos usuários da sua organização estão usando recursos de redefinição de senha de autoatendimento.
localization_priority: Normal
author: besiler
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 9807e333fd13443462d2d3237150820afd254baa
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523144"
---
# <a name="credentialusagesummary-resource-type"></a>tipo de recurso credentialUsageSummary

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o estado atual de quantos usuários da sua organização estão usando recursos de redefinição de senha de autoatendimento.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [getCredentialUsageSummary](../api/reportroot-getcredentialusagesummary.md) | credentialUsageSummary | Ler propriedades e relações de um objeto credentialUsageSummary. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| authMethod | cadeia de caracteres | Representa o método de autenticação usado pelo usuário. Os valores possíveis são: `email` , `mobileSMS` ,, `mobileCall` `officePhone` , `securityQuestion` (usado somente para redefinição de senha de autoatendimento),, `appNotification` `appCode` e  `alternateMobileCall` (somente com suporte para registro). |
| failureActivityCount | Int64 | Fornece a contagem de redefinições ou dados de registro com falha. |
| apresentam | cadeia de caracteres | Define o recurso a ser relatado. Os valores possíveis são: `registration` e `reset` . |
| id | String | O identificador exclusivo da atividade. Somente leitura. |
| successfulActivityCount | Int64 | Fornece a contagem de registros ou redefinições bem-sucedidas. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.credentialUsageSummary",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id" : "String",
  "feature":"string",
  "successfulActivityCount":"Int64",
  "failureActivityCount": "Int64",
  "authMethod": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "credentialUsageSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

