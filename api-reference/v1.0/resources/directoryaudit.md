---
title: Tipo de recurso directoryObject
description: Representa os itens de auditoria de diretório e sua coleção.
author: SarahBar
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 08a723f5d26e6d45b6cb4e7ede6b2d5a496dab86
ms.sourcegitcommit: b21ad24622e199331b6ab838a949ddce9726b41b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2022
ms.locfileid: "64848731"
---
# <a name="directoryaudit-resource-type"></a>Tipo de recurso directoryObject

Namespace: microsoft.graph

Representa os itens de auditoria de diretório e sua coleção.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Lista directoryAudits](../api/directoryaudit-list.md) | [directoryAudit](directoryaudit.md) |Liste os itens de auditoria de diretório no conjunto de suas propriedades.|
|[Obter directoryAudit](../api/directoryaudit-get.md) | [directoryAudit](directoryaudit.md) |Obter um item de auditoria do diretório específico e suas propriedades.|

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo                                                | Descrição                                                                                                                                                                                                                                                                        |
|:--------------------|:----------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| activityDateTime    | DateTimeOffset                                      | Indica a data e hora que a atividade foi executada. O tipo de Timestamp é sempre UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.                                                                                          |
| activityDisplayName | Cadeia de caracteres                                              | Indica o nome da atividade ou o nome da operação (exemplos: "Criar Usuário" e "Adicionar membro ao grupo"). Para obter uma lista completa, consulte [a lista de atividades do Azure AD](/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list). |
| additionalDetails   | Coleção [KeyValue](keyvalue.md)                  | Indica detalhes adicionais sobre a atividade.                                                                                                                                                                                                                                      |
| category            | Cadeia de caracteres                                              | Indica qual categoria de recurso direcionada pela atividade. (Por exemplo: gerenciamento de usuário, grupo gerenciamento etc..)                                                                                                                                                          |
| correlationId       | Guid                                                | Indica uma ID exclusiva que ajuda correlacionar atividades que englobam vários serviços. Pode ser usado para os logs de serviços de rastreamento.                                                                                                                                                |
| id                  | Cadeia de caracteres                                              | Indica que a ID exclusiva para a atividade. Este é um GUID.                                                                                                                                                                                                                          |
| initiatedBy         | [auditActivityInitiator](auditactivityinitiator.md) | Indica que informações sobre o usuário ou o aplicativo iniciou a atividade.                                                                                                                                                                                                                |
| operationType       | Cadeia de Caracteres                                              | Indica o tipo de operação que foi executada. Os valores possíveis incluem, mas não estão limitados aos seguintes: `Add`, `Assign`, `Update`, `Unassign`e `Delete`.                                                                                   |
| loggedByService     | Cadeia de caracteres                                              | Indica informações sobre qual serviço iniciou a atividade (por exemplo: `Self-service Password Management`, , `Core Directory`, `B2C`, `Invited Users`, `Microsoft Identity Manager``Privileged Identity Management`.                                                                      |
| resultado              | Operationresult                                              | Indica o resultado da atividade. Os valores possíveis são: `success`, `failure`, `timeout`, `unknownFutureValue`.                                                                                                                                                                   |
| resultReason        | Cadeia de caracteres                                              | Indica o motivo da falha se o **resultado** for `failure` ou `timeout`.                                                                                                                                                                                                                                 |
| targetResources     | [targetResource](targetresource.md) conjunto      | Indica informação que o recurso foi alterado devido a atividade. O tipo de recurso de destino `User`pode ser , , `Directory`, `Role``App`, , `Group``Policy` ou `Other`. `Device`                                                                                                                   |

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
  "result": "String",
  "resultReason": "String",
  "targetResources": [{"@odata.type": "microsoft.graph.targetResource"}]
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
