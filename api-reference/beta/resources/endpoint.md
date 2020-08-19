---
title: Tipo de recurso de ponto de extremidade
description: 'Os pontos de extremidade representam URLs para recursos associados a uma entidade.  Por exemplo, quando um novo grupo Microsoft 365 é criado, recursos adicionais também são criados como parte do grupo Microsoft 365. Isso inclui itens como uma caixa de correio de grupo para conversas e uma pasta do OneDrive de grupo para documentos e arquivos. Informações adicionais sobre esses recursos de grupo do Microsoft 365, incluindo suas URLs de recurso associadas, agora podem ser lidas usando a navegação de *pontos de extremidade* no tipo de recurso de grupo. Isso permite que os aplicativos entendam esses recursos e, até mesmo, incorpore as experiências de URL de recurso em suas próprias experiências. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: yyuank
ms.openlocfilehash: bb5af31f8cad2cf6fa738d55d13775d20a589b97
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806706"
---
# <a name="endpoint-resource-type"></a>Tipo de recurso de ponto de extremidade

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Os pontos de extremidade representam URLs para recursos associados a uma entidade.  Por exemplo, quando um novo grupo Microsoft 365 é criado, recursos adicionais também são criados como parte do grupo Microsoft 365. Isso inclui itens como uma caixa de correio de grupo para conversas e uma pasta do OneDrive de grupo para documentos e arquivos. Informações adicionais sobre esses recursos de grupo do Microsoft 365, incluindo suas URLs de recurso associadas, agora podem ser lidas usando a navegação de *pontos de extremidade* no tipo de recurso de grupo. Isso permite que os aplicativos entendam esses recursos e, até mesmo, incorpore as experiências de URL de recurso em suas próprias experiências.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar pontos de extremidade](../api/group-list-endpoints.md) |conjunto [Ponto de extremidade](endpoint.md)| Obtenha uma coleção de o objeto ponto de extremidade. |
|[Obter o ponto de extremidade](../api/endpoint-get.md) | [Ponto de extremidade](endpoint.md) |Leia as propriedades e os relacionamentos do objeto ponto de extremidade.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| função     | String  | Descreve o recurso que está associado a esse recurso. (por exemplo, mensagens, conversas etc.)  Não anulável. Somente leitura. |
| id             | String  | Identificador exclusivo do ponto de extremidade; Chaves. Não anulável. Somente leitura.|
| providerId     | String  | ID de aplicativo do serviço subjacente de publicação. Não anulável. Somente leitura.|
| providerName   | String  | Nome do serviço subjacente de publicação. Somente leitura.|
| providerResourceId|String| Para os grupos do Microsoft 365, isso é definido como um nome conhecido para o recurso (por exemplo, Yammer. FeedURL etc.). Não anulável. Somente leitura.|
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
  "suppressions": []
}
-->
