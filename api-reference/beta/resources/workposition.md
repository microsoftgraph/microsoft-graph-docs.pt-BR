---
title: Tipo de recurso workPosition
description: Tipo de recurso workPosition
ms.localizationpriority: medium
author: kevinbellinger
ms.prod: people-and-workplace-intelligence
doc_type: resourcePageType
ms.openlocfilehash: e26e9d5a4d48cb2b1186b1ea69e4b462a8ef93a4
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66730571"
---
# <a name="workposition-resource-type"></a>Tipo de recurso workPosition

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações detalhadas sobre as posições de trabalho associadas ao perfil de um [usuário](profile.md).

Esse tipo de recurso herda de [itemFacet](itemfacet.md).


## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar posições](../api/profile-list-positions.md)|[coleção workPosition](../resources/workposition.md)|Obtenha os recursos workPosition da propriedade de navegação de posições.|
|[Criar workPosition](../api/profile-post-positions.md)|[workPosition](../resources/workposition.md)|Crie um novo objeto workPosition.|
|[Obter workPosition](../api/workposition-get.md)|[workPosition](../resources/workposition.md)|Leia as propriedades e as relações de um [objeto workPosition](../resources/workposition.md) .|
|[Atualizar workPosition](../api/workposition-update.md)|[workPosition](../resources/workposition.md)|Atualize as propriedades de um [objeto workPosition](../resources/workposition.md) .|
|[Excluir workPosition](../api/workposition-delete.md)|Nenhum|Exclui um [objeto workPosition](../resources/workposition.md) .|


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowedAudiences|String|Os públicos-alvo que podem ver os valores contidos na entidade. Herdado de [itemFacet](../resources/itemfacet.md). Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|categories|Coleção de cadeias de caracteres|Categorias que o usuário associou a essa posição.|
|Colegas|[Coleção relatedPerson](../resources/relatedperson.md)|Colegas associados a essa posição.|
|createdBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que criou a entidade. Herdado de [itemFacet](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Fornece o dateTimeOffset para quando a entidade foi criada. Herdado de [itemFacet](../resources/itemfacet.md).|
|Detalhe|[positionDetail](../resources/positiondetail.md)|Contém informações detalhadas sobre a posição. |
|id|String|Identificador usado para endereçar individualmente a entidade. Herdado da [entidade](../resources/entity.md)|
|Inferência|[inferenceData](../resources/inferencedata.md)|Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação. Herdado de [itemFacet](../resources/itemfacet.md).|
|Iscurrent|Boolean|Indica se a posição é atual ou não.|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que modificou a entidade pela última vez. Herdado de [itemFacet](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Fornece o dateTimeOffset para quando a entidade foi criada. Herdado de [itemFacet](../resources/itemfacet.md).|
|manager|[relatedPerson](../resources/relatedperson.md)|Contém detalhes do gerente do usuário nessa posição.|
|source|[personDataSource](../resources/persondatasource.md)|Onde os valores foram originados se sincronizados de outro serviço. Herdado de [itemFacet](../resources/itemfacet.md).|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workPosition",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workPosition",
  "id": "String (identifier)",
  "allowedAudiences": "String",
  "inference": {
    "@odata.type": "microsoft.graph.inferenceData"
  },
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "source": {
    "@odata.type": "microsoft.graph.personDataSource"
  },
  "categories": [
    "String"
  ],
  "detail": {
    "@odata.type": "microsoft.graph.positionDetail"
  },
  "manager": {
    "@odata.type": "microsoft.graph.relatedPerson"
  },
  "colleagues": [
    {
      "@odata.type": "microsoft.graph.relatedPerson"
    }
  ],
  "isCurrent": "Boolean"
}
```

