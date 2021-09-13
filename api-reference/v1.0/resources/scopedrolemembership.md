---
title: Tipo de recurso scopedRoleMembership
description: Uma associação de função com escopo descreve a associação de um usuário a uma função de diretório, que é ainda mais escopo para uma Unidade Administrativa (AU).  Isso fornece um mecanismo para permitir que um administrador de uma empresa de todo o locatário delegar privilégios administrativos a um usuário gerencie usuários e grupos em um subconjunto da organização (o subconjunto que está sendo definido por uma AU).
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: directory-management
author: abhijeetsinha
ms.openlocfilehash: 7da1297b03b875a423fb135a2e8c1bab611041a5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59035938"
---
# <a name="scopedrolemembership-resource-type"></a>Tipo de recurso scopedRoleMembership

Namespace: microsoft.graph

Uma associação de função com escopo descreve a associação de um usuário a uma função de diretório, que é ainda mais escopo para uma Unidade Administrativa (AU).  Isso fornece um mecanismo para permitir que um administrador de uma empresa de todo o locatário delegar privilégios administrativos a um usuário gerencie usuários e grupos em um subconjunto da organização (o subconjunto que está sendo definido por uma AU).

## <a name="methods"></a>Métodos
Não há suporte para consultas diretas a esse recurso.  Consulte o tópico [unidades administrativas](administrativeunit.md) para ver informações sobre como consultar associações de função com escopo, bem como adicionar e remover associações de funções com escopo.

## <a name="properties"></a>Propriedades
| Propriedade   | Tipo | Descrição |
|:---------------|:--------|:----------|
|administrativeUnitId|cadeia de caracteres|Identificador exclusivo da unidade administrativa à qual a função de diretório é escopo|
|id|cadeia de caracteres| Identificador exclusivo para a associação de função com escopo. Somente leitura.|
|roleId|cadeia de caracteres| Identificador exclusivo da função de diretório na qual o membro está.|
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
