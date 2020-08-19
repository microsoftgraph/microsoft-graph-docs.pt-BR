---
title: tipo de recurso personAnniversary
description: tipo de recurso personAnniversary
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 6d59ee0d95b4f5ad0a79ad86476e971e5f9e9896
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812489"
---
# <a name="personanniversary-resource-type"></a>tipo de recurso personAnniversary

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes de datas significativas associadas a uma pessoa em um [perfil](profile.md)de usuário.

Herda de [Myfacet](itemFacet.md).

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar aniversários](../api/profile-list-anniversaries.md)|coleção [personAnniversary](../resources/personanniversary.md)|Obtenha os recursos personAnniversary da propriedade de navegação aniversários.|
|[Criar personAnniversary](../api/profile-post-anniversaries.md)|[personAnniversary](../resources/personanniversary.md)|Criar um novo objeto personAnniversary.|
|[Obter personAnniversary](../api/personanniversary-get.md)|[personAnniversary](../resources/personanniversary.md)|Leia as propriedades e os relacionamentos de um objeto [personAnniversary](../resources/personanniversary.md) .|
|[Atualizar personAnniversary](../api/personanniversary-update.md)|[personAnniversary](../resources/personanniversary.md)|Atualiza as propriedades de um objeto [personAnniversary](../resources/personanniversary.md) .|
|[Excluir personAnniversary](../api/personanniversary-delete.md)|Nenhum|Exclui um objeto [personAnniversary](../resources/personanniversary.md) .|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowedAudiences|String|As audiências que podem ver os valores contidos na entidade. Herdado de [MyFace](../resources/itemfacet.md). Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|createdBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que criou a entidade. Herdado de [MyFace](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Fornece o dateTimeOffset para quando a entidade foi criada. Herdado de [MyFace](../resources/itemfacet.md).|
|data|Data|Contém a data associada ao tipo de aniversário.|
|id|String|Identificador usado para o endereçamento individual da entidade. Herdado da [entidade](../resources/entity.md)|
|fracassa|[inferenceData](../resources/inferencedata.md)|Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação. Herdado de [MyFace](../resources/itemfacet.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que modificou a entidade pela última vez. Herdado de [MyFace](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Fornece o dateTimeOffset para quando a entidade foi criada. Herdado de [MyFace](../resources/itemfacet.md).|
|source|[personDataSource](../resources/persondatasource.md)|Onde os valores são originados se forem sincronizados a partir de outro serviço. Herdado de [MyFace](../resources/itemfacet.md).|
|type|data especial|O tipo de aniversário que a data representa. Os valores possíveis são: `birthday`, `wedding`, `unknownFutureValue`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.personAnniversary",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.personAnniversary",
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
  "type": "String",
  "date": "Date"
}
```
