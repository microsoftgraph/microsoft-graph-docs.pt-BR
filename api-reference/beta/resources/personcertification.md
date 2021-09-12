---
title: Tipo de recurso personCertification
description: Tipo de recurso personCertification
ms.localizationpriority: medium
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: ce360bd663549e7dc5fb0b9d9f1ccbce28f8dc15
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59017097"
---
# <a name="personcertification-resource-type"></a>Tipo de recurso personCertification

Namespace: microsoft.graph

Representa uma certificação ou designação que foi associada ao perfil de um [usuário.](../resources/profile.md)

Herda do [itemFacet](../resources/itemfacet.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar certificações](../api/profile-list-certifications.md)|[Coleção personCertification](../resources/personcertification.md)|Obter os recursos personCertification da propriedade de navegação de certificações.|
|[Criar personCertification](../api/profile-post-certifications.md)|[personCertification](../resources/personcertification.md)|Crie um novo objeto personCertification.|
|[Obter personCertification](../api/personCertification-get.md)|[personCertification](../resources/personcertification.md)|Leia as propriedades e as relações de um [objeto personCertification.](../resources/personcertification.md)|
|[Atualizar personCertification](../api/personCertification-update.md)|[personCertification](../resources/personcertification.md)|Atualize as propriedades de um [objeto personCertification.](../resources/personcertification.md)|
|[Excluir personCertification](../api/personCertification-delete.md)|None|Exclui um [objeto personCertification.](../resources/personcertification.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowedAudiences|String|As audiências que são capazes de ver os valores contidos na entidade. Herdado [do itemFacet](../resources/itemfacet.md). Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|certificationId  |Cadeia de caracteres      |O identificador referencial para a certificação. |
|createdBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que criou a entidade. Herdado [do itemFacet](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Fornece a dataTimeOffset para quando a entidade foi criada. Herdado [do itemFacet](../resources/itemfacet.md).|
|description      |String      |Descrição da certificação.                   |
|displayName      |Cadeia de caracteres      |Título da certificação.                         |
|endDate          |Data        |A data em que a certificação expira.            |
|id|String|Identificador usado para endereçamento individual da entidade. Herdado da [entidade](../resources/entity.md)|
|inferência|[inferenceData](../resources/inferencedata.md)|Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação. Herdado [do itemFacet](../resources/itemfacet.md).|
|issuedDate       |Data        |A data em que a certificação foi emitida.         |
|issuingAuthority |Cadeia de caracteres      |Autoridade que concedeu a certificação.          |
|emissãoCompany   |Cadeia de caracteres      |Empresa que concedeu a certificação.          |
|lastModifiedBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que modificou a entidade pela última vez. Herdado [do itemFacet](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Fornece a dataTimeOffset para quando a entidade foi criada. Herdado [do itemFacet](../resources/itemfacet.md).|
|source|[personDataSource](../resources/persondatasource.md)|Onde os valores se originaram se sincronizados de outro serviço. Herdado [do itemFacet](../resources/itemfacet.md).|
|startDate        |Data        |A data em que a certificação se tornou válida.       |
|thumbnailUrl     |String      |URL fazendo referência a uma miniatura da certificação.   |
|webUrl           |String      |URL fazendo referência à certificação.                  |

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


