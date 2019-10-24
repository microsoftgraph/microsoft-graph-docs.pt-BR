---
title: tipo de recurso ipNamedLocation
description: Representa um local nomeado do Azure Active Directory definido por intervalos de IP. Locais nomeados são regras personalizadas que definem locais de rede que podem ser usados em uma política de acesso condicional.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 10bdafb9894d822f345bb6fb23174fa7f7deee4c
ms.sourcegitcommit: d189830649794365464e37539e02239f883011da
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/24/2019
ms.locfileid: "37653815"
---
# <a name="ipnamedlocation-resource-type"></a>tipo de recurso ipNamedLocation

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um local nomeado do Azure Active Directory definido por intervalos de IP. Locais nomeados são regras personalizadas que definem locais de rede que podem ser usados em uma política de acesso condicional.

Herda de [namedLocation](../resources/namedLocation.md)

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar ipNamedLocations](../api/conditionalaccessroot-list-namedlocations.md) | coleção [ipNamedLocation](ipNamedLocation.md) | Obtenha todos os objetos **ipNamedLocation** na organização. |
| [Criar ipNamedLocation](../api/conditionalaccessroot-post-namedlocations.md) | [ipNamedLocation](ipNamedLocation.md) | Criar um novo objeto **ipNamedLocation** . |
| [Obter ipNamedLocation](../api/ipnamedlocation-get.md) | [ipNamedLocation](ipnamedlocation.md) | Leia as propriedades e os relacionamentos de um objeto **ipNamedLocation** . |
| [Atualizar ipNamedLocation](../api/ipnamedlocation-update.md) | [ipNamedLocation](ipnamedlocation.md) | Atualize um objeto **ipNamedLocation** . |
| [Excluir ipNamedLocation](../api/ipnamedlocation-delete.md) | Nenhum | Excluir um objeto **ipNamedLocation** . |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|createdDateTime|DateTimeOffset|O tipo TIMESTAMP representa data e hora de criação do local usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura. Herdado de [namedLocation](../resources/namedLocation.md).|
|displayName|Cadeia de caracteres|Nome legível do local.|
|id|String|Identificador de um objeto namedLocation. Somente leitura. Herdado de [namedLocation](../resources/namedLocation.md).|
|Intervalos|Coleção [ipRange](iprange.md)|Lista de intervalos de endereços IP no formato CIDR do IPv4 (por exemplo, 1.2.3.4/32) ou qualquer formato IPv6 permitido da IETF RFC596.|
|isTrusted|Booliano|True se esse local é explicitamente confiável.|
|modifiedDateTime|DateTimeOffset|O tipo TIMESTAMP representa data e hora da última modificação do local usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura. Herdado de [namedLocation](../resources/namedLocation.md).|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.ipNamedLocation",
  "baseType": ""
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
