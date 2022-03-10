---
title: Tipo de recurso directoryObject
description: Representa um objeto do Azure Active Directory. O tipo directoryObject é o tipo base para muitos outros tipos de entidade de diretório.
ms.localizationpriority: high
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 4db8a25eac6d627b82d38e6d060d3098fc25baa6
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335434"
---
# <a name="directoryobject-resource-type"></a>Tipo de recurso directoryObject

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um objeto do Active Directory do Azure. O tipo **directoryObject** é o tipo básico de muitos outros tipos de entidade de diretório.

Esse recurso permite:

- Usar a [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função **delta**.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Get directoryObject](../api/directoryobject-get.md) | [directoryObject](directoryobject.md) |Leia as propriedades de um objeto de diretório.|
|[Delete](../api/directoryobject-delete.md) | Nenhum |Exclua um objeto de diretório. |
|[checkMemberGroups](../api/directoryobject-checkmembergroups.md)|Coleção de cadeias de caracteres|Verifique se há associação em uma lista especificada de grupos e retorne dessa lista os grupos dos quais o usuário, grupo, entidade de serviço especificado, contato organizacional, dispositivo ou objeto de diretório é membro. A verificação é transitória.|
|[getMemberGroups](../api/directoryobject-getmembergroups.md)|Coleção de cadeias de caracteres|Retorna todos os grupos dos qual o usuário, grupo, entidade de serviço, contato organizacional, dispositivo ou objeto de diretório é membro. A verificação é transitória.|
|[checkMemberObjects](../api/directoryobject-checkmemberobjects.md)|Coleção de cadeias de caracteres|Verifica se há associação em uma lista de funções de grupo, unidades administrativas ou diretórios para o usuário, grupo, dispositivo, contato organizacional ou objeto de diretório especificado. Esse método é transitório.|
|[getMemberObjects](../api/directoryobject-getmemberobjects.md)|Coleção String| Retorna todos os grupos, unidades administrativas e funções de diretório das quais o usuário, grupo, dispositivo, contato organizacional ou objeto de diretório é membro. A verificação é transitória. |
|[getByIds](../api/directoryobject-getbyids.md) | Coleção [directoryObject](directoryobject.md) | Obtenha um conjunto de objetos de diretório com base em um conjunto de ids fornecidas. |
|[validateProperties](../api/directoryobject-validateproperties.md)|JSON| Validar se o nome de exibição de um grupo do Microsoft 365 ou apelido de email está em conformidade com as políticas de nomenclatura. |
|delta|Coleção [directoryObject](directoryObject.md)| Obtenha alterações incrementais para objetos de diretório, por exemplo, [usuários](../api/user-delta.md), [grupos](../api/group-delta.md), [aplicativos](../api/application-delta.md) e [entidades de serviço](../api/serviceprincipal-delta.md). Cada tipo derivado oferece suporte à filtragem pelo **id**. Para obter mais informações sobre consultas delta, consulte [Usar consulta delta para rastrear alterações nos dados do Microsoft Graph](/graph/delta-query-overview).|

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|deletedDateTime|DateTimeOffset|Data e hora em que este objeto foi excluído. Sempre `null` quando o objeto não tiver sido excluído. |
|id|Cadeia de caracteres|O identificador exclusivo do objeto. Por exemplo, 12345678-9abc-def0-1234-56789abcde. O valor da propriedade da **ID** é geralmente, mas não exclusivamente na forma de um GUID; trate-o como um identificador opaco e não confie que ele seja um GUID. Chave. Não pode ser anulado. Somente leitura.|

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


