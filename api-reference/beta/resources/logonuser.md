---
title: tipo de recurso logonUser
description: Contém informações de estado sobre o usuário conectado neste host
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: f480ff8c67c602512d7d8ef3f090366734f0ca7e
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808659"
---
# <a name="logonuser-resource-type"></a>tipo de recurso logonUser

Namespace: microsoft.graph

Contém informações de estado sobre o usuário conectado neste host

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|accountDomain|String|Domínio da conta de usuário usada para fazer logon.|
|accountName|String|Nome da conta de usuário usada para fazer logon.|
|accountType|String|Tipo de conta de usuário, por definição do Windows. Os valores possíveis são: `unknown`, `standard`, `power`, `administrator`.|
|firstSeenDateTime|DateTimeOffset|Data e hora em que o logon mais antigo por essa conta de usuário ocorreu (período determinado pelo provedor). O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|lastSeenDateTime|DateTimeOffset|DateTime no qual a conta de usuário tem o logon mais recente. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|LogonId|String|ID de logon do usuário.|
|Logontypesowner|Coleção de cadeia de caracteres|Coleção dos tipos de logon observados para o usuário conectado da primeira vez para a última vista. Os possíveis valores são: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.|

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
