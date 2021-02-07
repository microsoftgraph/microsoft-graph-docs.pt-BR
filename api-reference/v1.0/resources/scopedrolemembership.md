---
title: Tipo de recurso scopedRoleMembership
description: Uma associação de função com escopo descreve a associação de um usuário a uma função de diretório, que tem como escopo uma Unidade Administrativa (AU).  Isso fornece um mecanismo para permitir que um administrador de empresa em todo o locatário delegar privilégios administrativos a um usuário para gerenciar usuários e grupos em um subconjunto da organização (o subconjunto sendo definido por uma AU).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: abhijeetsinha
ms.openlocfilehash: 8b7a2239d0ee44ab6caf0e98c7d818431764b1b1
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129902"
---
# <a name="scopedrolemembership-resource-type"></a>Tipo de recurso scopedRoleMembership

Namespace: microsoft.graph

Uma associação de função com escopo descreve a associação de um usuário a uma função de diretório, que tem como escopo uma Unidade Administrativa (AU).  Isso fornece um mecanismo para permitir que um administrador de empresa de todo o locatário delegar privilégios administrativos a um usuário para gerenciar usuários e grupos em um subconjunto da organização (o subconjunto definido por uma AU).

## <a name="methods"></a>Methods
Não há suporte para consultas diretas a esse recurso.  Consulte o tópico [de](administrativeunit.md) unidades administrativas para ver informações sobre como consultar associações de função com escopo, bem como adicionar e remover associações de função com escopo.

## <a name="properties"></a>Propriedades
| Propriedade   | Tipo | Descrição |
|:---------------|:--------|:----------|
|administrativeUnitId|string|Identificador exclusivo da unidade administrativa para a qual a função de diretório tem escopo|
|id|string| Identificador exclusivo da associação de função com escopo. Somente leitura.|
|roleId|string| Identificador exclusivo da função de diretório na qual o membro está.|
|roleMemberInfo|[identity](identity.md)| Informações de identidade do membro da função. Representa o usuário que é membro dessa função com escopo.|

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
