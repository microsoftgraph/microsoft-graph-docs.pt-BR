---
title: tipo de recurso webaccount
description: tipo de recurso webaccount
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 29d66809d14cfc72d43286aef801490cef20cb9d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057673"
---
# <a name="webaccount-resource-type"></a>tipo de recurso webaccount

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa contas da Web que o usuário indicou que usa ou adicionou ao [perfil](profile.md)do usuário.

Esse tipo de recurso herda de [Myfacet](itemfacet.md).

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar contas da webaccount](../api/profile-list-webaccounts.md)|coleção [Webaccount](../resources/webaccount.md)|Obtenha os recursos da conta da webaccount da propriedade de navegação webaccounts.|
|[Criar conta da](../api/profile-post-webaccounts.md)|[conta da](../resources/webaccount.md)|Criar um novo objeto webaccount.|
|[Obter webaccount](../api/webaccount-get.md)|[conta da](../resources/webaccount.md)|Leia as propriedades e os relacionamentos de um objeto [webaccount](../resources/webaccount.md) .|
|[Atualizar webaccount](../api/webaccount-update.md)|[conta da](../resources/webaccount.md)|Atualizar as propriedades de um objeto [webaccount](../resources/webaccount.md) .|
|[Excluir conta da](../api/webaccount-delete.md)|Nenhum|Exclui um objeto [webaccount](../resources/webaccount.md) .|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowedAudiences|Cadeia de caracteres|As audiências que podem ver os valores contidos na entidade. Herdado de [MyFace](../resources/itemfacet.md). Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|createdBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que criou a entidade. Herdado de [MyFace](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Fornece o dateTimeOffset para quando a entidade foi criada. Herdado de [MyFace](../resources/itemfacet.md).|
|description|String|Contém a descrição que o usuário forneceu para a conta no serviço que está sendo referenciado.|
|id|Cadeia de caracteres|Identificador usado para o endereçamento individual da entidade. Herdado da [entidade](../resources/entity.md)|
|fracassa|[inferenceData](../resources/inferencedata.md)|Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação. Herdado de [MyFace](../resources/itemfacet.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que modificou a entidade pela última vez. Herdado de [MyFace](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Fornece o dateTimeOffset para quando a entidade foi criada. Herdado de [MyFace](../resources/itemfacet.md).|
|service|[Informações sobre o](../resources/serviceinformation.md)| Contém detalhes básicos sobre o serviço que está sendo associado. |
|source|[personDataSource](../resources/persondatasource.md)|Onde os valores são originados se forem sincronizados a partir de outro serviço. Herdado de [MyFace](../resources/itemfacet.md).|
|statusMessage|Cadeia de caracteres|Contém uma mensagem de status do serviço de nuvem, se fornecido ou sincronizado. |
|userId|Cadeia de caracteres|O nome de usuário exibido para a conta da Web.  |
|webUrl|String|Contém um link para o perfil do usuário no serviço de nuvem, se houver um.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.webAccount",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.webAccount",
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
  "userId": "String",
  "service": {
    "@odata.type": "microsoft.graph.serviceInformation"
  },
  "statusMessage": "String",
  "webUrl": "String"
}
```


