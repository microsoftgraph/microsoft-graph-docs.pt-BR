---
title: tipo de recurso de scopedRoleMembership
description: Uma associação de função com escopo descreve a associação de um usuário de uma função de diretório, que ainda mais destinada para uma unidade administrativa (AU).  Isso oferece um mecanismo para permitir que um adminsistrator locatário toda empresa delegar privilégios administrativos para um usuário gerencie usuários e grupos em um subconjunto da organização (o subconjunto está sendo definido por um AU).
ms.openlocfilehash: bd635a5b1b06b98657ba24c397e2f67afb76fa8f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036460"
---
# <a name="scopedrolemembership-resource-type"></a>tipo de recurso de scopedRoleMembership

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Uma associação de função com escopo descreve a associação de um usuário de uma função de diretório, que ainda mais destinada para uma unidade administrativa (AU).  Isso oferece um mecanismo para permitir que um adminsistrator locatário toda empresa delegar privilégios administrativos para um usuário gerencie usuários e grupos em um subconjunto da organização (o subconjunto está sendo definido por um AU).

## <a name="methods"></a>Métodos
Consultas diretas para este recurso não são suportadas.  Por favor, consulte o tópico de [unidades administrativas](administrativeunit.md) para ver informações sobre como consultar as associações de função com escopo, bem como adicionando e removendo associações de função com escopo. 

## <a name="properties"></a>Propriedades
| Propriedade   | Tipo | Descrição |
|:---------------|:--------|:----------|
|administrativeUnitId|string|Identificador exclusivo para a unidade administrativa que a função directory destinada a|
|id|string| Identificador exclusivo para a associação da função com escopo. Somente leitura.|
|roleId|string| Identificador exclusivo para a função de diretório que o membro é no.|
|roleMemberInfo|[identity](identity.md)| Informações de identidade do membro de função. Representa o usuário que seja membro desta função com escopo.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scopedrolemembership"
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
<!-- {
  "type": "#page.annotation",
  "description": "scopedRoleMembership resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->