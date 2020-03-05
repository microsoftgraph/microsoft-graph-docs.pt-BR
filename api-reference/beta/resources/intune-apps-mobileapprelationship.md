---
title: tipo de recurso mobileAppRelationship
description: Descreve o relacionamento de um aplicativo móvel filho para seu aplicativo móvel pai.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3841ab8e10bb1306dcd2f7b5b3002ded0bd2fcbc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42491425"
---
# <a name="mobileapprelationship-resource-type"></a>tipo de recurso mobileAppRelationship

Namespace: Microsoft. Graph

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



