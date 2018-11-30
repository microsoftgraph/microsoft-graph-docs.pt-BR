---
title: Tipo de recurso servicePlanInfo
description: Contém informações sobre um plano de serviço associado a uma SKU inscrita. A propriedade **servicePlans** da entidade subscribedSku é uma coleção de **servicePlanInfo**.
ms.openlocfilehash: 70d49eb22542e9bc22ee28df5bc77b3bf6146b6d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005314"
---
# <a name="serviceplaninfo-resource-type"></a>Tipo de recurso servicePlanInfo

Contém informações sobre um plano de serviço associado a uma SKU inscrita. A propriedade **servicePlans** da entidade [subscribedSku](subscribedsku.md) é uma coleção de **servicePlanInfo**.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|servicePlanId|Guid|O identificador exclusivo do plano de serviços.|
|servicePlanName|String|O nome do plano de serviços.|
|provisioningStatus|String|O status de provisionamento do plano de serviços. Valores possíveis:<br/>"Success" – o serviço está totalmente provisionado.<br/>“Disabled” – o serviço foi desabilitado.<br/>"PendingInput" – o serviço ainda não está provisionado; aguardando confirmação do serviço.<br/>"PendingActivation" – o serviço está provisionado, mas requer ativação explícita pelo administrador (por exemplo, plano de serviço do Intune_O365)<br/>"PendingProvisioning" – a Microsoft adicionou um novo serviço ao SKU do produto e ele não foi ativado no locatário ainda.|
|appliesTo|String|O objeto ao qual o plano de serviço pode ser atribuído. Valores possíveis:<br/>"Usuário" – o plano de serviço pode ser atribuído a usuários individuais.<br/>"Empresa" – o plano de serviço pode ser atribuído a todos os locatários.|

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
<!-- {
  "type": "#page.annotation",
  "description": "servicePlanInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
