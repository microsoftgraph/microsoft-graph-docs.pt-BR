---
title: Tipo de recurso directoryObject
description: Representa um objeto do Active Directory do Azure. O tipo **directoryObject** é o tipo básico de muitos outros tipos de entidade de diretório.
localization_priority: Priority
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 83750686b4075f7577e88e1e6107dd2f2a5f4d2f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439902"
---
# <a name="directoryobject-resource-type"></a>Tipo de recurso directoryObject

Namespace: microsoft.graph

Representa um objeto do Active Directory do Azure. O tipo **directoryObject** é o tipo básico de muitos outros tipos de entidade de diretório.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Get directoryObject](../api/directoryobject-get.md) | [directoryObject](directoryobject.md) |Leia as propriedades de um objeto de diretório.|
|[Delete directoryObject](../api/directoryobject-delete.md) | Nenhum |Exclua um objeto de diretório. |
|[checkMemberGroups](../api/directoryobject-checkmembergroups.md)|Coleção de cadeias de caracteres|Verifique se há uma associação em uma lista de grupos. A verificação é transitiva.|
|[Obtenha as propriedades de extensão disponíveis](../api/directoryobject-getavailableextensionproperties.md)|Coleção [extensionProperty](../resources/extensionproperty.md)|Obtenha todas as listas ou uma lista filtrada das propriedades de extensão do diretório que foram registradas em um diretório.|
|[getMemberGroups](../api/directoryobject-getmembergroups.md)|Coleção de cadeias de caracteres|Retorne todos os grupos dos quais o objeto de usuário, grupo ou diretório é membro. A verificação é transitiva.|
|[getMemberObjects](../api/directoryobject-getmemberobjects.md)|Coleção de cadeias de caracteres| Retorne todos os grupos e funções de diretório dos quais o objeto de usuário, grupo ou diretório é membro. A verificação é transitiva. |
|[getByIds](../api/directoryobject-getbyids.md) | Coleção [directoryObject](directoryobject.md) | Obtenha um conjunto de objetos de diretório com base em um conjunto de ids fornecidas. |
|[validateProperties](../api/directoryobject-validateproperties.md)|Json| Valide se o nome de exibição ou apelido de email de um grupo da Microsoft 365 está em conformidade com as políticas de nomenclatura. |

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|id|Cadeia de caracteres|O identificador exclusivo para o objeto. Por exemplo, 12345678-9abc-def0-1234-56789abcde. O valor da propriedade **ID** é frequentemente, mas não exclusivamente, sob o formato de um GUID; O valor deve ser tratado como um identificador opaco e não confie no fato de ser um GUID. Chave. Não anulável. Somente leitura.|

## <a name="relationships"></a>Relações

Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.directoryObject",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "countable": false,
        "expandable": false,
        "filterable": false,
        "referenceable": false,
        "selectable": false
      }
    }
  ]
}-->

```json
{
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

