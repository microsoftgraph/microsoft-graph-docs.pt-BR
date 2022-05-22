---
title: Tipo de recurso assignedPlan
description: A propriedade **assignedPlans** das entidades user e organization é uma coleção de **assignedPlan**.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: directory-management
author: jconley76
ms.openlocfilehash: b3749a6af4537459179619e83dbed9f9c7aea1fe
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629115"
---
# <a name="assignedplan-resource-type"></a>Tipo de recurso assignedPlan

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A propriedade **assignedPlans** das entidades [user](user.md) e [organization](organization.md) é uma coleção de **assignedPlan**.


## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|assignedDateTime|DateTimeOffset|A data e hora em que o plano foi atribuído; por exemplo: 2013-01-02T19:32:30Z. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|capabilityStatus|[capabilityStatus](#capabilitystatus-values)|Condição da atribuição de funcionalidade. Os valores possíveis são `Enabled`, `Warning`, `Suspended`, `Deleted`. `LockedOut`|
|service|Cadeia de caracteres|O nome do serviço; por exemplo, `exchange`.|
|servicePlanId|Guid|Um GUID que identifica o plano de serviço. Para obter uma lista completa de GUIDs e seus nomes de serviço amigáveis equivalentes, consulte Nomes de produtos e identificadores de plano [de serviço para licenciamento](/azure/active-directory/enterprise-users/licensing-service-plan-reference).|


### <a name="capabilitystatus-values"></a>Valores de capabilityStatus

A tabela a seguir descreve os possíveis status para **o capabilityStatus** de uma assinatura. Os membros serão listados na ordem de sua transição se a licença não for renovada.

| Member | Descrição  |
|:---------------|:--------|
| Habilitado | Disponível para uso normal e atribuição. |
| Aviso | Disponível para uso normal e atribuição, mas está em um período de carência. |
| Suspenso | Não disponível para atribuição, mas todos os dados associados à funcionalidade devem ser preservados. |
| Bloqueado | Não disponível para todos os administradores e usuários para atribuição, mas todos os dados associados à funcionalidade devem ser preservados. Esse é o estado após `Suspended` e se a licença não for renovada, ele será o estado final antes do plano ser `Deleted`. |
| Deleted | Indisponível e todos os dados associados à funcionalidade podem ser excluídos. |

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
  "capabilityStatus": "String",
  "service": "String",
  "servicePlanId": "Guid"
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


