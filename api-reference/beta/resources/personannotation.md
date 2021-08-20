---
title: Tipo de recurso personAnnotation
description: Tipo de recurso personAnnotation
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 49e7945b1ba07d7daedbd197b826148921f2f0227dd71b5780413a3b67b6c6be
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54197846"
---
# <a name="personannotation-resource-type"></a>Tipo de recurso personAnnotation

Namespace: microsoft.graph

Fornece informações em notas que o usuário se associou a si mesmo em vários serviços e compartilhou com outras pessoas.

Herda do [itemFacet](../resources/itemfacet.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar anotações](../api/profile-list-notes.md)|[Coleção personAnnotation](../resources/personannotation.md)|Obter os recursos personAnnotation da propriedade de navegação notes.|
|[Criar personAnnotation](../api/profile-post-notes.md)|[personAnnotation](../resources/personannotation.md)|Crie um novo objeto personAnnotation.|
|[Obter personAnnotation](../api/personannotation-get.md)|[personAnnotation](../resources/personannotation.md)|Leia as propriedades e as relações de um [objeto personAnnotation.](../resources/personannotation.md)|
|[Atualizar personAnnotation](../api/personannotation-update.md)|[personAnnotation](../resources/personannotation.md)|Atualize as propriedades de [um objeto personAnnotation.](../resources/personannotation.md)|
|[Excluir personAnnotation](../api/personannotation-delete.md)|Nenhum|Exclui um [objeto personAnnotation.](../resources/personannotation.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowedAudiences|Cadeia de caracteres|As audiências que são capazes de ver os valores contidos na entidade. Herdado [do itemFacet](../resources/itemfacet.md). Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|createdBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que criou a entidade. Herdado [do itemFacet](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Fornece a dataTimeOffset para quando a entidade foi criada. Herdado [do itemFacet](../resources/itemfacet.md).|
|detail|[itemBody](../resources/itembody.md)|Contém os detalhes da própria nota.|
|displayName|Cadeia de caracteres|Contém um nome amigável para a nota.|
|id|Cadeia de caracteres|Identificador usado para endereçamento individual da entidade. Herdado da [entidade](../resources/entity.md)|
|inferência|[inferenceData](../resources/inferencedata.md)|Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação. Herdado [do itemFacet](../resources/itemfacet.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que modificou a entidade pela última vez. Herdado [do itemFacet](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Fornece a dataTimeOffset para quando a entidade foi criada. Herdado [do itemFacet](../resources/itemfacet.md).|
|source|[personDataSource](../resources/persondatasource.md)|Onde os valores se originaram se sincronizados de outro serviço. Herdado [do itemFacet](../resources/itemfacet.md).|

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


