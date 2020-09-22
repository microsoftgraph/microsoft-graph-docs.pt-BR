---
title: tipo de recurso personCertification
description: tipo de recurso personCertification
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: b6f7349d5c279b00e504ca93945c5a2f3b8fbc73
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997932"
---
# <a name="personcertification-resource-type"></a>tipo de recurso personCertification

Namespace: microsoft.graph

Representa uma certificação ou designação que foi associada ao [perfil](../resources/profile.md)de um usuário.

Herda de [Myfacet](../resources/itemfacet.md).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar certificações](../api/profile-list-certifications.md)|coleção [personCertification](../resources/personcertification.md)|Obtenha os recursos personCertification da propriedade de navegação certificações.|
|[Criar personCertification](../api/profile-post-certifications.md)|[personCertification](../resources/personcertification.md)|Criar um novo objeto personCertification.|
|[Obter personCertification](../api/personCertification-get.md)|[personCertification](../resources/personcertification.md)|Leia as propriedades e os relacionamentos de um objeto [personCertification](../resources/personcertification.md) .|
|[Atualizar personCertification](../api/personCertification-update.md)|[personCertification](../resources/personcertification.md)|Atualiza as propriedades de um objeto [personCertification](../resources/personcertification.md) .|
|[Excluir personCertification](../api/personCertification-delete.md)|Nenhum|Exclui um objeto [personCertification](../resources/personcertification.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowedAudiences|String|As audiências que podem ver os valores contidos na entidade. Herdado de [MyFace](../resources/itemfacet.md). Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|Certification  |String      |O identificador de referência para a certificação. |
|createdBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que criou a entidade. Herdado de [MyFace](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Fornece o dateTimeOffset para quando a entidade foi criada. Herdado de [MyFace](../resources/itemfacet.md).|
|description      |String      |Descrição da certificação.                   |
|displayName      |String      |Título da certificação.                         |
|endDate          |Data        |A data em que a certificação expira.            |
|id|String|Identificador usado para o endereçamento individual da entidade. Herdado da [entidade](../resources/entity.md)|
|fracassa|[inferenceData](../resources/inferencedata.md)|Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação. Herdado de [MyFace](../resources/itemfacet.md).|
|issuedDate       |Data        |A data em que a certificação foi emitida.         |
|issuingAuthority |String      |Autoridade que atribuiu a certificação.          |
|issuingCompany   |String      |Empresa que concedeu a certificação.          |
|lastModifiedBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que modificou a entidade pela última vez. Herdado de [MyFace](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Fornece o dateTimeOffset para quando a entidade foi criada. Herdado de [MyFace](../resources/itemfacet.md).|
|source|[personDataSource](../resources/persondatasource.md)|Onde os valores são originados se forem sincronizados a partir de outro serviço. Herdado de [MyFace](../resources/itemfacet.md).|
|startDate        |Data        |A data em que a certificação se tornou válida.       |
|thumbnailUrl     |String      |URL que faz referência a uma miniatura da certificação.   |
|webUrl           |String      |URL que faz referência à certificação.                  |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.personCertification",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.personCertification",
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
  "certificationId": "String",
  "description": "String",
  "displayName": "String",
  "endDate": "Date",
  "issuedDate": "Date",
  "issuingAuthority": "String",
  "issuingCompany": "String",
  "startDate": "Date",
  "thumbnailUrl": "String",
  "webUrl": "String"
}
```


