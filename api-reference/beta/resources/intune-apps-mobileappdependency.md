---
title: Tipo de recurso mobileAppDependency
description: Descreve um tipo de dependência entre dois aplicativos móveis.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bfdb66d5baa3bf16d870b69f8187a836e2d92bff
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58793912"
---
# <a name="mobileappdependency-resource-type"></a>Tipo de recurso mobileAppDependency

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Descreve um tipo de dependência entre dois aplicativos móveis.


Herda de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar mobileAppDependencies](../api/intune-apps-mobileappdependency-list.md)|[Coleção mobileAppDependency](../resources/intune-apps-mobileappdependency.md)|Listar propriedades e relações dos objetos [mobileAppDependency.](../resources/intune-apps-mobileappdependency.md)|
|[Obter mobileAppDependency](../api/intune-apps-mobileappdependency-get.md)|[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)|Leia propriedades e relações do [objeto mobileAppDependency.](../resources/intune-apps-mobileappdependency.md)|
|[Criar mobileAppDependency](../api/intune-apps-mobileappdependency-create.md)|[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)|Crie um novo [objeto mobileAppDependency.](../resources/intune-apps-mobileappdependency.md)|
|[Excluir mobileAppDependency](../api/intune-apps-mobileappdependency-delete.md)|Nenhum(a)|Exclui um [mobileAppDependency](../resources/intune-apps-mobileappdependency.md).|
|[Atualizar mobileAppDependency](../api/intune-apps-mobileappdependency-update.md)|[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)|Atualize as propriedades de um [objeto mobileAppDependency.](../resources/intune-apps-mobileappdependency.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID da entidade de relação. Herdado [de mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetId|Cadeia de caracteres|A ID do aplicativo móvel de destino. Herdado [de mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetDisplayName|Cadeia de caracteres|O nome de exibição do aplicativo móvel de destino. Herdado [de mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetDisplayVersion|Cadeia de caracteres|A versão de exibição do aplicativo móvel de destino. Herdado [de mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetPublisher|Cadeia de caracteres|O editor do aplicativo móvel de destino. Herdado [de mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetType|[mobileAppRelationshipType](../resources/intune-apps-mobileapprelationshiptype.md)|O tipo de relação que indica se o destino é pai ou filho. Herdado [de mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md). Os valores possíveis são: `child` e `parent`.|
|dependencyType|[mobileAppDependencyType](../resources/intune-apps-mobileappdependencytype.md)|O tipo de relação de dependência entre os aplicativos pai e filho. Os valores possíveis são: `detect` e `autoInstall`.|
|dependentAppCount|Int32|O número total de aplicativos que dependem direta ou indiretamente do aplicativo pai.|
|dependsOnAppCount|Int32|O número total de aplicativos dos quais o aplicativo filho depende direta ou indiretamente.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppDependency"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppDependency",
  "id": "String (identifier)",
  "targetId": "String",
  "targetDisplayName": "String",
  "targetDisplayVersion": "String",
  "targetPublisher": "String",
  "targetType": "String",
  "dependencyType": "String",
  "dependentAppCount": 1024,
  "dependsOnAppCount": 1024
}
```



