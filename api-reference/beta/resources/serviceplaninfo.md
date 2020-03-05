---
title: Tipo de recurso servicePlanInfo
description: Contém informações sobre um plano de serviço associado a uma SKU inscrita. A propriedade **servicePlans** da entidade subscribedSku é uma coleção de **servicePlanInfo**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 069c42031b1738a3dcb5da77544a33d88ca998e8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520777"
---
# <a name="serviceplaninfo-resource-type"></a>Tipo de recurso servicePlanInfo

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém informações sobre um plano de serviço associado a uma SKU inscrita. A propriedade **servicePlans** da entidade [subscribedSku](subscribedsku.md) é uma coleção de **servicePlanInfo**.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|onplanid|Guid|O identificador exclusivo do plano de serviços.|
|onplanname|String|O nome do plano de serviços.|
|provisioningStatus|Cadeia de caracteres|O status de provisionamento do plano de serviços. Valores possíveis:<br/>"Success"-o serviço está totalmente provisionado.<br/>"Disabled"-o serviço foi desabilitado.<br/>"PendingInput" – o serviço ainda não foi provisionado; aguardando confirmação do serviço.<br/>"PendingActivation" – o serviço é provisionado, mas requer ativação explícita por administrador (por exemplo, Intune_O365 plano de serviço).<br/>"PendingProvisioning"-a Microsoft adicionou um novo serviço ao SKU do produto e ainda não foi ativado no locatário.|
|appliesTo|Cadeia de caracteres|O objeto ao qual o plano de serviço pode ser atribuído. Valores possíveis:<br/>"User" – o plano de serviço pode ser atribuído a usuários individuais.<br/>"Empresa"-o plano de serviço pode ser atribuído a todo o locatário.|

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
