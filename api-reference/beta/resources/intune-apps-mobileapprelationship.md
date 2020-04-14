---
title: tipo de recurso mobileAppRelationship
description: Descreve o relacionamento de um aplicativo móvel filho para seu aplicativo móvel pai.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 80cf0fd5897d0ff3d1b3b3adc5343ad4c059442e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43462579"
---
# <a name="mobileapprelationship-resource-type"></a>tipo de recurso mobileAppRelationship

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Descreve o relacionamento de um aplicativo móvel filho para seu aplicativo móvel pai.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar mobileAppRelationships](../api/intune-apps-mobileapprelationship-list.md)|coleção [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|Listar Propriedades e relações dos objetos [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) .|
|[Obter mobileAppRelationship](../api/intune-apps-mobileapprelationship-get.md)|[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|Leia as propriedades e as relações do objeto [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A ID da entidade de relação.|
|targetId|String|A ID de aplicativo do aplicativo móvel do filho de destino.|
|targetDisplayName|String|O nome de exibição do aplicativo móvel filho de destino.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppRelationship"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppRelationship",
  "id": "String (identifier)",
  "targetId": "String",
  "targetDisplayName": "String"
}
```



