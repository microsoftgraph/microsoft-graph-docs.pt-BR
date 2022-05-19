---
title: Tipo de recurso servicePlanInfo
description: Contém informações sobre um plano de serviço associado a uma SKU inscrita. A propriedade **servicePlans** da entidade subscribedSku é uma coleção de **servicePlanInfo**.
ms.localizationpriority: medium
author: jconley76
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 54897e9a1d5d36baae67570388c603b2b7f8d6e8
ms.sourcegitcommit: 562dc670cea411de0ecc232840ce1c650abbe34c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2022
ms.locfileid: "65549530"
---
# <a name="serviceplaninfo-resource-type"></a>Tipo de recurso servicePlanInfo

Namespace: microsoft.graph

Contém informações sobre um plano de serviço associado a uma SKU inscrita. A propriedade **servicePlans** da entidade [subscribedSku](subscribedsku.md) é uma coleção de **servicePlanInfo**.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|servicePlanId|Guid|O identificador exclusivo do plano de serviços.|
|servicePlanName|Cadeia de caracteres|O nome do plano de serviços.|
|provisioningStatus|Cadeia de caracteres|O status de provisionamento do plano de serviços. Os valores possíveis são:<br/>`Success` - O serviço está totalmente provisionado.<br/>`Disabled` - O serviço foi desabilitado.<br/>`ErrorStatus` - O plano de serviço não foi provisionado e está em um estado de erro.<br/>`PendingInput` - O serviço ainda não foi provisionado; aguardando confirmação do serviço.<br/>`PendingActivation` - O serviço é provisionado, mas requer ativação explícita pelo administrador (por exemplo, Intune_O365 de serviço)<br/>`PendingProvisioning` - A Microsoft adicionou um novo serviço ao SKU do produto e ainda não foi ativado no locatário.|
|Appliesto|Cadeia de caracteres|O objeto ao qual o plano de serviço pode ser atribuído. Os valores possíveis são:<br/>`User` – o plano de serviço pode ser atribuído a usuários individuais.<br/>`Company` – o plano de serviço pode ser atribuído a todo o locatário.|

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
  "servicePlanId": "Guid",
  "servicePlanName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePlanInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

