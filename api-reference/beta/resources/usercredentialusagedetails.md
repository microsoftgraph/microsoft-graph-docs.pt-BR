---
title: tipo de recurso userCredentialUsageDetails
description: Representa o uso de redefinição de senha de autoatendimento para um determinado locatário.
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: cd71091293041d84f0f2c1d5436999fa5793037b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519530"
---
# <a name="usercredentialusagedetails-resource-type"></a>tipo de recurso userCredentialUsageDetails

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o uso de redefinição de senha de autoatendimento para um determinado locatário. Os detalhes incluem informações do usuário, status da redefinição e o motivo da falha.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar userCredentialUsageDetails](../api/reportroot-list-usercredentialusagedetails.md) | userCredentialUsageDetails | Ler propriedades e relações de um objeto userCredentialUsageDetails. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| authMethod | string | Representa o método de autenticação usado pelo usuário. Os valores possíveis são `email`: `mobileSMS`, `mobileCall`, `officePhone`, `securityQuestion` , (usado somente para redefinição de senha de autoatendimento `appCode`), `alternateMobileCall` `appNotification`e (somente para o registro). |
| eventDateTime | DateTimeOffset | O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. |
| failureReason | Cadeia de caracteres | Fornece o motivo da falha para o fluxo de trabalho de redefinição ou registro correspondente. |
| apresentam | string | Os valores possíveis são `registration` : `reset`e. |
| id | String | Somente leitura. O identificador exclusivo da atividade. Somente leitura.|
| IsSuccess | Boolean | Indica êxito ou falha do fluxo de trabalho. |
| userDisplayName | String | Nome de usuário do usuário que está executando o fluxo de trabalho de redefinição ou registro. |
| userPrincipalName | String | Nome principal do usuário que está executando o fluxo de trabalho de redefinição ou registro. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userCredentialUsageDetails",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id" : "String",
  "feature":"string",
  "userPrincipalName":"String",
  "userDisplayName": "String",
  "isSuccess" : true,
  "authMethod": "string",
  "failureReason": "String",
  "eventDateTime" : "DateTimeOffset"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userCredentialUsageDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->