---
title: Tipo de recurso de ponto de extremidade
description: 'Pontos de extremidade representam URLs para recursos associados a uma entidade.  Por exemplo, quando um novo grupo do Office 365 é criado, recursos adicionais também são criados como parte do grupo do Office 365. Eles incluem coisas como uma caixa de correio de grupo para conversas e uma pasta de OneDrive de grupo para documentos e arquivos. Mais informações sobre esses recursos de grupo do Office 365, incluindo suas URLs de recurso associado agora podem ser lido usando a navegação de *pontos de extremidade* no tipo de recurso de grupo. Isso permite que aplicativos entender esses recursos e até mesmo incorporar o recurso que URL experiências em suas próprias experiências. '
localization_priority: Normal
ms.openlocfilehash: 5a342bee0a1918eb142542693198173239d1b3c7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871279"
---
# <a name="endpoint-resource-type"></a>Tipo de recurso de ponto de extremidade

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Pontos de extremidade representam URLs para recursos associados a uma entidade.  Por exemplo, quando um novo grupo do Office 365 é criado, recursos adicionais também são criados como parte do grupo do Office 365. Eles incluem coisas como uma caixa de correio de grupo para conversas e uma pasta de OneDrive de grupo para documentos e arquivos. Mais informações sobre esses recursos de grupo do Office 365, incluindo suas URLs de recurso associado agora podem ser lido usando a navegação de *pontos de extremidade* no tipo de recurso de grupo. Isso permite que aplicativos entender esses recursos e até mesmo incorporar o recurso que URL experiências em suas próprias experiências. 

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Lista de pontos de extremidade](../api/group-list-endpoints.md) |Coleção de [ponto de extremidade](endpoint.md)| Obtenha uma coleção de objetos de ponto de extremidade. |
|[Obtenha o ponto de extremidade](../api/endpoint-get.md) | [Ponto de extremidade](endpoint.md) |Leia as propriedades e os relacionamentos de um objeto de ponto de extremidade.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| recurso     | Cadeia de caracteres  | Descreve o recurso que está associado a esse recurso. (por exemplo, mensagens, conversas, etc.)  Não são nulas. Somente leitura. |
| id             | Cadeia de caracteres  | Identificador exclusivo para o ponto de extremidade; Tecla. Não anulável. Somente leitura.|
| providerId     | Cadeia de caracteres  | Id do aplicativo de publicação do serviço subjacente. Não anulável. Somente leitura.|
| providerName   | Cadeia de caracteres  | Nome da publicação do serviço subjacente. Somente leitura.|
| providerResourceId|Cadeia de caracteres| Para grupos do Office 365, isso é definido como um nome conhecido do recurso (por exemplo, Yammer.FeedURL etc.). Não anulável. Somente leitura.|
| URI            | Cadeia de caracteres  | URL do recurso publicado. Não anulável. Somente leitura.|

## <a name="relationships"></a>Relações

Nenhum


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.Endpoint"
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
<!-- {
  "type": "#page.annotation",
  "description": "Endpoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
