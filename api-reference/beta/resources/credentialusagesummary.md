---
title: tipo de recurso credentialUsageSummary
description: Representa o estado atual de quantos usuários em sua organização estão usando recursos de redefinição de senha de autoatendados.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 9db31a0d0397f1394a342fb52796a1bec37bae36
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941821"
---
# <a name="credentialusagesummary-resource-type"></a>tipo de recurso credentialUsageSummary

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o estado atual de quantos usuários em sua organização estão usando recursos de redefinição de senha de autoatendados.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [getCredentialUsageSummary](../api/reportroot-getcredentialusagesummary.md) | credentialUsageSummary | Ler propriedades e relações de um objeto credentialUsageSummary. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| authMethod | usageAuthMethod | Representa o método de autenticação que o usuário usou. Os valores possíveis são: , , , , , (usado apenas para redefinição de senha de `email` `mobileSMS` `mobileCall` `officePhone` `securityQuestion` autoatendido), , (suportado somente `appNotification` `appCode` no `alternateMobileCall` registro), , , `fido` `appPassword` `unknownFutureValue` . |
| failureActivityCount | Int64 | Fornece a contagem de redefinições com falha ou dados de registro. |
| feature | featureType | Define o recurso a ser relatório. Os valores possíveis são: `registration`, `reset`, `unknownFutureValue`. |
| id | Cadeia de caracteres | O identificador exclusivo da atividade. Somente leitura. |
| successfulActivityCount | Int64 | Fornece a contagem de registros bem-sucedidos ou redefinições. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.credentialUsageSummary",
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

