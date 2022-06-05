---
title: Tipo de recurso personWebsite
description: Representa informações detalhadas sobre sites associados a um usuário em vários serviços.
ms.localizationpriority: medium
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: c26bda366fe03893e138551cb3ae3e8ab1efd8c8
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900468"
---
# <a name="personwebsite-resource-type"></a>Tipo de recurso personWebsite

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações detalhadas sobre sites associados a um usuário em vários serviços.

Herda de [itemFacet](itemfacet.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar sites](../api/profile-list-websites.md)|[coleção personWebsite](../resources/personwebsite.md)|Obtenha os recursos personWebsite da propriedade de navegação de sites.|
|[Criar personWebsite](../api/profile-post-websites.md)|[personWebsite](../resources/personwebsite.md)|Crie um novo objeto personWebsite.|
|[Obter personWebsite](../api/personwebsite-get.md)|[personWebsite](../resources/personwebsite.md)|Leia as propriedades e as relações de um [objeto personWebsite](../resources/personwebsite.md) .|
|[Atualizar personWebsite](../api/personwebsite-update.md)|[personWebsite](../resources/personwebsite.md)|Atualize as propriedades de um [objeto personWebsite](../resources/personwebsite.md) .|
|[Excluir personWebsite](../api/personwebsite-delete.md)|Nenhum|Exclui um [objeto personWebsite](../resources/personwebsite.md) .|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo              | Descrição                                                                                   |
|:-------------|:------------------|:----------------------------------------------------------------------------------------------|
|categories    |Coleção de cadeias de caracteres  | Contém categorias que um usuário associou ao site (por exemplo, receitas pessoais).  |
|descrição   |String             | Contém uma descrição do site.                                                        |
|displayName   |String             | Contém um nome amigável para o site.                                                     |
|webUrl        |String             | Contém um link para o próprio site.                                                        |

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


