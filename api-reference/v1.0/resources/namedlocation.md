---
title: Tipo de recurso namedLocation
description: Esta é a classe base que representa um Azure Active Directory local nomeado. Locais nomeados são regras personalizadas que definem locais de rede que podem ser usados em uma política de Acesso Condicional.
ms.localizationpriority: medium
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 01825465c415ef3a769812896dbc80105c50ed68
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084269"
---
# <a name="namedlocation-resource-type"></a>Tipo de recurso namedLocation

Namespace: microsoft.graph

Esta é a classe base que representa um Azure Active Directory local nomeado. Locais nomeados são regras personalizadas que definem locais de rede que podem ser usados em uma política de Acesso Condicional.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar namedLocations](../api/conditionalaccessroot-list-namedlocations.md) | [coleção namedLocation](namedLocation.md) | Obter todos os **objetos namedLocation** na organização. |
| [Obter namedLocation](../api/namedlocation-get.md) | [namedLocation](namedlocation.md) | Leia as propriedades e as relações de um **objeto namedLocation.** |
| [Excluir namedLocation](../api/namedlocation-delete.md) | Nenhum(a) | Exclua **um objeto namedLocation.** |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|createdDateTime|DateTimeOffset|O tipo Timestamp representa a data e a hora de criação do local usando o formato ISO 8601 e está sempre em horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura.|
|displayName|Cadeia de caracteres|Nome acessível para humanos do local.|
|id|String|Identificador de um objeto namedLocation. Somente leitura.|
|modifiedDateTime|DateTimeOffset|O tipo Timestamp representa a última data e hora modificadas do local usando o formato ISO 8601 e está sempre em horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.namedLocation",
  "keyProperty": "id"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "id": "String (identifier)",
  "modifiedDateTime": "String (timestamp)"
}
```

## <a name="see-also"></a>Confira também

+ [O que é Acesso Condicional?](/azure/active-directory/conditional-access/overview)
+ [Usando a condição de local em uma política de Acesso Condicional](/azure/active-directory/conditional-access/location-condition)

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "namedLocation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

