---
title: tipo de recurso agreementAcceptance
description: Representa o status atual de um usuário dentro do escopo dos termos de uso personalizáveis de uma empresa, fornecido pelo Azure Active Directory (Azure AD).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 28f3c0adccb853ac8daddca9aaad70a2c0b35e2c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508377"
---
# <a name="agreementacceptance-resource-type"></a>tipo de recurso agreementAcceptance

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o status atual de um usuário dentro do escopo dos termos de uso personalizáveis de uma empresa, fornecido pelo Azure Active Directory (Azure AD).

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementAcceptance](../api/agreementacceptance-get.md) | [agreementAcceptance](agreementacceptance.md) | Read properties and relationships of agreementAcceptance object. |
| [Update](../api/agreementacceptance-update.md) | [agreementAcceptance](agreementacceptance.md) | Update an **agreementAcceptance** object. |
| [Delete](../api/agreementacceptance-delete.md) | None | Delete an **agreementAcceptance** object. |
-->

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|agreementFileId|String|ID do arquivo de contrato aceito pelo usuário.|
|agreementid|String|ID do contrato.|
|id|String| Somente leitura.|
|recordedDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|estado|string| Os valores possíveis são: `accepted` e `declined`.|
|userDisplayName|String|Nome para exibição do usuário quando a aceitação foi registrada.|
|userEmail|Cadeia de caracteres|Email do usuário quando a aceitação foi registrada.|
|userId|String|ID do usuário que aceitou o contrato.|
|userPrincipalName|String|UPN do usuário quando a aceitação foi registrada.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementAcceptance"
}-->

```json
{
  "agreementFileId": "String",
  "agreementId": "String",
  "id": "String (identifier)",
  "recordedDateTime": "String (timestamp)",
  "state": "string",
  "userDisplayName": "String",
  "userEmail": "String",
  "userId": "String",
  "userPrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreementAcceptance resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
