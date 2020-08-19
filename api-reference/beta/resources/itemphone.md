---
title: tipo de recurso de Tel.
description: tipo de recurso de Tel.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 0c36ea4d861738316a3ce6593c12a79a59d97c68
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809401"
---
# <a name="itemphone-resource-type"></a>tipo de recurso de Tel.

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações detalhadas sobre números de telefone associados a um usuário em vários serviços.

Herda de [Myfacet](../resources/itemfacet.md).

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar telefones](../api/profile-list-phones.md)|coleção [Multiphone](../resources/itemphone.md)|Obtenha os recursos de telefonia da propriedade de navegação phones.|
|[Criar um número de telefone](../api/profile-post-phones.md)|[Número de telefone](../resources/itemphone.md)|Criar um novo objeto MyPhone.|
|[Obter o número de telefone](../api/itemphone-get.md)|[Número de telefone](../resources/itemphone.md)|Leia as propriedades e os relacionamentos de um objeto [MyPhone](../resources/itemphone.md) .|
|[Atualizar o número de telefone](../api/itemphone-update.md)|[Número de telefone](../resources/itemphone.md)|Atualiza as propriedades de um objeto [MyPhone](../resources/itemphone.md) .|
|[Excluir o número de telefone](../api/itemphone-delete.md)|Nenhum|Exclui um objeto [MyPhone](../resources/itemphone.md) .|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowedAudiences|String|As audiências que podem ver os valores contidos na entidade. Herdado de [MyFace](../resources/itemfacet.md). Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|createdBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que criou a entidade. Herdado de [MyFace](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Fornece o dateTimeOffset para quando a entidade foi criada. Herdado de [MyFace](../resources/itemfacet.md).|
|displayName|String|Nome amigável o usuário atribuiu este número de telefone. |
|id|String|Identificador usado para o endereçamento individual da entidade. Herdado da [entidade](../resources/entity.md)|
|fracassa|[inferenceData](../resources/inferencedata.md)|Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação. Herdado de [MyFace](../resources/itemfacet.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que modificou a entidade pela última vez. Herdado de [MyFace](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Fornece o dateTimeOffset para quando a entidade foi criada. Herdado de [MyFace](../resources/itemfacet.md).|
|number|String|Número de telefone fornecido pelo usuário.|
|source|[personDataSource](../resources/persondatasource.md)|Onde os valores são originados se forem sincronizados a partir de outro serviço. Herdado de [MyFace](../resources/itemfacet.md).|
|type|PhoneType|O tipo de número de telefone dentro do objeto. Os valores possíveis são: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.itemPhone",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.itemPhone",
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
  "displayName": "String",
  "type": "String",
  "number": "String"
}
```
