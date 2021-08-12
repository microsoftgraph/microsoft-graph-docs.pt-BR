---
title: tipo de recurso de processo
description: Contém informações de estado sobre o processo relacionado ao alerta.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 5fa15502d380d651128f55e6854bfe3592a290d1fb413b591a3f8f2571dca19f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54222711"
---
# <a name="process-resource-type"></a>tipo de recurso de processo

Namespace: microsoft.graph

Contém informações de estado sobre o processo relacionado ao alerta.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|accountName|String|Identificador de conta de usuário (contexto de conta de usuário no qual o processo foi submetido) por exemplo, AccountName, SID e assim por diante.|
|commandLine|String|A linha de comando de invocação de processo completo, incluindo todos os parâmetros.|
|createdDateTime|DateTimeOffset|Hora em que o processo foi iniciado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|fileHash|[fileHash](filehash.md)|Tipo complexo que contém hashes de arquivo (criptográficos e sensíveis ao local).|
|integrityLevel|processIntegrityLevel|O nível de integridade do processo. Os possíveis valores são: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.|
|isElevated|Booliano|True se o processo estiver elevado.|
|nome|Cadeia de caracteres|O nome do arquivo de imagem do processo.|
|parentProcessCreatedDateTime|DateTimeOffset|DateTime no qual o processo pai foi iniciado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|parentProcessId|Int32|A ID do Processo (PID) do processo pai.|
|parentProcessName|String|O nome do arquivo de imagem do processo pai.|
|caminho|String|Caminho completo, incluindo nome do arquivo.|
|processId|Int32|A ID do Processo (PID) do processo.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.process"
}-->

```json
{
  "accountName": "String",
  "commandLine": "String",
  "createdDateTime": "String (timestamp)",
  "fileHash": {"@odata.type": "microsoft.graph.fileHash"},
  "integrityLevel": "@odata.type: microsoft.graph.processIntegrityLevel",
  "isElevated": true,
  "name": "String",
  "parentProcessCreatedDateTime": "String (timestamp)",
  "parentProcessId": 1024,
  "parentProcessName": "String",
  "path": "String",
  "processId": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "process resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

