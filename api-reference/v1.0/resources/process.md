---
title: tipo de recurso de processo
description: Contém informações com estado sobre o processo relacionado ao alerta.
ms.localizationpriority: medium
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 1c290ed08adae9f9b995c5c24c398826a2bb1160
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900489"
---
# <a name="process-resource-type"></a>tipo de recurso de processo

Namespace: microsoft.graph

Contém informações com estado sobre o processo relacionado ao alerta.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|Accountname|String|Identificador de conta de usuário (contexto de conta de usuário no qual o processo foi executado), por exemplo, AccountName, SID e assim por diante.|
|commandLine|String|A linha de comando de invocação de processo completa, incluindo todos os parâmetros.|
|createdDateTime|DateTimeOffset|Hora em que o processo foi iniciado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|fileHash|[fileHash](filehash.md)|Tipo complexo que contém hashes de arquivo (criptográficos e sensíveis à localização).|
|integrityLevel|processIntegrityLevel|O nível de integridade do processo. Os possíveis valores são: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.|
|isElevated|Booliano|True se o processo for elevado.|
|nome|String|O nome do arquivo de imagem do processo.|
|parentProcessCreatedDateTime|DateTimeOffset|DateTime no qual o processo pai foi iniciado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|parentProcessId|Int32|A ID do Processo (PID) do processo pai.|
|parentProcessName|String|O nome do arquivo de imagem do processo pai.|
|caminho|String|Caminho completo, incluindo o nome do arquivo.|
|Processid|Int32|A ID do Processo (PID) do processo.|

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

