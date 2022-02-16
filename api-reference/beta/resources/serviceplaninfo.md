---
title: Tipo de recurso servicePlanInfo
description: Contém informações sobre um plano de serviço associado a uma SKU inscrita. A propriedade **servicePlans** da entidade subscribedSku é uma coleção de **servicePlanInfo**.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: directory-management
author: jpettere
ms.openlocfilehash: 99ed2a06864953697858ee338d7b8ace9074c1b6
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/16/2022
ms.locfileid: "62854402"
---
# <a name="serviceplaninfo-resource-type"></a>Tipo de recurso servicePlanInfo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém informações sobre um plano de serviço associado a uma SKU inscrita. A propriedade **servicePlans** da entidade [subscribedSku](subscribedsku.md) é uma coleção de **servicePlanInfo**.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|servicePlanId|GUID|O identificador exclusivo do plano de serviços.|
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
  "appliesTo": "String",
  "provisioningStatus": "String",
  "servicePlanId": "GUID",
  "servicePlanName": "String"
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


