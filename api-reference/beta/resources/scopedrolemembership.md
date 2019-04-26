---
title: tipo de recurso scopedRoleMembership
description: Uma associação de função com escopo descreve a associação de um usuário de uma função de diretório, que tem mais escopo para uma unidade administrativa (AU).  Isso fornece um mecanismo para permitir que uma empresa de todo o locatário adminsistrator delegar privilégios administrativos a um usuário para gerenciar usuários e grupos em um subconjunto da organização (o subconjunto que está definido por uma AU).
localization_priority: Normal
ms.openlocfilehash: 56a2514fa65033154b6ab69c497c90fde201c28e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343450"
---
# <a name="scopedrolemembership-resource-type"></a>tipo de recurso scopedRoleMembership

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma associação de função com escopo descreve a associação de um usuário de uma função de diretório, que tem mais escopo para uma unidade administrativa (AU).  Isso fornece um mecanismo para permitir que uma empresa de todo o locatário adminsistrator delegar privilégios administrativos a um usuário para gerenciar usuários e grupos em um subconjunto da organização (o subconjunto que está definido por uma AU).

## <a name="methods"></a>Métodos
Não há suporte para consultas diretas a esse recurso.  Confira o tópico [unidades administrativas](administrativeunit.md) para ver informações sobre como consultar as associações com escopo de função, bem como adicionar e remover associações com escopo de função. 

## <a name="properties"></a>Propriedades
| Propriedade   | Tipo | Descrição |
|:---------------|:--------|:----------|
|administrativeUnitId|string|Identificador exclusivo da unidade administrativa à qual a função de diretório tem escopo|
|id|string| Identificador exclusivo da associação com escopo de função. Somente leitura.|
|roleId|string| Identificador exclusivo da função de diretório em que o membro está.|
|roleMemberInfo|[identity](identity.md)| Informações de identidade de membro da função. Representa o usuário que é um membro desse escopo-Role.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scopedRoleMembership"
}-->

```json
{
  "administrativeUnitId": "string",
  "id": "string (identifier)",
  "roleId": "string",
  "roleMemberInfo": {"@odata.type": "microsoft.graph.identity"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "scopedRoleMembership resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
