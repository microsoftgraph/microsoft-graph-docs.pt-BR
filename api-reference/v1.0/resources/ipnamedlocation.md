---
title: Tipo de recurso ipNamedLocation
description: Representa um local nomeado pelo Azure Active Directory definido por intervalos IP. Locais nomeados são regras personalizadas que definem locais de rede que podem ser usados em uma política de Acesso Condicional.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 1781c10e28e2d3efc28154cd15a8c36c9b43ac21
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50719336"
---
# <a name="ipnamedlocation-resource-type"></a>Tipo de recurso ipNamedLocation

Namespace: microsoft.graph

Representa um local nomeado pelo Azure Active Directory definido por intervalos IP. Locais nomeados são regras personalizadas que definem locais de rede que podem ser usados em uma política de Acesso Condicional.

Herda de [namedLocation](../resources/namedLocation.md)

## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar ipNamedLocations](../api/conditionalaccessroot-list-namedlocations.md) | [Coleção ipNamedLocation](ipNamedLocation.md) | Obter todos os **objetos ipNamedLocation** na organização. |
| [Criar ipNamedLocation](../api/conditionalaccessroot-post-namedlocations.md) | [ipNamedLocation](ipNamedLocation.md) | Crie um novo **objeto ipNamedLocation.** |
| [Obter ipNamedLocation](../api/ipnamedlocation-get.md) | [ipNamedLocation](ipnamedlocation.md) | Leia as propriedades e as relações de um **objeto ipNamedLocation.** |
| [Atualizar ipNamedLocation](../api/ipnamedlocation-update.md) | [ipNamedLocation](ipnamedlocation.md) | Atualize um **objeto ipNamedLocation.** |
| [Excluir ipNamedLocation](../api/ipnamedlocation-delete.md) | Nenhum | **Exclua um objeto ipNamedLocation.** |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|createdDateTime|DateTimeOffset|O tipo Timestamp representa a data e a hora de criação do local usando o formato ISO 8601 e está sempre em horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura. Herdado [de namedLocation](../resources/namedLocation.md).|
|displayName|Cadeia de caracteres|Nome acessível para humanos do local.|
|id|Cadeia de caracteres|Identificador de um objeto namedLocation. Somente leitura. Herdado [de namedLocation](../resources/namedLocation.md).|
|ipRanges|Coleção [ipRange](iprange.md)|Lista de intervalos de endereços IP no formato CIDR IPv4 (por exemplo, 1.2.3.4/32) ou qualquer formato IPv6 acessível do IETF RFC596.|
|isTrusted|Booliano|True se esse local for explicitamente confiável.|
|modifiedDateTime|DateTimeOffset|O tipo Timestamp representa a última data e hora modificadas do local usando o formato ISO 8601 e está sempre em horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura. Herdado [de namedLocation](../resources/namedLocation.md).|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.ipNamedLocation"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "id": "String (identifier)",
  "ipRanges": [{"@odata.type": "microsoft.graph.ipRange"}],
  "isTrusted": true,
  "modifiedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ipNamedLocation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

