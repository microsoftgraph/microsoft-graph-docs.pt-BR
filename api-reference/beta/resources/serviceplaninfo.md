---
title: Tipo de recurso servicePlanInfo
description: Contém informações sobre um plano de serviço associado a uma SKU inscrita. A propriedade **servicePlans** da entidade **subscribedSku** é uma coleção de servicePlanInfo.
localization_priority: Normal
ms.openlocfilehash: e759082984cc66f7d3efec3cbb7cbee11561f253
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512602"
---
# <a name="serviceplaninfo-resource-type"></a>Tipo de recurso servicePlanInfo

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém informações sobre um plano de serviço associado a uma SKU inscrita. A propriedade **servicePlans** da entidade [subscribedSku](subscribedsku.md) é uma coleção de **servicePlanInfo**.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|servicePlanId|Guid|O identificador exclusivo do plano de serviços.|
|servicePlanName|Cadeia de caracteres|O nome do plano de serviços.|
|provisioningStatus|String|O status de provisionamento do plano de serviços. Valores possíveis:<br/>"Success" – o serviço está totalmente provisionado.<br/>“Disabled” – o serviço foi desabilitado.<br/>"PendingInput" – o serviço ainda não está provisionado; aguardando confirmação do serviço.<br/>"PendingActivation" - serviço é provisionado, mas requer ativação explícita pelo administrador (por exemplo, plano de serviço Intune_O365).<br/>"PendingProvisioning" – a Microsoft adicionou um novo serviço ao SKU do produto e ele não foi ativado no locatário ainda.|
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
<!--
{
  "type": "#page.annotation",
  "description": "servicePlanInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/serviceplaninfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
