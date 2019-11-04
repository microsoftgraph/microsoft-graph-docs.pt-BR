---
title: tipo de recurso webaccount
description: tipo de recurso webaccount
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 414e3f491736f51ee670390519241110bc81f66e
ms.sourcegitcommit: dd94c3a0f7663699825b6dbc119cdcef494cd130
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2019
ms.locfileid: "37950352"
---
# <a name="webaccount-resource-type"></a>tipo de recurso webaccount

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa contas da Web que o usuário indicou que usa ou adicionou ao [perfil](profile.md)do usuário.

Esse tipo de recurso herda de [Myfacet](itemfacet.md).

## <a name="methods"></a>Métodos

| Método                                     | Tipo de retorno                 | Descrição                                             |
|:-------------------------------------------|:----------------------------|:--------------------------------------------------------|
| [Obter webaccount](../api/webaccount-get.md) | [conta da](webaccount.md) | Leia as propriedades e os relacionamentos de um objeto **webaccount** . |
| [Atualizar webaccount](../api/webaccount-update.md)      | [conta da](webaccount.md) | Atualize um objeto **webaccount** .                               |
| [Excluir conta da](../api/webaccount-delete.md)      | Nenhum                        | Excluir um objeto **webaccount** .                               |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo                                      | Descrição                                                                                    |
|:-------------|:------------------------------------------|:-----------------------------------------------------------------------------------------------|
|description   |String                                     | Contém a descrição que o usuário forneceu para a conta no serviço que está sendo referenciado.|
|service       |[Informações sobre o](serviceinformation.md)| Contém detalhes básicos sobre o serviço que está sendo associado.                              |
|statusMessage |Cadeia de caracteres                                     | Contém uma mensagem de status do serviço de nuvem, se fornecido ou sincronizado.                  |
|userId        |Cadeia de caracteres                                     | O nome de usuário exibido para a conta da Web.                                    |
|webUrl        |String                                     | Contém um link para o perfil do usuário no serviço de nuvem, se houver um.                       |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.webAccount",
  "baseType": ""
}-->

```json
{
  "description": "String",
  "service": {"@odata.type": "microsoft.graph.serviceInformation"},
  "statusMessage": "String",
  "userId": "String",
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "webAccount resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
