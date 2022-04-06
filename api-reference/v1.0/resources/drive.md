---
author: JeremyKelley
title: tipo de recurso de unidade
description: O recurso drive é o objeto de nível superior que representa o OneDrive de um usuário ou uma biblioteca de documentos no SharePoint.
ms.localizationpriority: high
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: eb7070e357681311cfe0d881940c3047dbac5505
ms.sourcegitcommit: f5382652b6880fab42040df40a08de7cb2d74d35
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/17/2022
ms.locfileid: "63560233"
---
# <a name="drive-resource-type"></a>tipo de recurso de unidade

Namespace: microsoft.graph

O objeto de nível superior que representa a OneDrive de um usuário ou uma biblioteca de documentos em SharePoint.

Os usuários do OneDrive sempre terão pelo menos uma unidade disponível, sua unidade padrão. Usuários sem uma licença do OneDrive talvez não tenham uma unidade padrão disponível.

## <a name="methods"></a>Métodos

|                        Método                              |         Tipo de retorno         | Descrição |
| :--------------------------------------------------------- | :-------------------------- |-------------|
| [Obter unidade][drive-get]                                     | unidade                       | Obter metadados sobre uma unidade |
| [Obter raiz da unidade][item-get]                                 | [driveItem][]               | Obter pasta raiz de uma unidade |
| [Listar itens seguidos][drive-following]                     | Coleção de [driveItem][]    | Listar os driveItems seguidos do usuário |
| [Listar secundários][item-children]                             | Coleção de [driveItem][]    | Listar secundários da pasta raiz de uma unidade |
| [Listar alterações][item-changes]                               | Coleção de [driveItem][]    | Listar alterações de todos os driveItems na Unidade |
| [Pesquisa][item-search]                                      | Coleção de [driveItem][]    | Pesquisar driveItems em uma unidade |
| [Obter pasta especial](../api/drive-get-specialfolder.md)    | [driveItem][]               | Acessar uma pasta especial por nome canônico |


## <a name="properties"></a>Propriedades

| Propriedade             | Tipo                          | Descrição                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| createdBy            | [identitySet][]               | Identidade do usuário, dispositivo ou aplicativo que criou o item. Somente leitura.                                                                                                                                                  |
| createdDateTime      | dateTimeOffset                | Data e hora de criação do item. Somente leitura.                                                                                                                                                                                       |
| description          | Cadeia de caracteres                        | Fornecer uma descrição visível aos usuários da unidade. Leitura e gravação.
| driveType            | String                        | Descreve o tipo de unidade representado por esse recurso. As unidades pessoais do OneDrive retornarão `personal`. O OneDrive for Business retornará `business`. As bibliotecas de documentos do SharePoint retornarão `documentLibrary`. Somente leitura. |
| id                   | String                        | O identificador exclusivo da unidade. Somente leitura.                                                                                                                                                                                   |
| lastModifiedBy       | [identitySet][]               | Identidade do usuário, dispositivo e aplicativo que modificou o item pela última vez. Somente leitura.                                                                                                                                           |
| lastModifiedDateTime | dateTimeOffset                | Data e hora em que o item foi modificado pela última vez. Somente leitura.                                                                                                                                                                             |
| nome                 | string                        | O nome do item. Leitura e gravação.                                                                                                                                                                                                |
| owner                | [identitySet](identityset.md) | Opcional. A conta do usuário que é proprietário da unidade. Somente leitura.                                                                                                                                                                       |
| quota                | [quota](quota.md)             | Opcional. Informações sobre a cota de espaço de armazenamento da unidade. Somente leitura.                                                                                                                                                          |
| sharepointIds        | [sharepointIds][]             | Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura. A propriedade não é retornada por padrão e deve ser selecionada usando o parâmetro de consulta `$select`.  |
| sistema               | [systemFacet][]               | Se estiver presente, indica que se trata de uma unidade gerenciada pelo sistema. Somente leitura.
| webUrl               | string (url)                  | URL que exibe o recurso no navegador. Somente leitura.                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md
[systemFacet]: systemfacet.md

## <a name="relationships"></a>Relações

| Relação | Tipo                                 | Descrição
|:-------------|:-------------------------------------|:-----------------------
| pacotes      | Coleção de [driveItem][]             | Coleção de [pacotes][bundle] (álbuns e conjuntos de itens compartilhados com várias seleções). Apenas no OneDrive pessoal.
| following    | Coleção [driveItem][]             | A lista de itens que o usuário está seguindo. Somente no OneDrive for Business.
| items        | Coleção [driveItem][]             | Todos os itens contidos na unidade. Somente leitura. Anulável.
| root         | [driveItem][]                        | A pasta raiz da unidade. Somente leitura.
| special      | Coleção [driveItem][]             | Coleção de pastas comuns disponíveis no OneDrive. Somente leitura. Anulável.
| list         | [list][]                             | Para unidades no SharePoint, a lista de biblioteca de documentos subjacentes. Somente leitura. Anulável.

## <a name="json-representation"></a>Representação JSON

A seguir está uma representação JSON desse recurso.

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
    "sharepointIds",
    "special",
    "system"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.drive"
}-->

```json
{
  "id": "string",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "string (timestamp)",
  "description": "string",
  "driveType": "personal | business | documentLibrary",
  "following": [{"@odata.type": "microsoft.graph.driveItem"}],
  "items": [{"@odata.type": "microsoft.graph.driveItem"}],
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "string (timestamp)",
  "name": "string",
  "owner": {"@odata.type": "microsoft.graph.identitySet"},
  "quota": {"@odata.type": "microsoft.graph.quota"},
  "root": {"@odata.type": "microsoft.graph.driveItem"},
  "sharepointIds": {"@odata.type": "microsoft.graph.sharepointIds"},
  "special": [{"@odata.type": "microsoft.graph.driveItem"}],
  "system": {"@odata.type": "microsoft.graph.systemFacet"},
  "webUrl": "string",

}
```

[bundle]: bundle.md
[driveItem]: driveItem.md
[item-resource]: driveitem.md
[identity-set]: identityset.md
[list]: list.md
[quota-facet]: quota.md
[drive-resource]: drive.md
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
    "Resources/Drive&quot;: &quot;#"
  },
  "suppressions": []
}
-->


