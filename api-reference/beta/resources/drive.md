---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Unidade
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: e788765c3405a1455eda55f6fefdc21ade3da8fd
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573925"
---
# <a name="drive-resource-type"></a>tipo de recurso de unidade

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso drive é o objeto de nível superior que representa o OneDrive de um usuário ou uma biblioteca de documentos no SharePoint.

Os usuários do OneDrive sempre terão pelo menos uma unidade disponível, sua unidade padrão. Usuários sem uma licença do OneDrive talvez não tenham uma unidade padrão disponível.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON de um recurso Drive.

O recurso **drive** é derivado de [**baseItem**](baseitem.md) e herda propriedades desse recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "activities",
    "createdBy",
    "createdDateTime",
    "description",
    "lastModifiedBy",
    "lastModifiedDateTime",
    "name",
    "webUrl",
    "items",
    "root",
    "special",
    "system"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.drive"
}-->

```json
{
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "id": "string",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "string (timestamp)",
  "description": "string",
  "driveType": "personal | business | documentLibrary",
  "following": [ { "@odata.type": "microsoft.graph.driveItem" } ],
  "items": [ { "@odata.type": "microsoft.graph.driveItem" } ],
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "string (timestamp)",
  "name": "string",
  "owner": { "@odata.type": "microsoft.graph.identitySet" },
  "quota": { "@odata.type": "microsoft.graph.quota" },
  "root": { "@odata.type": "microsoft.graph.driveItem" },
  "special": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "system": { "@odata.type": "microsoft.graph.systemFacet" },
  "webUrl": "url"
}
```

## <a name="properties"></a>Propriedades

| Propriedade             | Tipo                          | Descrição                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| createdBy            | [identitySet][]               | Identidade do usuário, dispositivo ou aplicativo que criou o item. Somente leitura.                                                                                                                                                  |
| createdDateTime      | dateTimeOffset                | Data e hora de criação do item. Somente leitura.                                                                                                                                                                                       |
| description          | String                        | Fornecer uma descrição visível para os usuários da unidade. Leitura e gravação.
| driveType            | String                        | Descreve o tipo de unidade representado por esse recurso. As unidades pessoais do OneDrive retornarão `personal`. O OneDrive for Business retornará `business`. As bibliotecas de documentos do SharePoint retornarão `documentLibrary`. Somente leitura. |
| id                   | String                        | O identificador exclusivo da unidade. Somente leitura.                                                                                                                                                                                   |
| lastModifiedBy       | [identitySet][]               | Identidade do usuário, dispositivo e aplicativo que modificou o item pela última vez. Somente leitura.                                                                                                                                           |
| lastModifiedDateTime | dateTimeOffset                | Data e hora em que o item foi modificado pela última vez. Somente leitura.                                                                                                                                                                             |
| nome                 | string                        | O nome do item. Leitura e gravação.                                                                                                                                                                                                |
| owner                | [identitySet](identityset.md) | Opcional. A conta do usuário que é proprietário da unidade. Somente leitura.                                                                                                                                                                       |
| quota                | [quota](quota.md)             | Opcional. Informações sobre a cota de espaço de armazenamento da unidade. Somente leitura.                                                                                                                                                          |
| sharepointIds        | [sharepointIds][]             | Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.                                                                                                                                                         |
| sistema               | [systemFacet][]               | Se estiver presente, indica que se trata de uma unidade gerenciada pelo sistema. Somente leitura.
| webUrl               | string (url)                  | URL que exibe o recurso no navegador. Somente leitura.                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md
[systemFacet]: systemfacet.md

## <a name="relationships"></a>Relações

| Relação | Tipo                                 | Descrição
|:-------------|:-------------------------------------|:-----------------------
| activities   | Conjunto [itemActivity][]          | A lista de atividades recentes que ocorreram nesta unidade.
| items        | Coleção [driveItem](driveitem.md) | Todos os itens contidos na unidade. Somente leitura. Anulável.
| root         | [driveItem](driveitem.md)            | A pasta raiz da unidade. Somente leitura.
| special      | Coleção [driveItem](driveitem.md) | Coleção de pastas comuns disponíveis no OneDrive. Somente leitura. Anulável.
| following    | Coleção [driveItem](driveitem.md) | A lista de itens que o usuário está seguindo. Somente no OneDrive for Business.

## <a name="methods"></a>Métodos

|                        Tarefa comum                         |         Método HTTP         |
| :--------------------------------------------------------- | :-------------------------- |
| [Recuperar metadados de outra Unidade][drive-get]           | `GET /drives/{drive-id}`    |
| [Recuperar a pasta raiz da Unidade padrão do usuário][item-get]       | `GET /drive/root`           |
| [Listar atividades sob a Unidade][drive-activities]        | `GET /drive/activities`     |
| [Listar itens seguidos][drive-following]                     | `GET /drive/following`      |
| [Listar filhos na Unidade][item-children]             | `GET /drive/root/children`  |
| [Listar alterações de todos os Itens na Unidade][item-changes]    | `GET /drive/root/delta`     |
| [Pesquisar Itens na Unidade][item-search]               | `GET /drive/root/search`    |
| [Acessar pasta especial](../api/drive-get-specialfolder.md) | `GET /drive/special/{name}` |

Na tabela anterior, os exemplos usam `/drive`, mas outros caminhos também são válidos.

[itemActivity]: itemactivity.md
[item-resource]: driveitem.md
[identity-set]: identityset.md
[quota-facet]: quota.md
[drive-resource]: drive.md
[drive-activities]: ../api/activities-list.md
[drive-following]: ../api/drive-list-following.md
[drive-get]: ../api/drive-get.md
[item-get]: ../api/driveitem-get.md
[item-changes]: ../api/driveitem-delta.md
[item-search]: ../api/driveitem-search.md
[item-children]: ../api/driveitem-list-children.md


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Drive is a top level object for OneDrive API that provides access to the contents of a drive. ",
  "keywords": "drive,objects,resources",
  "section": "documentation",
  "tocPath": "Drives",
  "tocBookmarks": {
    "Resources/Drive": "#"
  },
  "suppressions": [
    "Error: /api-reference/beta/resources/drive.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
