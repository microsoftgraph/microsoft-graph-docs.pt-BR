---
title: Tipo de recurso countryNamedLocation
description: Representa uma Azure Active Directory nome definida por países e regiões. Locais nomeados são regras personalizadas que definem locais de rede que podem ser usados em uma política de Acesso Condicional.
ms.localizationpriority: medium
author: davidspooner
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f80a31798e30ae91c0179c420323e71ff31afebf
ms.sourcegitcommit: 3f3975916b5c531ee63d92340ccd6e73e879e8d7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/21/2022
ms.locfileid: "62162087"
---
# <a name="countrynamedlocation-resource-type"></a>Tipo de recurso countryNamedLocation

Namespace: microsoft.graph

Representa uma Azure Active Directory nome definida por países e regiões. Locais nomeados são regras personalizadas que definem locais de rede que podem ser usados em uma política de Acesso Condicional.

Herda de [namedLocation](../resources/namedLocation.md)

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar countryNamedLocations](../api/conditionalaccessroot-list-namedlocations.md) | [coleção countryNamedLocation](countryNamedLocation.md) | Obter todos os **objetos countryNamedLocation** na organização. |
| [Criar countryNamedLocation](../api/conditionalaccessroot-post-namedlocations.md) | [countryNamedLocation](countryNamedLocation.md) | Crie um novo **objeto countryNamedLocation.** |
| [Obter countryNamedLocation](../api/countrynamedlocation-get.md) | [countryNamedLocation](countrynamedlocation.md) | Leia as propriedades e as relações de um **objeto countryNamedLocation.** |
| [Atualizar countryNamedLocation](../api/countrynamedlocation-update.md) | [countryNamedLocation](countrynamedlocation.md) | Atualize um **objeto countryNamedLocation.** |
| [Excluir countryNamedLocation](../api/countrynamedlocation-delete.md) | Nenhum | Exclua **um objeto countryNamedLocation.** |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|countriesAndRegions|Coleção String|Lista de países e/ou regiões no formato de duas letras especificado pela ISO 3166-2. Obrigatório.|
|countryLookupMethod|countryLookupMethodType|Determina em qual método é usado para decidir em qual país o usuário está localizado. Os valores possíveis `clientIpAddress` são (padrão) e `authenticatorAppGps` . Observação: `authenticatorAppGps` ainda não há suporte no Microsoft Cloud for US Government.|
|createdDateTime|DateTimeOffset|O tipo Timestamp representa a data e a hora de criação do local usando o formato ISO 8601 e está sempre em horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura. Herdado [de namedLocation](../resources/namedLocation.md).|
|displayName|Cadeia de caracteres|Nome acessível para humanos do local. Obrigatório. Herdado [de namedLocation](../resources/namedLocation.md).|
|id|Cadeia de caracteres|Identificador de um objeto namedLocation. Somente leitura. Herdado [de namedLocation](../resources/namedLocation.md).|
|includeUnknownCountriesAndRegions|Booliano|`true` se os endereços IP que não mapeiam para um país ou região devem ser incluídos no local nomeado. Opcional. O valor padrão é `false`.|
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
  "countryLookupMethod": "String",
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "id": "String (identifier)",
  "includeUnknownCountriesAndRegions": true,
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
  "description": "countryNamedLocation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
