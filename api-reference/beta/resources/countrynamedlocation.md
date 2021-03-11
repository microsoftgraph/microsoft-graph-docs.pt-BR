---
title: Tipo de recurso countryNamedLocation
description: Representa um Azure Active Directory nomeado local definido por países e regiões. Locais nomeados são regras personalizadas que definem locais de rede que podem ser usados em uma política de Acesso Condicional.
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f6a986907ee82ea3f40c7b294cf21bf4dcc191a4
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721653"
---
# <a name="countrynamedlocation-resource-type"></a>Tipo de recurso countryNamedLocation

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um Azure Active Directory nomeado local definido por países e regiões. Locais nomeados são regras personalizadas que definem locais de rede que podem ser usados em uma política de Acesso Condicional.

Herda de [namedLocation](../resources/namedLocation.md)

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar countryNamedLocations](../api/conditionalaccessroot-list-namedlocations.md) | [coleção countryNamedLocation](countryNamedLocation.md) | Obter todos os **objetos countryNamedLocation** na organização. |
| [Criar countryNamedLocation](../api/conditionalaccessroot-post-namedlocations.md) | [countryNamedLocation](countryNamedLocation.md) | Crie um novo **objeto countryNamedLocation.** |
| [Obter countryNamedLocation](../api/countrynamedlocation-get.md) | [countryNamedLocation](countrynamedlocation.md) | Leia as propriedades e as relações de um **objeto countryNamedLocation.** |
| [Atualizar countryNamedLocation](../api/countrynamedlocation-update.md) | [countryNamedLocation](countrynamedlocation.md) | Atualize um **objeto countryNamedLocation.** |
| [Excluir countryNamedLocation](../api/countrynamedlocation-delete.md) | Nenhum(a) | Exclua **um objeto countryNamedLocation.** |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|countriesAndRegions|Coleção de cadeias de caracteres|Lista de países e/ou regiões no formato de duas letras especificado pela ISO 3166-2.|
|createdDateTime|DateTimeOffset|O tipo Timestamp representa a data e a hora de criação do local usando o formato ISO 8601 e está sempre em horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura. Herdado [de namedLocation](../resources/namedLocation.md).|
|displayName|Cadeia de caracteres|Nome acessível para humanos do local. Herdado [de namedLocation](../resources/namedLocation.md).|
|id|Cadeia de caracteres|Identificador de um objeto namedLocation. Somente leitura. Herdado [de namedLocation](../resources/namedLocation.md).|
|includeUnknownCountriesAndRegions|Booliano|True se os endereços IP que não mapeiam para um país ou região devem ser incluídos no local nomeado.|
|modifiedDateTime|DateTimeOffset|O tipo Timestamp representa a última data e hora modificadas do local usando o formato ISO 8601 e está sempre em horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura. Herdado [de namedLocation](../resources/namedLocation.md).|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.countryNamedLocation"
}-->

```json
{
  "countriesAndRegions": ["String"],
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "id": "String (identifier)",
  "includeUnknownCountriesAndRegions": true,
  "modifiedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "countryNamedLocation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


