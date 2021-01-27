---
title: Tipo de recurso Endpoint
description: Os pontos de extremidade representam URLs de recursos associados a uma entidade.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: yyuank
ms.openlocfilehash: 47bef2bfa14fb8a00fd1ca2356d7f880ff3207d6
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013594"
---
# <a name="endpoint-resource-type"></a>Tipo de recurso Endpoint

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Os pontos de extremidade representam URLs de recursos associados a uma entidade.  Por exemplo, quando um novo grupo do Microsoft 365 é criado, recursos adicionais também são criados como parte do grupo do Microsoft 365. Isso inclui coisas como uma caixa de correio de grupo para conversas e uma pasta do OneDrive de grupo para documentos e arquivos. Mais informações sobre esses recursos de grupo do Microsoft 365, incluindo suas URLs de recursos associadas agora podem ser *lidas* usando a navegação de pontos de extremidade no tipo de recurso do grupo. Isso permite que os aplicativos compreendam esses recursos e, até mesmo, incorporam as experiências de URL do recurso em suas próprias experiências.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar pontos de extremidade](../api/group-list-endpoints.md) |conjunto [Ponto de extremidade](endpoint.md)| Obtenha uma coleção de o objeto ponto de extremidade. |
|[Obter o ponto de extremidade](../api/endpoint-get.md) | [Ponto de extremidade](endpoint.md) |Leia as propriedades e os relacionamentos do objeto ponto de extremidade.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| capability     | Cadeia de caracteres  | Descreve a funcionalidade associada a esse recurso. (por exemplo, mensagens, conversas, etc.)  Não anulada. Somente leitura. |
| id             | Cadeia de caracteres  | Identificador exclusivo do ponto de extremidade; Tecla. Não anulável. Somente leitura.|
| providerId     | Cadeia de caracteres  | ID do aplicativo do serviço subjacente de publicação. Não anulável. Somente leitura.|
| providerName   | Cadeia de caracteres  | Nome do serviço subjacente de publicação. Somente leitura.|
| providerResourceId|Cadeia de caracteres| Para grupos do Microsoft 365, isso é definido como um nome conhecido para o recurso (por exemplo, Yammer.FeedURL etc.). Não anulável. Somente leitura.|
| uri            | Cadeia de caracteres  | URL do recurso publicado. Não anulável. Somente leitura.|

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


