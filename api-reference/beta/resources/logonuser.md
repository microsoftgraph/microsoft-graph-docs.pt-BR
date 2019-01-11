---
title: tipo de recurso de logonUser
description: Contém informações com informações de estado sobre o usuário conectado nesse host
localization_priority: Normal
ms.openlocfilehash: 3b7862555c62eb16aaceaa53d4df58541426e08a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855591"
---
# <a name="logonuser-resource-type"></a>tipo de recurso de logonUser

Contém informações com informações de estado sobre o usuário conectado nesse host

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|accountDomain|Cadeia de caracteres|Domínio da conta de usuário usada para logon.|
|accountName|Cadeia de caracteres|Nome da conta da conta de usuário usada para logon.|
|accountType|Cadeia de caracteres|Tipo de conta de usuário, por definição do Windows. Os valores possíveis são: `unknown`, `standard`, `power`, `administrator`.|
|firstSeenDateTime|DateTimeOffset|Data e hora em que o logon mais antigo por esta conta de usuário ocorreu (período determinado pelo provedor). O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|lastSeenDateTime|DateTimeOffset|Data e hora em que o logon mais recente por esta conta de usuário ocorreu. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|identificação de logon|Cadeia de caracteres|ID de logon do usuário.|
|logonTypes|String collection|Coleção dos tipos de logon observados para o usuário conectado ao primeiro ao último vistas. Os possíveis valores são: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.logonUser"
}-->

```json
{
  "accountDomain": "String",
  "accountName": "String",
  "accountType": "String",
  "firstSeenDateTime": "String (timestamp)",
  "lastSeenDateTime": "String (timestamp)",
  "logonId": "String",
  "logonTypes": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "logonUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
