---
title: tipo de recurso mobileAppDependency
description: Descreve um tipo de dependência entre dois aplicativos móveis.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9b55faee86852d8b7070850a4c14a2df8fe82631
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052737"
---
# <a name="mobileappdependency-resource-type"></a>tipo de recurso mobileAppDependency

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Descreve um tipo de dependência entre dois aplicativos móveis.


Herda de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar mobileAppDependencies](../api/intune-apps-mobileappdependency-list.md)|coleção [mobileAppDependency](../resources/intune-apps-mobileappdependency.md)|Listar Propriedades e relações dos objetos [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) .|
|[Obter mobileAppDependency](../api/intune-apps-mobileappdependency-get.md)|[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)|Leia as propriedades e as relações do objeto [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) .|
|[Criar mobileAppDependency](../api/intune-apps-mobileappdependency-create.md)|[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)|Criar um novo objeto [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) .|
|[Excluir mobileAppDependency](../api/intune-apps-mobileappdependency-delete.md)|Nenhum|Exclui [mobileAppDependency](../resources/intune-apps-mobileappdependency.md).|
|[Atualizar mobileAppDependency](../api/intune-apps-mobileappdependency-update.md)|[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)|Atualiza as propriedades de um objeto [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID da entidade de relação. Herdado de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetId|Cadeia de caracteres|A ID de aplicativo do aplicativo móvel de destino. Herdado de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetDisplayName|Cadeia de caracteres|O nome de exibição do aplicativo móvel de destino. Herdado de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetType|[mobileAppRelationshipType](../resources/intune-apps-mobileapprelationshiptype.md)|O tipo de relação que indica se o destino é um pai ou filho. Herdado de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md). Os valores possíveis são: `child` e `parent`.|
|DependencyType|[mobileAppDependencyType](../resources/intune-apps-mobileappdependencytype.md)|O tipo de relação de dependência entre os aplicativos pai e filho. Os valores possíveis são: `detect` e `autoInstall`.|
|dependentAppCount|Int32|O número total de dependências do aplicativo filho.|

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
  "targetType": "String",
  "dependencyType": "String",
  "dependentAppCount": 1024
}
```






