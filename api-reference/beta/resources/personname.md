---
title: tipo de recurso PersonName
description: tipo de recurso PersonName
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 1f1817e3d9868e47158453113f4781ebfc155f86
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997939"
---
# <a name="personname-resource-type"></a>tipo de recurso PersonName

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as informações de nome estendidas fornecidas pelo usuário ou que elas associaram ao [perfil](../resources/profile.md).

Herda de [Myfacet](../resources/itemfacet.md).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Nomes da lista](../api/profile-list-names.md)|coleção [PersonName](../resources/personname.md)|Obtenha os recursos PersonName da propriedade de navegação names.|
|[Criar PersonName](../api/profile-post-names.md)|[personName](../resources/personname.md)|Crie um novo objeto [PersonName](../resources/personname.md) da propriedade de navegação names.|
|[Obter PersonName](../api/personname-get.md)|[personName](../resources/personname.md)|Leia as propriedades e os relacionamentos de um objeto [PersonName](../resources/personname.md) .|
|[Atualizar PersonName](../api/personname-update.md)|[personName](../resources/personname.md)|Atualiza as propriedades de um objeto [PersonName](../resources/personname.md) .|
|[Excluir PersonName](../api/personname-delete.md)|Nenhum|Exclui um objeto [PersonName](../resources/personname.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowedAudiences|String|As audiências que podem ver os valores contidos na entidade. Herdado de [MyFace](../resources/itemfacet.md). Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|createdBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que criou a entidade. Herdado de [MyFace](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Fornece o dateTimeOffset para quando a entidade foi criada. Herdado de [MyFace](../resources/itemfacet.md).|
|displayName|String|Fornece uma renderização ordenada de firstName e lastName, dependendo da localidade do usuário ou de seu dispositivo.|
|primeiro|String|Nome do usuário.|
|id|String|Identificador usado para o endereçamento individual da entidade. Herdado da [entidade](../resources/entity.md)|
|fracassa|[inferenceData](../resources/inferencedata.md)|Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação. Herdado de [MyFace](../resources/itemfacet.md).|
|initials|String|Iniciais do usuário.|
|languageTag|String|Contém o nome do idioma (en-US, no-NB, en-AU) após o formato BCP47 da IETF.   |
|durar|String|Sobrenome do usuário.|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que modificou a entidade pela última vez. Herdado de [MyFace](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Fornece o dateTimeOffset para quando a entidade foi criada. Herdado de [MyFace](../resources/itemfacet.md).|
|Virgem|String|Nome de solteira do usuário. |
|middleware|String|Nome do meio do usuário.|
|apelido|String|Apelido do usuário.|
|pronúncia|[yomiPersonName](../resources/yomipersonname.md)|Orientações sobre como pronunciar o nome dos usuários.|
|source|[personDataSource](../resources/persondatasource.md)|Onde os valores são originados se forem sincronizados a partir de outro serviço. Herdado de [MyFace](../resources/itemfacet.md).|
|sufixo|String|Designadores usados após o nome dos usuários (por exemplo: PhD).  |
|title|String|Honorifics usado para prefixar um nome de usuário (por exemplo: Dr, Sir, Madam, Sra.)|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.personName",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.personName",
  "id": "e13f7a4d-303c-464f-a6af-80ea18eb74f3",
  "allowedAudiences": "organization",
  "inference": {
    "@odata.type": "microsoft.graph.inferenceData"
  },
  "createdDateTime": "2020-07-06T06:34:12.2294868Z",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "2020-07-06T06:34:12.2294868Z",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "source": {
    "@odata.type": "microsoft.graph.personDataSource"
  },
  "displayName": "Innocenty Popov",
  "first": "Innocenty",
  "initials": "IP",
  "last": "Popov",
  "languageTag": "en-US",
  "maiden": null,
  "middle": null,
  "nickname": "Kesha",
  "suffix": null,
  "title": null,
  "pronunciation": {
    "@odata.type": "microsoft.graph.yomiPersonName"
  }
}
```

