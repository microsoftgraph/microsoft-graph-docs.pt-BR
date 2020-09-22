---
title: tipo de recurso agreementAcceptance
description: Representa o status atual de um usuário dentro do escopo dos termos de uso personalizáveis de uma empresa, fornecido pelo Azure Active Directory (Azure AD).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: raprakasMSFT
ms.openlocfilehash: f3bad64c1cb691c5a5f5c1c5377bcb4e0188f184
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067500"
---
# <a name="agreementacceptance-resource-type"></a>tipo de recurso agreementAcceptance

Namespace: microsoft.graph

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
|agreementFileId|Cadeia de caracteres|ID do arquivo de contrato aceito pelo usuário.|
|agreementid|Cadeia de caracteres|ID do contrato.|
|deviceDisplayName|Cadeia de caracteres|O nome de exibição do dispositivo usado para aceitar o contrato.|
|deviceId|Cadeia de caracteres|O identificador exclusivo do dispositivo usado para aceitar o contrato.|
|deviceOSType|Cadeia de caracteres|O sistema operacional usado para aceitar o contrato.|
|deviceOSVersion|Cadeia de caracteres|A versão do sistema operacional do dispositivo usado para aceitar o contrato.    |
|expirationDateTime|DateTimeOffset|A data e hora da validade da aceitação. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|id|String| Somente leitura.|
|recordedDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|estado|string| Os valores possíveis são: `accepted` e `declined`.|
|userDisplayName|Cadeia de caracteres|Nome para exibição do usuário quando a aceitação foi registrada.|
|userEmail|Cadeia de caracteres|Email do usuário quando a aceitação foi registrada.|
|userId|Cadeia de caracteres|ID do usuário que aceitou o contrato.|
|userPrincipalName|Cadeia de caracteres|UPN do usuário quando a aceitação foi registrada.|

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
      "id": "String (identifier)",
      "agreementId": "String",
      "userId": "String",
      "deviceId": "String",
      "deviceDisplayName": "String",
      "deviceOSType": "String",
      "deviceOSVersion": "String",
      "agreementFileId": "String",
      "userDisplayName": "String",
      "userPrincipalName": "String",
      "userEmail": "String",
      "recordedDateTime": "String (timestamp)",
      "expirationDateTime": "String",
      "state": "String"
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


