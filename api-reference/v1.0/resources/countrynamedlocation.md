---
title: tipo de recurso countryNamedLocation
description: Representa um local nomeado do Azure Active Directory definido por países e regiões. Locais nomeados são regras personalizadas que definem locais de rede que podem ser usados em uma política de acesso condicional.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d458a61e0877e7eb367edb65afe4bf7daca422f4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018799"
---
# <a name="countrynamedlocation-resource-type"></a>tipo de recurso countryNamedLocation

Namespace: microsoft.graph

Representa um local nomeado do Azure Active Directory definido por países e regiões. Locais nomeados são regras personalizadas que definem locais de rede que podem ser usados em uma política de acesso condicional.

Herda de [namedLocation](../resources/namedLocation.md)

## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar countryNamedLocations](../api/conditionalaccessroot-list-namedlocations.md) | coleção [countryNamedLocation](countryNamedLocation.md) | Obtenha todos os objetos **countryNamedLocation** na organização. |
| [Criar countryNamedLocation](../api/conditionalaccessroot-post-namedlocations.md) | [countryNamedLocation](countryNamedLocation.md) | Criar um novo objeto **countryNamedLocation** . |
| [Obter countryNamedLocation](../api/countrynamedlocation-get.md) | [countryNamedLocation](countrynamedlocation.md) | Leia as propriedades e os relacionamentos de um objeto **countryNamedLocation** . |
| [Atualizar countryNamedLocation](../api/countrynamedlocation-update.md) | [countryNamedLocation](countrynamedlocation.md) | Atualizar um objeto **countryNamedLocation** . |
| [Excluir countryNamedLocation](../api/countrynamedlocation-delete.md) | Nenhum | Excluir um objeto **countryNamedLocation** . |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|countriesAndRegions|Coleção de cadeias de caracteres|Lista de países e/ou regiões no formato de duas letras especificado pela ISO 3166-2.|
|createdDateTime|DateTimeOffset|O tipo TIMESTAMP representa data e hora de criação do local usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura. Herdado de [namedLocation](../resources/namedLocation.md).|
|displayName|String|Nome legível do local. Herdado de [namedLocation](../resources/namedLocation.md).|
|id|String|Identificador de um objeto namedLocation. Somente leitura. Herdado de [namedLocation](../resources/namedLocation.md).|
|includeUnknownCountriesAndRegions|Boolean|True se endereços IP que não mapeiam para um país ou região devem ser incluídos no local nomeado.|
|modifiedDateTime|DateTimeOffset|O tipo TIMESTAMP representa data e hora da última modificação do local usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura. Herdado de [namedLocation](../resources/namedLocation.md).|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.countryNamedLocation",
  "baseType": ""
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

