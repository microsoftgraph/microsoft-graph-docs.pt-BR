---
title: tipo de recurso de patente
description: tipo de recurso de patente
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 7e6732a53f841902422348f90dada22174813b39
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089287"
---
# <a name="itempatent-resource-type"></a>tipo de recurso de patente
 
Namespace: microsoft.graph

Representa uma patente concedida ou em um campo que foi adicionada ao [perfil](../resources/profile.md)de um usuário.

Herda de [Myfacet](../resources/itemfacet.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar patentes](../api/profile-list-patents.md)|coleção [Ispatenteado](../resources/itempatent.md)|Obtenha os recursos de patente da propriedade de navegação patentes.|
|[Criar ispatente](../api/profile-post-patents.md)|[Patente](../resources/itempatent.md)|Criar um novo objeto de patente.|
|[Obter ispatente](../api/itempatent-get.md)|[Patente](../resources/itempatent.md)|Leia as propriedades e os relacionamentos de um objeto de [patente](../resources/itempatent.md) .|
|[Atualizar a ispatente](../api/itempatent-update.md)|[Patente](../resources/itempatent.md)|Atualiza as propriedades de um objeto [dopatente](../resources/itempatent.md) .|
|[Excluir a ispatente](../api/itempatent-delete.md)|Nenhum|Exclui um objeto [ispatente](../resources/itempatent.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowedAudiences|Cadeia de caracteres|As audiências que podem ver os valores contidos na entidade. Herdado de [MyFace](../resources/itemfacet.md). Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|createdBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que criou a entidade. Herdado de [MyFace](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Fornece o dateTimeOffset para quando a entidade foi criada. Herdado de [MyFace](../resources/itemfacet.md).|
|description|Cadeia de caracteres|Descpription da patente ou do arquivamento. |
|displayName|Cadeia de caracteres|Título da patente ou do arquivamento. |
|id|Cadeia de caracteres|Identificador usado para o endereçamento individual da entidade. Herdado da [entidade](../resources/entity.md)|
|fracassa|[inferenceData](../resources/inferencedata.md)|Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação. Herdado de [MyFace](../resources/itemfacet.md).|
|ispending        |Boolean     |Indica que a patente está pendente.        |
|issuedDate       |Data        |A data em que a patente foi concedida.   |
|issuingAuthority |Cadeia de caracteres      |Autoridade que concedeu a patente.     |
|lastModifiedBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que modificou a entidade pela última vez. Herdado de [MyFace](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Fornece o dateTimeOffset para quando a entidade foi criada. Herdado de [MyFace](../resources/itemfacet.md).|
|number           |Cadeia de caracteres      |O número de patente.                      |
|source|[personDataSource](../resources/persondatasource.md)|Onde os valores são originados se forem sincronizados a partir de outro serviço. Herdado de [MyFace](../resources/itemfacet.md).|
|webUrl           |String      |URL que faz referência à patente ou ao arquivamento. |


## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.itemPatent",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.itemPatent",
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
  "description": "String",
  "displayName": "String",
  "isPending": "Boolean",
  "issuedDate": "Date",
  "issuingAuthority": "String",
  "number": "String",
  "webUrl": "String"
}
```


