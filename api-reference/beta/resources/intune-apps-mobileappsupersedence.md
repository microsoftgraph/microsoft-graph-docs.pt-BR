---
title: Tipo de recurso mobileAppSupersedence
description: Descreve uma relação de supersedência entre dois aplicativos móveis.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ff91da571956d7579d27f65d485d97c158c17bee
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59075848"
---
# <a name="mobileappsupersedence-resource-type"></a>Tipo de recurso mobileAppSupersedence

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Descreve uma relação de supersedência entre dois aplicativos móveis.


Herda de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar mobileAppSupersedences](../api/intune-apps-mobileappsupersedence-list.md)|[Coleção mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md)|Listar propriedades e relações dos [objetos mobileAppSupersedence.](../resources/intune-apps-mobileappsupersedence.md)|
|[Obter mobileAppSupersedence](../api/intune-apps-mobileappsupersedence-get.md)|[mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md)|Leia propriedades e relações do [objeto mobileAppSupersedence.](../resources/intune-apps-mobileappsupersedence.md)|
|[Criar mobileAppSupersedence](../api/intune-apps-mobileappsupersedence-create.md)|[mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md)|Crie um novo [objeto mobileAppSupersedence.](../resources/intune-apps-mobileappsupersedence.md)|
|[Excluir mobileAppSupersedence](../api/intune-apps-mobileappsupersedence-delete.md)|Nenhum|Exclui uma [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md).|
|[Atualizar mobileAppSupersedence](../api/intune-apps-mobileappsupersedence-update.md)|[mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md)|Atualize as propriedades de um [objeto mobileAppSupersedence.](../resources/intune-apps-mobileappsupersedence.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID da entidade de relação. Herdado [de mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetId|Cadeia de caracteres|A ID do aplicativo móvel de destino. Herdado [de mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetDisplayName|Cadeia de caracteres|O nome de exibição do aplicativo móvel de destino. Herdado [de mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetDisplayVersion|Cadeia de Caracteres|A versão de exibição do aplicativo móvel de destino. Herdado [de mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetPublisher|String|O editor do aplicativo móvel de destino. Herdado [de mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetType|[mobileAppRelationshipType](../resources/intune-apps-mobileapprelationshiptype.md)|O tipo de relação que indica se o destino é pai ou filho. Herdado [de mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md). Os valores possíveis são: `child` e `parent`.|
|supersedenceType|[mobileAppSupersedenceType](../resources/intune-apps-mobileappsupersedencetype.md)|O tipo de relação de supersedência entre os aplicativos pai e filho. Os valores possíveis são: `update` e `replace`.|
|supersededAppCount|Int32|O número total de aplicativos, direta ou indiretamente, sobressumentados pelo aplicativo filho.|
|supersedingAppCount|Int32|O número total de aplicativos, direta ou indiretamente, sobressando o aplicativo pai.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppSupersedence"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppSupersedence",
  "id": "String (identifier)",
  "targetId": "String",
  "targetDisplayName": "String",
  "targetDisplayVersion": "String",
  "targetPublisher": "String",
  "targetType": "String",
  "supersedenceType": "String",
  "supersededAppCount": 1024,
  "supersedingAppCount": 1024
}
```



