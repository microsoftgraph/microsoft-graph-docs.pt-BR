---
title: tipo de recurso personAnnotation
description: tipo de recurso personAnnotation
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 757797a8a252f934050cb8425f49042707734ed5
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812896"
---
# <a name="personannotation-resource-type"></a>tipo de recurso personAnnotation

Namespace: microsoft.graph

Fornece informações sobre as anotações que o usuário já associou em vários serviços e compartilhou com outras pessoas.

Herda de [Myfacet](../resources/itemfacet.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar anotações](../api/profile-list-notes.md)|coleção [personAnnotation](../resources/personannotation.md)|Obtenha os recursos personAnnotation da propriedade de navegação Notes.|
|[Criar personAnnotation](../api/profile-post-notes.md)|[personAnnotation](../resources/personannotation.md)|Criar um novo objeto personAnnotation.|
|[Obter personAnnotation](../api/personannotation-get.md)|[personAnnotation](../resources/personannotation.md)|Leia as propriedades e os relacionamentos de um objeto [personAnnotation](../resources/personannotation.md) .|
|[Atualizar personAnnotation](../api/personannotation-update.md)|[personAnnotation](../resources/personannotation.md)|Atualiza as propriedades de um objeto [personAnnotation](../resources/personannotation.md) .|
|[Excluir personAnnotation](../api/personannotation-delete.md)|Nenhum|Exclui um objeto [personAnnotation](../resources/personannotation.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowedAudiences|String|As audiências que podem ver os valores contidos na entidade. Herdado de [MyFace](../resources/itemfacet.md). Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|createdBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que criou a entidade. Herdado de [MyFace](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Fornece o dateTimeOffset para quando a entidade foi criada. Herdado de [MyFace](../resources/itemfacet.md).|
|detalhada|[itemBody](../resources/itembody.md)|Contém os detalhes da anotação propriamente dita.|
|displayName|String|Contém um nome amigável para a anotação.|
|id|String|Identificador usado para o endereçamento individual da entidade. Herdado da [entidade](../resources/entity.md)|
|fracassa|[inferenceData](../resources/inferencedata.md)|Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação. Herdado de [MyFace](../resources/itemfacet.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que modificou a entidade pela última vez. Herdado de [MyFace](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Fornece o dateTimeOffset para quando a entidade foi criada. Herdado de [MyFace](../resources/itemfacet.md).|
|source|[personDataSource](../resources/persondatasource.md)|Onde os valores são originados se forem sincronizados a partir de outro serviço. Herdado de [MyFace](../resources/itemfacet.md).|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.personAnnotation",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.personAnnotation",
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
  "detail": {
    "@odata.type": "microsoft.graph.itemBody"
  },
  "displayName": "String"
}
```
