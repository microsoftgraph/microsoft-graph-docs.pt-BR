---
title: tipo de recurso de directoryAudit
description: Esse recurso representa os itens de auditoria de diretório e sua coleção
author: lleonard-msft
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1f980208788731206dc58870635644a1f3edc4c7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991780"
---
# <a name="directoryaudit-resource-type"></a>tipo de recurso de directoryAudit
Esse recurso representa os itens de auditoria de diretório e sua coleção


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Lista directoryAudits](../api/directoryaudit-list.md) | [directoryAudit](directoryaudit.md) |Listam os itens de auditoria de diretório na coleção e suas propriedades.|
|[Obter directoryAudit](../api/directoryaudit-get.md) | [directoryAudit](directoryaudit.md) |Obtenha um item de auditoria de diretório específico e suas propriedades.|


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|activityDateTime|DateTimeOffset|Indica a data e hora que a atividade foi executada. O tipo de carimbo de hora é sempre em horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|activityDisplayName|String|Indica o nome da atividade ou o nome da operação (ex.: "Criar usuário", "Adicionar membro ao grupo"). Para obter uma lista de atividades conectado, consulte [lista de atividades do Windows Azure Ad](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list).|
|additionalDetails|coleção [keyValue](keyvalue.md)|Indica detalhes adicionais sobre a atividade.|
|Ferramentas para desenvolvedores|Cadeia de caracteres|Indica qual categoria de recurso que está programada pela atividade. (Por exemplo: gerenciamento de usuário, grupo gerenciamento etc..)|
|correlationId|GUID|Indica uma identificação exclusiva que ajuda a correlacionar atividades que se estendem por vários serviços. Podem ser usadas para logs de rastreamento em serviços.|
|id|String| Indica a ID exclusiva da atividade. Este é um GUID.|
|initiatedBy|[auditActivityInitiator](auditactivityinitiator.md)|Indica informações sobre o usuário ou aplicativo iniciado a atividade.|
|loggedByService|String|Indica informações no qual o serviço iniciou a atividade (por exemplo: gerenciamento de senha pessoal, Core diretório, B2C, usuários convidados, Microsoft Identity Manager, privilegiado gerenciamento de identidade.|
|result|string| Indica o resultado da atividade. Os valores possíveis são: `success`, `failure`, `timeout`, `unknownFutureValue`.||
|resultReason|String|Indica o motivo da falha se o resultado é "Falha" ou "timeout".|
|targetResources|coleção [targetResource](targetresource.md)|Indica informações no qual o recurso foi alterado devido a atividade. Tipo de recurso de destino pode ser um usuário, dispositivo, diretório, App, função, grupo, política ou outros.

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
  "result": "string",
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
