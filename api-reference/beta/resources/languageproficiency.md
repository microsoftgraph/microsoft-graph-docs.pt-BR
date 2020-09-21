---
title: tipo de recurso languageProficiency
description: tipo de recurso languageProficiency
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 95fa1f1ebbd5022fe9e20c6f867706ce6402f398
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029223"
---
# <a name="languageproficiency-resource-type"></a>tipo de recurso languageProficiency

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações detalhadas sobre os idiomas que um usuário adicionou ao [perfil](profile.md).

Herda de [Myfacet](itemFacet.md).

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Idiomas de lista](../api/profile-list-languages.md)|coleção [languageProficiency](../resources/languageproficiency.md)|Obtenha os recursos languageProficiency da propriedade de navegação Languages.|
|[Criar languageProficiency](../api/profile-post-languages.md)|[languageProficiency](../resources/languageproficiency.md)|Criar um novo objeto languageProficiency.|
|[Obter languageProficiency](../api/languageproficiency-get.md)|[languageProficiency](../resources/languageproficiency.md)|Leia as propriedades e os relacionamentos de um objeto [languageProficiency](../resources/languageproficiency.md) .|
|[Atualizar languageProficiency](../api/languageproficiency-update.md)|[languageProficiency](../resources/languageproficiency.md)|Atualiza as propriedades de um objeto [languageProficiency](../resources/languageproficiency.md) .|
|[Excluir languageProficiency](../api/languageproficiency-delete.md)|Nenhum|Exclui um objeto [languageProficiency](../resources/languageproficiency.md) .|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowedAudiences|String|As audiências que podem ver os valores contidos na entidade. Herdado de [MyFace](../resources/itemfacet.md). Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|createdBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que criou a entidade. Herdado de [MyFace](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Fornece o dateTimeOffset para quando a entidade foi criada. Herdado de [MyFace](../resources/itemfacet.md).|
|displayName|String|Contém o nome de formato longo para o idioma. |
|id|String|Identificador usado para o endereçamento individual da entidade. Herdado da [entidade](../resources/entity.md)|
|fracassa|[inferenceData](../resources/inferencedata.md)|Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação. Herdado de [MyFace](../resources/itemfacet.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que modificou a entidade pela última vez. Herdado de [MyFace](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Fornece o dateTimeOffset para quando a entidade foi criada. Herdado de [MyFace](../resources/itemfacet.md).|
|Converte|languageProficiencyLevel|Representa os usuários que estão lendo a compreensão do idioma representado pelo objeto. Os valores possíveis são: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.|
|source|[personDataSource](../resources/persondatasource.md)|Onde os valores são originados se forem sincronizados a partir de outro serviço. Herdado de [MyFace](../resources/itemfacet.md).|
|idioma|languageProficiencyLevel|Representa a proficiência dos usuários falada sobre o idioma representado pelo objeto. Os valores possíveis são: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.|
|tag|String|Contém o nome BCP47 de quatro caracteres para o idioma (en-US, no-NB, en-AU).|
|pré-gravados|languageProficiencyLevel|Representa a proficiência dos usuários gravados para o idioma representado pelo objeto. Os valores possíveis são: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.languageProficiency",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.languageProficiency",
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
  "tag": "String",
  "spoken": "String",
  "written": "String",
  "reading": "String"
}
```


