---
title: tipo de recurso Process
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 6b67ec28dadb09442c5e3d66b6c03c54db821a85
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965688"
---
# <a name="process-resource-type"></a>tipo de recurso Process

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém informações de estado sobre o processo relacionado ao alerta.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|accountName|String|Identificador da conta de usuário (contexto da conta de usuário o processo executado em) por exemplo, AccountName, SID e assim por diante.|
|commandLine|String|A linha de comando de invocação de processo completo, incluindo todos os parâmetros.|
|createdDateTime|DateTimeOffset|Hora em que o processo foi iniciado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|fileHash|[fileHash](filehash.md)|Tipo complexo contendo hashes de arquivo (criptográfico e diferencia local).|
|integrityLevel|processIntegrityLevel|O nível de integridade do processo. Os possíveis valores são: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.|
|iselevados|Booliano|True se o processo é elevado.|
|name|String|O nome do arquivo de imagem do processo.|
|parentProcessCreatedDateTime|DateTimeOffset|DateTime no qual o processo pai foi iniciado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|parentProcessId|Int32|A ID de processo (PID) do processo pai.|
|parentProcessName|String|O nome do arquivo de imagem do processo pai.|
|caminho|String|Caminho completo, incluindo o nome do arquivo.|
|Identificação|Int32|A identificação do processo (PID) do processo.|

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
<!--
{
  "type": "#page.annotation",
  "description": "process resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
