---
title: Tipo de recurso de ponto de extremidade
description: 'Pontos de extremidade representam URLs para recursos associados a uma entidade.  Por exemplo, quando um novo grupo do Office 365 é criado, recursos adicionais também são criados como parte do grupo do Office 365. Eles incluem coisas como uma caixa de correio de grupo para conversas e uma pasta de OneDrive de grupo para documentos e arquivos. Mais informações sobre esses recursos de grupo do Office 365, incluindo suas URLs de recurso associado agora podem ser lido usando a navegação de *pontos de extremidade* no tipo de recurso de grupo. Isso permite que aplicativos entender esses recursos e até mesmo incorporar o recurso que URL experiências em suas próprias experiências. '
localization_priority: Normal
ms.openlocfilehash: 39a6a2d8213e809f426c492654272aa994c25a6d
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574479"
---
# <a name="endpoint-resource-type"></a>Tipo de recurso de ponto de extremidade

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Pontos de extremidade representam URLs para recursos associados a uma entidade.  Por exemplo, quando um novo grupo do Office 365 é criado, recursos adicionais também são criados como parte do grupo do Office 365. Eles incluem coisas como uma caixa de correio de grupo para conversas e uma pasta de OneDrive de grupo para documentos e arquivos. Mais informações sobre esses recursos de grupo do Office 365, incluindo suas URLs de recurso associado agora podem ser lido usando a navegação de *pontos de extremidade* no tipo de recurso de grupo. Isso permite que aplicativos entender esses recursos e até mesmo incorporar o recurso que URL experiências em suas próprias experiências. 

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar pontos de extremidade](../api/group-list-endpoints.md) |conjunto [Ponto de extremidade](endpoint.md)| Obtenha uma coleção de o objeto ponto de extremidade. |
|[Obter o ponto de extremidade](../api/endpoint-get.md) | [Ponto de extremidade](endpoint.md) |Leia as propriedades e os relacionamentos do objeto ponto de extremidade.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| recurso     | String  | Descreve o recurso que está associado a esse recurso. (por exemplo, mensagens, conversas, etc.)  Não são nulas. Somente leitura. |
| id             | String  | Identificador exclusivo para o ponto de extremidade; Tecla. Não anulável. Somente leitura.|
| providerId     | String  | Id do aplicativo de publicação do serviço subjacente. Não anulável. Somente leitura.|
| providerName   | String  | Nome da publicação do serviço subjacente. Somente leitura.|
| providerResourceId|String| Para grupos do Office 365, isso é definido como um nome conhecido do recurso (por exemplo, Yammer.FeedURL etc.). Não anulável. Somente leitura.|
| URI            | String  | URL do recurso publicado. Não anulável. Somente leitura.|

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
  "suppressions": [
    "Error: /api-reference/beta/resources/endpoint.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
