---
title: tipo de recurso workPosition
description: tipo de recurso workPosition
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: e9a13bc36b2ed1eb42b4155e86d69826b0c22d9d
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810353"
---
# <a name="workposition-resource-type"></a>tipo de recurso workPosition

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações detalhadas sobre posições de trabalho associadas ao [perfil](profile.md)de um usuário.

Esse tipo de recurso herda de [Myfacet](itemfacet.md).

## <a name="methods"></a>Métodos

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar posições](../api/profile-list-positions.md)|coleção [workPosition](../resources/workposition.md)|Obtenha os recursos workPosition da propriedade de navegação positions.|
|[Criar workPosition](../api/profile-post-positions.md)|[workPosition](../resources/workposition.md)|Criar um novo objeto workPosition.|
|[Obter workPosition](../api/workposition-get.md)|[workPosition](../resources/workposition.md)|Leia as propriedades e os relacionamentos de um objeto [workPosition](../resources/workposition.md) .|
|[Atualizar workPosition](../api/workposition-update.md)|[workPosition](../resources/workposition.md)|Atualiza as propriedades de um objeto [workPosition](../resources/workposition.md) .|
|[Excluir workPosition](../api/workposition-delete.md)|Nenhum|Exclui um objeto [workPosition](../resources/workposition.md) .|


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowedAudiences|String|As audiências que podem ver os valores contidos na entidade. Herdado de [MyFace](../resources/itemfacet.md). Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|categories|Coleção de cadeias de caracteres|Categorias que o usuário tenha associado a esta posição.|
|conhecidos|coleção [relatedPerson](../resources/relatedperson.md)|Colegas associados a esta posição.|
|createdBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que criou a entidade. Herdado de [MyFace](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Fornece o dateTimeOffset para quando a entidade foi criada. Herdado de [MyFace](../resources/itemfacet.md).|
|detalhada|[positionDetail](../resources/positiondetail.md)|Contém informações detalhadas sobre a posição. |
|id|String|Identificador usado para o endereçamento individual da entidade. Herdado da [entidade](../resources/entity.md)|
|fracassa|[inferenceData](../resources/inferencedata.md)|Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação. Herdado de [MyFace](../resources/itemfacet.md).|
|IsCurrent|Booliano|Indica se a posição é ou não atual.|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que modificou a entidade pela última vez. Herdado de [MyFace](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Fornece o dateTimeOffset para quando a entidade foi criada. Herdado de [MyFace](../resources/itemfacet.md).|
|manager|[relatedPerson](../resources/relatedperson.md)|Contém detalhes do gerente do usuário nesta posição.|
|source|[personDataSource](../resources/persondatasource.md)|Onde os valores são originados se forem sincronizados a partir de outro serviço. Herdado de [MyFace](../resources/itemfacet.md).|

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