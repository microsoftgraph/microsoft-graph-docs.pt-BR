---
title: Tipo de recurso do ponto de extremidade
description: Os pontos de extremidade representam URLs para recursos associados a uma entidade.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: groups
author: psaffaie
ms.openlocfilehash: fef9ce8b89d83df87751ad93bc7feaa7ccc31b46
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64588047"
---
# <a name="endpoint-resource-type"></a>Tipo de recurso do ponto de extremidade

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Os pontos de extremidade representam URLs para recursos associados a uma entidade. Por exemplo, quando um novo grupo Microsoft 365 é criado, recursos adicionais também são criados como parte do Microsoft 365 grupo. Isso inclui coisas como uma caixa de correio de grupo para conversas e uma pasta de OneDrive para documentos e arquivos. Mais informações sobre esses Microsoft 365 de grupo, incluindo suas URLs de recurso associadas agora podem ser _lidas_ usando a navegação de pontos de extremidade no tipo de recurso do grupo. Isso permite que os aplicativos compreendam esses recursos e até mesmo insembutam as experiências de URL de recursos em suas próprias experiências.

## <a name="methods"></a>Métodos

| Método                                           | Tipo de retorno                        | Descrição                                              |
| :----------------------------------------------- | :--------------------------------- | :------------------------------------------------------- |
| [Listar pontos de extremidade](../api/group-list-endpoints.md) | conjunto [Ponto de extremidade](endpoint.md) | Obtenha uma coleção de o objeto ponto de extremidade.                       |
| [Obter o ponto de extremidade](../api/endpoint-get.md)           | [Ponto de extremidade](endpoint.md)            | Leia as propriedades e os relacionamentos do objeto ponto de extremidade. |

## <a name="properties"></a>Propriedades

| Propriedade           | Tipo   | Descrição                                                                                                                      |
| :----------------- | :----- | :------------------------------------------------------------------------------------------------------------------------------- |
| capability         | Cadeia de caracteres | Descreve a funcionalidade associada a esse recurso. (por exemplo, mensagens, conversas etc.) Não anulada. Somente leitura.    |
| id                 | Cadeia de caracteres | Identificador exclusivo do ponto de extremidade; Chave. Não anulável. Somente leitura.                                                                |
| providerId         | String | ID do aplicativo do serviço subjacente de publicação. Não anulável. Somente leitura.                                                    |
| providerName       | Cadeia de caracteres | Nome do serviço subjacente de publicação. Somente leitura.                                                                            |
| providerResourceId | String | Para Microsoft 365 grupos, isso é definido como um nome conhecido para o recurso (por exemplo, Yammer. FeedURL etc.). Não anulável. Somente leitura. |
| uri                | Cadeia de caracteres | URL do recurso publicado. Não anulável. Somente leitura.                                                                          |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.endpoint"
}-->

```json
{
  "capability": "String",
  "id": "String (identifier)",
  "providerId": "String",
  "providerName": "String",
  "providerResourceId": "String",
  "uri": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Endpoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
