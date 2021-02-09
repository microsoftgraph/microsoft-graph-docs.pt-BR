---
title: Tipo de recurso userCredentialUsageDetails
description: Representa o uso de redefinição de senha de autoatendado para um determinado locatário.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 3992272aa6917aa43d2ffdb4c4c980b88fc60e7e
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159812"
---
# <a name="usercredentialusagedetails-resource-type"></a>Tipo de recurso userCredentialUsageDetails

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o uso de redefinição de senha de autoatendado para um determinado locatário. Os detalhes incluem informações do usuário, status da redefinição e o motivo da falha.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar userCredentialUsageDetails](../api/reportroot-list-usercredentialusagedetails.md) | userCredentialUsageDetails | Ler propriedades e relações de um objeto userCredentialUsageDetails. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| authMethod | string | Representa o método de autenticação que o usuário usou. Os valores possíveis são: , , , (usado somente para redefinição de senha de `email` `mobileSMS` `mobileCall` `officePhone` `securityQuestion` autoatendido) e (com suporte `appNotification` somente no `appCode` `alternateMobileCall` registro). |
| eventDateTime | DateTimeOffset | O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. |
| failureReason | Cadeia de caracteres | Fornece o motivo da falha para a redefinição ou o fluxo de trabalho de registro correspondente. |
| recurso | string | Os valores possíveis são: `registration` e `reset` . |
| id | String | Somente leitura. O identificador exclusivo da atividade. Somente leitura.|
| isSuccess | Boolean | Indica o sucesso ou falha do fluxo de trabalho. |
| userDisplayName | Cadeia de caracteres | Nome de usuário do usuário executando o fluxo de trabalho de redefinição ou registro. |
| userPrincipalName | String | Nome principal do usuário executando o fluxo de trabalho de redefinição ou registro. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userCredentialUsageDetails",
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

