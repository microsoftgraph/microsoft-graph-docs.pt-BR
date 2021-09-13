---
title: Tipo de recurso mobileAppRelationship
description: Descreve uma relação entre dois aplicativos móveis.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6e3a355b2eab4c70349156a921d508f33705c65c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59124151"
---
# <a name="mobileapprelationship-resource-type"></a>Tipo de recurso mobileAppRelationship

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Descreve uma relação entre dois aplicativos móveis.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar mobileAppRelationships](../api/intune-apps-mobileapprelationship-list.md)|[Coleção mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|Listar propriedades e relações dos objetos [mobileAppRelationship.](../resources/intune-apps-mobileapprelationship.md)|
|[Obter mobileAppRelationship](../api/intune-apps-mobileapprelationship-get.md)|[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|Leia propriedades e relações do [objeto mobileAppRelationship.](../resources/intune-apps-mobileapprelationship.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID da entidade de relação.|
|targetId|Cadeia de Caracteres|A ID do aplicativo móvel de destino.|
|targetDisplayName|Cadeia de Caracteres|O nome de exibição do aplicativo móvel de destino.|
|targetDisplayVersion|Cadeia de Caracteres|A versão de exibição do aplicativo móvel de destino.|
|targetPublisher|Cadeia de Caracteres|O editor do aplicativo móvel de destino.|
|targetType|[mobileAppRelationshipType](../resources/intune-apps-mobileapprelationshiptype.md)|O tipo de relação que indica se o destino é pai ou filho. Os valores possíveis são: `child`, `parent`.|

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
  "targetDisplayName": "String",
  "targetDisplayVersion": "String",
  "targetPublisher": "String",
  "targetType": "String"
}
```



