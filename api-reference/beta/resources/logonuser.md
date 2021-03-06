---
title: Tipo de recurso logonUser
description: Contém informações de estado sobre o usuário conectado neste host
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 9986aaa7cb5fbf5f8687c43de019b234a4a971d8
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720491"
---
# <a name="logonuser-resource-type"></a>Tipo de recurso logonUser

Namespace: microsoft.graph

Contém informações de estado sobre o usuário conectado neste host

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|accountDomain|Cadeia de caracteres|Domínio da conta de usuário usada para fazer logon.|
|accountName|Cadeia de caracteres|Nome da conta de usuário usada para fazer logon.|
|accountType|Cadeia de caracteres|Tipo de Conta de Usuário, por definição do Windows. Os valores possíveis são: `unknown`, `standard`, `power`, `administrator`.|
|firstSeenDateTime|DateTimeOffset|DateTime no qual ocorreu o primeiro logon por essa conta de usuário (período determinado pelo provedor). O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|lastSeenDateTime|DateTimeOffset|DateTime no qual ocorreu o logon mais recente por essa conta de usuário. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|logonId|Cadeia de caracteres|ID de logon do usuário.|
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


