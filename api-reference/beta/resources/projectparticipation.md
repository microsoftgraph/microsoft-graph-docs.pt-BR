---
title: tipo de recurso projectParticipation
description: tipo de recurso projectParticipation
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 2e292795eeccc25029063763c0e1a2c4883009d7
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43227677"
---
# <a name="projectparticipation-resource-type"></a>tipo de recurso projectParticipation

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações detalhadas sobre os projetos associados a um usuário.

Herda de [Myfacet](itemfacet.md).

## <a name="methods"></a>Métodos

| Método                                                                | Tipo de retorno                                     | Descrição                                                                 |
|:----------------------------------------------------------------------|:------------------------------------------------|:----------------------------------------------------------------------------|
| [Obter projectParticipation](../api/projectparticipation-get.md)        | [projectParticipation](projectparticipation.md) | Leia as propriedades e os relacionamentos de um objeto **projectParticipation** . |
| [Atualizar projectParticipation](../api/projectparticipation-update.md)  | [projectParticipation](projectparticipation.md) | Atualizar um objeto **projectParticipation** .                                   |
| [Excluir projectParticipation](../api/projectparticipation-delete.md)  | Nenhum.                                           | Excluir um objeto **projectParticipation** .                                   |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo                                        | Descrição                                                                                                |
|:-------------|:--------------------------------------------|:-----------------------------------------------------------------------------------------------------------|
|categories    | String collection                           | Contém categorias que um usuário associou ao projeto (por exemplo, transformação digital, Rig óleo). |
|clientes        |[companyDetail](companydetail.md)            | Contém informações detalhadas sobre o cliente para o qual o projeto foi.                                        |
|conhecidos    |coleção [relatedPerson](relatedperson.md) | Lista as pessoas que também trabalharam no projeto.                                                              |
|detalhada        |[positionDetail](positiondetail.md)          | Contém detalhes sobre a função do usuário no projeto.                                                      |
|displayName   |String                                       |Contém um nome amigável para o projeto.                                                                   |
|responsáveis      |coleção [relatedPerson](relatedperson.md) | A pessoa ou as pessoas que patrocinaram o projeto.                                                            |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.projectParticipation",
  "baseType": ""
}-->

```json
{
  "categories": ["String"],
  "client": {"@odata.type": "microsoft.graph.companyDetail"},
  "colleagues": [{"@odata.type": "microsoft.graph.relatedPerson"}],
  "detail": {"@odata.type": "microsoft.graph.positionDetail"},
  "displayName": "String",
  "sponsors": [{"@odata.type": "microsoft.graph.relatedPerson"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "projectParticipation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
