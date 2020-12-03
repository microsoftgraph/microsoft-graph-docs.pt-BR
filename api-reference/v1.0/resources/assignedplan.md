---
title: Tipo de recurso assignedPlan
description: A propriedade **assignedPlans** das entidades user e organization é uma coleção de **assignedPlan**.
localization_priority: Normal
author: krbain
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5ea10e7894b91fd6bf23625c6c3c0097fbe9ed09
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563762"
---
# <a name="assignedplan-resource-type"></a>Tipo de recurso assignedPlan

Namespace: microsoft.graph

A propriedade **assignedPlans** das entidades [user](user.md) e [organization](organization.md) é uma coleção de **assignedPlan**.


## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|assignedDateTime|DateTimeOffset|A data e hora em que o plano foi atribuído; por exemplo: 2013-01-02T19:32:30Z. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|capabilityStatus|[capabilityStatus](#capabilitystatus-values)|Condição da atribuição de recurso. Os valores possíveis são:,,, `Enabled` `Warning` `Suspended` `Deleted` , `LockedOut` .|
|service|Cadeia de caracteres|O nome do serviço; por exemplo, "Exchange".|
|onplanid|Guid|Um GUID que identifica o plano de serviço.|


### <a name="capabilitystatus-values"></a>valores de capabilityStatus

| Member | Descrição  |
|:---------------|:--------|
| Habilitado | Disponível para uso normal. |
| Aviso | Disponível para uso normal, mas está em um período de cortesia. |
| Suspensão | Indisponível, mas os dados associados ao recurso devem ser preservados. |
| Deleted | Indisponível e todos os dados associados ao recurso podem ser excluídos. |
| Bloqueado | Indisponível para todos os administradores e usuários, mas os dados associados ao recurso devem ser preservados. |

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
<!-- {
  "type": "#page.annotation",
  "description": "assignedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

