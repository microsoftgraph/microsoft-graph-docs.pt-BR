---
title: Tipo de recurso servicePlanInfo
description: Contém informações sobre um plano de serviço associado a uma SKU inscrita. A propriedade **servicePlans** da entidade subscribedSku é uma coleção de **servicePlanInfo**.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: directory-management
author: jpettere
ms.openlocfilehash: 9d75e7ce3b4d7875c97ea7850465c578baaed9cf
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62348989"
---
# <a name="serviceplaninfo-resource-type"></a>Tipo de recurso servicePlanInfo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém informações sobre um plano de serviço associado a uma SKU inscrita. A propriedade **servicePlans** da entidade [subscribedSku](subscribedsku.md) é uma coleção de **servicePlanInfo**.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|servicePlanId|Guid|O identificador exclusivo do plano de serviços.|
|servicePlanName|Cadeia de caracteres|O nome do plano de serviços.|
|provisioningStatus|Cadeia de caracteres|O status de provisionamento do plano de serviços. Os valores possíveis são:<br/>`Success` - O serviço está totalmente provisionado.<br/>`Disabled` - O serviço foi desabilitado.<br/>`ErrorStatus` - O plano de serviço não foi provisionado e está em estado de erro.<br/>`PendingInput` - O serviço ainda não foi provisionado; aguardando confirmação do serviço.<br/>`PendingActivation` - O serviço é provisionado, mas exige ativação explícita pelo administrador (por exemplo, Intune_O365 plano de serviço)<br/>`PendingProvisioning` – A Microsoft adicionou um novo serviço à SKU do produto e ainda não foi ativado no locatário.|
|appliesTo|Cadeia de caracteres|O objeto ao que o plano de serviço pode ser atribuído. Os valores possíveis são:<br/>`User` - o plano de serviço pode ser atribuído a usuários individuais.<br/>`Company` - o plano de serviço pode ser atribuído a todo o locatário.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.servicePlanInfo"
}-->

```json
{
  "appliesTo": "string",
  "provisioningStatus": "string",
  "servicePlanId": "guid",
  "servicePlanName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "servicePlanInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


