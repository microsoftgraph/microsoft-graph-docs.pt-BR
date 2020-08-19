---
title: tipo de recurso personWebsite
description: tipo de recurso personWebsite
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: e3f41b352af77073d6338888c8349e38145daff9
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811081"
---
# <a name="personwebsite-resource-type"></a>tipo de recurso personWebsite

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações detalhadas sobre sites associados a um usuário em vários serviços.

Herda de [Myfacet](itemfacet.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar sites](../api/profile-list-websites.md)|coleção [personWebsite](../resources/personwebsite.md)|Obtenha os recursos personWebsite da propriedade de navegação sites.|
|[Criar personWebsite](../api/profile-post-websites.md)|[personWebsite](../resources/personwebsite.md)|Criar um novo objeto personWebsite.|
|[Obter personWebsite](../api/personwebsite-get.md)|[personWebsite](../resources/personwebsite.md)|Leia as propriedades e os relacionamentos de um objeto [personWebsite](../resources/personwebsite.md) .|
|[Atualizar personWebsite](../api/personwebsite-update.md)|[personWebsite](../resources/personwebsite.md)|Atualiza as propriedades de um objeto [personWebsite](../resources/personwebsite.md) .|
|[Excluir personWebsite](../api/personwebsite-delete.md)|Nenhum|Exclui um objeto [personWebsite](../resources/personwebsite.md) .|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo              | Descrição                                                                                   |
|:-------------|:------------------|:----------------------------------------------------------------------------------------------|
|categories    |Coleção de cadeias de caracteres  | Contém categorias que um usuário associou ao site (por exemplo, pessoal, receitas).  |
|description   |String             | Contém uma descrição do site.                                                        |
|displayName   |String             | Contém um nome amigável para o site.                                                     |
|webUrl        |String             | Contém um link para o próprio site.                                                        |

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowedAudiences|String|As audiências que podem ver os valores contidos na entidade. Herdado de [MyFace](../resources/itemfacet.md). Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|categories|Coleção de cadeias de caracteres|Contém categorias que um usuário associou ao site (por exemplo, pessoal, receitas).|
|createdBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que criou a entidade. Herdado de [MyFace](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Fornece o dateTimeOffset para quando a entidade foi criada. Herdado de [MyFace](../resources/itemfacet.md).|
|description|String|Contém uma descrição do site.|
|displayName|String|Contém um nome amigável para o site.|
|id|String|Identificador usado para o endereçamento individual da entidade. Herdado da [entidade](../resources/entity.md)|
|fracassa|[inferenceData](../resources/inferencedata.md)|Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação. Herdado de [MyFace](../resources/itemfacet.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que modificou a entidade pela última vez. Herdado de [MyFace](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Fornece o dateTimeOffset para quando a entidade foi criada. Herdado de [MyFace](../resources/itemfacet.md).|
|source|[personDataSource](../resources/persondatasource.md)|Onde os valores são originados se forem sincronizados a partir de outro serviço. Herdado de [MyFace](../resources/itemfacet.md).|
|webUrl|String|Contém um link para o próprio site.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.personWebsite",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.personWebsite",
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
  "description": "String",
  "displayName": "String",
  "webUrl": "String"
}
```
