---
title: Tipo de recurso logonUser
description: Contém informações com estado sobre o usuário conectado neste host
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: security
author: preetikr
ms.openlocfilehash: d665906abbbea3f49d352de5600c647f62d8bff6
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176780"
---
# <a name="logonuser-resource-type"></a>Tipo de recurso logonUser

Namespace: microsoft.graph

Contém informações com estado sobre o usuário conectado neste host

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|accountDomain|Cadeia de Caracteres|Domínio da conta de usuário usada para fazer logon.|
|Accountname|Cadeia de Caracteres|Nome da conta de usuário usada para fazer logon.|
|Accounttype|Cadeia de Caracteres|Tipo de conta de usuário, por definição Windows usuário. Os valores possíveis são: `unknown`, `standard`, `power`, `administrator`.|
|firstSeenDateTime|DateTimeOffset|DateTime em que o logon mais antigo por essa conta de usuário ocorreu (período determinado pelo provedor). O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|lastSeenDateTime|DateTimeOffset|DateTime no qual ocorreu o logon mais recente por essa conta de usuário. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|logonId|Cadeia de Caracteres|ID de logon do usuário.|
|logonTypes|Coleção de cadeias de caracteres|Coleção dos tipos de logon observados para o usuário conectado de quando foi visto pela primeira vez. Os possíveis valores são: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.|

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


