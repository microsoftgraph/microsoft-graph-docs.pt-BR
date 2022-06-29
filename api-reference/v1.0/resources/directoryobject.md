---
title: Tipo de recurso directoryObject
description: Representa um objeto do Azure Active Directory. O tipo directoryObject é o tipo base para muitos outros tipos de entidade de diretório geralmente chamados de objetos de diretório.
ms.localizationpriority: high
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: a9a17eae32984aeb42df8c395eaecdab8420c6a3
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437104"
---
# <a name="directoryobject-resource-type"></a>Tipo de recurso directoryObject

Namespace: microsoft.graph

Representa um objeto do Active Directory do Azure. O tipo **directoryObject** é o tipo base para os seguintes tipos de entidade de diretório geralmente chamados de objetos de diretório:

+ [application](application.md)
+ [administrativeUnit](administrativeunit.md)
+ [appRoleAssignment](approleassignment.md)
+ [directoryObject](directoryobject.md)
+ [directoryRole](directoryrole.md)
+ [device](device.md)
+ [group](group.md)
+ [orgContact](orgcontact.md)
+ [oauth2PermissionGrant](oauth2permissiongrant.md)
+ [servicePrincipal](serviceprincipal.md)
+ [user](user.md)

Herda de [entidade](entity.md).

## <a name="methods"></a>Methods

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Get directoryObject](../api/directoryobject-get.md) | [directoryObject](directoryobject.md) |Leia as propriedades de um objeto de diretório.|
|[Delete directoryObject](../api/directoryobject-delete.md) | Nenhum |Exclua um objeto de diretório. |
|[Obtenha as propriedades de extensão disponíveis](../api/directoryobject-getavailableextensionproperties.md)|Coleção [extensionProperty](../resources/extensionproperty.md)|Obtenha todas as listas ou uma lista filtrada das propriedades de extensão do diretório que foram registradas em um diretório.|
|[checkMemberGroups](../api/directoryobject-checkmembergroups.md)|Coleção de cadeias de caracteres|Verifique se há associação em uma lista especificada de grupos e retorne dessa lista os grupos dos quais o usuário, grupo, entidade de serviço especificado, contato organizacional, dispositivo ou objeto de diretório é um membro. A verificação é transitória.|
|[getMemberGroups](../api/directoryobject-getmembergroups.md)|Coleção de cadeias de caracteres|Retorna todos os grupos dos qual o usuário, grupo, entidade de serviço, contato organizacional, dispositivo ou objeto de diretório é membro. A verificação é transitória.|
|[checkMemberObjects](../api/directoryobject-checkmemberobjects.md)|Coleção de cadeias de caracteres|Verifica se há associação em uma lista de funções de grupo, unidades administrativas ou diretórios para o usuário, grupo, dispositivo, contato organizacional ou objeto de diretório especificado. Esse método é transitório.|
|[getMemberObjects](../api/directoryobject-getmemberobjects.md)|Coleção String| Retorna todos os grupos, unidades administrativas e funções de diretório das quais o usuário, grupo, dispositivo, contato organizacional ou objeto de diretório é membro. A verificação é transitória. |
|[getByIds](../api/directoryobject-getbyids.md) | Coleção [directoryObject](directoryobject.md) | Obtenha um conjunto de objetos de diretório com base em um conjunto de ids fornecidas. |
|[validateProperties](../api/directoryobject-validateproperties.md)|JSON| Valide se o nome de exibição ou apelido de email de um grupo da Microsoft 365 está em conformidade com as políticas de nomenclatura. |
|delta|Coleção [directoryObject](directoryObject.md)| Obtenha alterações incrementais para objetos de diretório, por exemplo, [usuários](../api/user-delta.md), [grupos](../api/group-delta.md), [aplicativos](../api/application-delta.md) e [entidades de serviço](../api/serviceprincipal-delta.md). Cada tipo derivado oferece suporte à filtragem pelo **id**. Para obter mais informações sobre consultas delta, consulte [Usar consulta delta para rastrear alterações nos dados do Microsoft Graph](/graph/delta-query-overview).|

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|deletedDateTime|DateTimeOffset|Data e hora em que este objeto foi excluído. Sempre `null` quando o objeto não tiver sido excluído. |
|id|Cadeia de caracteres|O identificador exclusivo para o objeto. Por exemplo, `12345678-9abc-def0-1234-56789abcde`. O valor da propriedade **ID** é frequentemente, mas não exclusivamente, sob o formato de um GUID; O valor deve ser tratado como um identificador opaco e não confie no fato de ser um GUID. Chave. Não anulável. Somente leitura. Herdado da [entidade](entity.md).|


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

