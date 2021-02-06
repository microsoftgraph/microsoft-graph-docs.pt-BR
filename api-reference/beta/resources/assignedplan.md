---
title: Tipo de recurso assignedPlan
description: A propriedade **assignedPlans** das entidades user e organization é uma coleção de **assignedPlan**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: krbain
ms.openlocfilehash: 7cb9aeeca6ad1838ede8395ab270cf10f84faa5f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130905"
---
# <a name="assignedplan-resource-type"></a>Tipo de recurso assignedPlan

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A propriedade **assignedPlans** das entidades [user](user.md) e [organization](organization.md) é uma coleção de **assignedPlan**.


## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|assignedDateTime|DateTimeOffset|A data e hora em que o plano foi atribuído; por exemplo: 2013-01-02T19:32:30Z. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|capabilityStatus|[capabilityStatus](#capabilitystatus-values)|Condição da atribuição de recursos. Os valores possíveis `Enabled` são , , , `Warning` `Suspended` `Deleted` `LockedOut` .|
|service|Cadeia de caracteres|O nome do serviço; por exemplo, "Exchange".|
|servicePlanId|Guid|Um GUID que identifica o plano de serviço.|


### <a name="capabilitystatus-values"></a>Valores de capabilityStatus

| Member | Descrição  |
|:---------------|:--------|
| Habilitado | Disponível para uso normal. |
| Aviso | Disponível para uso normal, mas está em um período de carência. |
| Suspenso | Indisponível, mas todos os dados associados à funcionalidade devem ser preservados. |
| Deleted | Indisponível e quaisquer dados associados à funcionalidade podem ser excluídos. |
| LockedOut | Indisponível para todos os administradores e usuários, mas todos os dados associados à funcionalidade devem ser preservados. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignedPlan"
}-->

```json
{
  "assignedDateTime": "String (timestamp)",
  "capabilityStatus": "string",
  "service": "string",
  "servicePlanId": "guid"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "assignedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


