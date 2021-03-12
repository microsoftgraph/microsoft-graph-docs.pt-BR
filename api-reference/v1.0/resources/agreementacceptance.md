---
title: Tipo de recurso agreementAcceptance
description: Representa o status atual de um usuário dentro do escopo dos termos de uso personalizáveis de uma empresa com o Azure Active Directory (Azure AD).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: ac0e6d67e10e7d7b81fc1c5c21e93251f84cab0a
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722555"
---
# <a name="agreementacceptance-resource-type"></a>Tipo de recurso agreementAcceptance

Namespace: microsoft.graph

Representa o status atual de um usuário dentro do escopo dos termos de uso personalizáveis de uma empresa com o Azure Active Directory (Azure AD).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|agreementFileId|Cadeia de caracteres|O identificador do arquivo de contrato aceito pelo usuário.|
|agreementId|Cadeia de caracteres|O identificador do contrato.|
|deviceDisplayName|Cadeia de caracteres|O nome de exibição do dispositivo usado para aceitar o contrato.|
|deviceId|Cadeia de caracteres|O identificador exclusivo do dispositivo usado para aceitar o contrato.|
|deviceOSType|Cadeia de caracteres|O sistema operacional usado para aceitar o contrato.|
|deviceOSVersion|Cadeia de caracteres|A versão do sistema operacional do dispositivo usado para aceitar o contrato.    |
|expirationDateTime|DateTimeOffset|A data de expiração da aceitação. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|id|Cadeia de caracteres| O identificador da aceitação do contrato. Somente leitura.|
|recordedDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|estado|string| O estado da aceitação do contrato. Os valores possíveis são: `accepted` e `declined`.|
|userDisplayName|Cadeia de caracteres|Nome de exibição do usuário quando a aceitação foi registrada.|
|userEmail|Cadeia de caracteres|Email do usuário quando a aceitação foi registrada.|
|userId|Cadeia de caracteres|O identificador do usuário que aceitou o contrato.|
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


