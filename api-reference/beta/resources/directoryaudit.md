---
title: Tipo de recurso directoryObject
description: Descreve o recurso directoryAudit (entidade) do Microsoft API do Graph (REST), que ajuda a auditar atividades de diretório (locatário) (versão beta).
author: SarahBar
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: a34e8deedfac1fa85273b37053b3019c59294cd3
ms.sourcegitcommit: b21ad24622e199331b6ab838a949ddce9726b41b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2022
ms.locfileid: "64848738"
---
# <a name="directoryaudit-resource-type"></a>Tipo de recurso directoryObject

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os itens de auditoria de diretório e sua coleção.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Lista directoryAudits](../api/directoryaudit-list.md) | [directoryAudit](directoryaudit.md) |Liste os itens de auditoria de diretório no conjunto de suas propriedades.|
|[Obter directoryAudit](../api/directoryaudit-get.md) | [directoryAudit](directoryaudit.md) |Obter um item de auditoria do diretório específico e suas propriedades.|


## <a name="properties"></a>Propriedades
| Propriedade            | Tipo                                                | Descrição                                                                                                                                                                                                                                                            |
|:--------------------|:----------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| activityDateTime    | DateTimeOffset                                      | Indica a data e hora que a atividade foi executada. O tipo de Timestamp é sempre UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.                                                                              |
| activityDisplayName | Cadeia de caracteres                                              | Indica o nome da atividade ou o nome da operação (ex.: "Criar usuário", "Adicionar membro ao grupo"). Para obter uma lista de atividades registradas, consulte a [lista de atividades do Azure AD](/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list). |
| additionalDetails   | Coleção [KeyValue](keyvalue.md)                  | Indica detalhes adicionais sobre a atividade.                                                                                                                                                                                                                          |
| category            | Cadeia de caracteres                                              | Indica qual categoria de recurso direcionada pela atividade. (Por exemplo: gerenciamento de usuário, grupo gerenciamento etc..)                                                                                                                                              |
| correlationId       | Guid                                                | Indica uma ID exclusiva que ajuda correlacionar atividades que englobam vários serviços. Pode ser usado para os logs de serviços de rastreamento.                                                                                                                                    |
| id                  | Cadeia de caracteres                                              | Indica que a ID exclusiva para a atividade.                                                                                                                                                                                                            |
| initiatedBy         | [auditActivityInitiator](auditactivityinitiator.md) | Indica que informações sobre o usuário ou o aplicativo iniciou a atividade.                                                                                                                                                                                                    |
| loggedByService     | Cadeia de caracteres                                              | Indica informação em que o serviço iniciou a atividade (por exemplo: gerenciamento de senha de autoatendimento, principais diretório, B2C, os usuários convidados, Microsoft Identity Manager, Privileged Identity Management.                                                          |
| operationType       | Cadeia de Caracteres                                              | Indica o tipo de operação que foi executada. Os valores possíveis incluem, mas não estão limitados aos seguintes: `Add`, `Assign`, `Update`, `Unassign`e `Delete`.                                                                                   |
| resultado              | Operationresult                                              | Indica o resultado da atividade. Os valores possíveis são: `success`, `failure`, `timeout`, `unknownFutureValue`.                                                                                                                                                       |
| resultReason        | Cadeia de caracteres                                              | Indica o motivo da falha se o **resultado** for `failure` ou `timeout`.                                                                                                                                                                                              |
| targetResources     | [targetResource](targetresource.md) conjunto      | Informações sobre o recurso que foi alterado devido à atividade.  | 
| userAgent | Cadeia de caracteres | Tipo de agente de usuário usado por um usuário na atividade. |                                                                                                      

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directoryAudit"
}-->

```json
{
  "activityDateTime": "String (timestamp)",
  "activityDisplayName": "String",
  "additionalDetails": [{"@odata.type": "microsoft.graph.keyValue"}],
  "category": "String",
  "correlationId": "Guid",
  "id": "String (identifier)",
  "initiatedBy": {"@odata.type": "microsoft.graph.auditActivityInitiator"},
  "loggedByService": "String",
  "operationType": "String",
  "result": "string",
  "resultReason": "String",
  "targetResources": [{"@odata.type": "microsoft.graph.targetResource"}],
  "userAgent": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryAudit resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


