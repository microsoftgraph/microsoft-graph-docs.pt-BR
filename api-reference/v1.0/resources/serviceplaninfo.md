---
title: Tipo de recurso servicePlanInfo
description: Contém informações sobre um plano de serviço associado a uma SKU inscrita. A propriedade **servicePlans** da entidade subscribedSku é uma coleção de **servicePlanInfo**.
ms.localizationpriority: medium
author: jpettere
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 1f8da276ccbd0f22023550797f1563939e6e7e39
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59126657"
---
# <a name="serviceplaninfo-resource-type"></a>Tipo de recurso servicePlanInfo

Namespace: microsoft.graph

Contém informações sobre um plano de serviço associado a uma SKU inscrita. A propriedade **servicePlans** da entidade [subscribedSku](subscribedsku.md) é uma coleção de **servicePlanInfo**.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|servicePlanId|Guid|O identificador exclusivo do plano de serviços.|
|servicePlanName|Cadeia de caracteres|O nome do plano de serviços.|
|provisioningStatus|Cadeia de caracteres|O status de provisionamento do plano de serviços. Valores possíveis:<br/>"Sucesso" - O serviço está totalmente provisionado.<br/>"Desabilitado" - O serviço foi desabilitado.<br/>"PendingInput" - O serviço ainda não foi provisionado; aguardando confirmação do serviço.<br/>"PendingActivation" - O serviço é provisionado, mas exige ativação explícita pelo administrador (por exemplo, Intune_O365 plano de serviço)<br/>"PendingProvisioning" - A Microsoft adicionou um novo serviço à SKU do produto e ainda não foi ativado no locatário.|
|appliesTo|Cadeia de caracteres|O objeto ao que o plano de serviço pode ser atribuído. Valores possíveis:<br/>"Usuário" - o plano de serviço pode ser atribuído a usuários individuais.<br/>"Empresa" - o plano de serviço pode ser atribuído a todo o locatário.|

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

