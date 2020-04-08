---
title: Tipo de recurso directoryObject
description: Representa um objeto do Active Directory do Azure. O tipo **directoryObject** é o tipo básico de muitos outros tipos de entidade de diretório.
localization_priority: Priority
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 43fd850274006d763535ad30b2de58f634375541
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181691"
---
# <a name="directoryobject-resource-type"></a>Tipo de recurso directoryObject

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um objeto do Active Directory do Azure. O tipo **directoryObject** é o tipo básico de muitos outros tipos de entidade de diretório.

Esse recurso permite:

- Usar a [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/directoryobject-delta.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Get directoryObject](../api/directoryobject-get.md) | [directoryObject](directoryobject.md) |Leia as propriedades de um objeto de diretório.|
|[Delete](../api/directoryobject-delete.md) | Nenhum |Exclua um objeto de diretório. |
|[checkMemberGroups](../api/directoryobject-checkmembergroups.md)|Coleção de cadeias de caracteres|Verifique se há uma associação em uma lista de grupos. A verificação é transitiva.|
|[getMemberGroups](../api/directoryobject-getmembergroups.md)|Coleção de cadeias de caracteres|Retorne todos os grupos dos quais o objeto de usuário, grupo ou diretório é membro. A verificação é transitiva.|
|[getMemberObjects](../api/directoryobject-getmemberobjects.md)|Coleção de cadeias de caracteres| Retorne todos os grupos e funções de diretório dos quais o objeto de usuário, grupo ou diretório é membro. A verificação é transitiva. |
|[getByIds](../api/directoryobject-getbyids.md) | Coleção [directoryObject](directoryobject.md) | Obtenha um conjunto de objetos de diretório com base em um conjunto de ids fornecidas. |
|[validateProperties](../api/directoryobject-validateproperties.md)|Json| Validar um nome de exibição ou um apelido de email do grupo do Office 365 em conformidade com as políticas de nomenclatura. |
|[delta](../api/directoryobject-delta.md)|Coleção [directoryObject](directoryobject.md)| Obtenha alterações incrementais para objetos de diretório. Oferece suporte à filtragem por tipo derivado. |

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|id|String|Um Guid que é o identificador exclusivo do objeto; por exemplo, 12345678-9abc-def0-1234-56789abcde12. Chave. Não anulável. Somente leitura.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryObject",
  "openType": true
}-->

```json
{
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
