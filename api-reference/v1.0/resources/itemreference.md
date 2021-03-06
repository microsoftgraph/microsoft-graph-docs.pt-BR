---
author: JeremyKelley
ms.date: 09/10/2017
title: ItemReference
localization_priority: Normal
description: O recurso ItemReference proporciona as informações necessárias para enviar um DriveItem pela API.
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: dd24f0d1fc0a5f5db576f5eea89b8205ff55b2b7
ms.sourcegitcommit: 0d4377b0153bc339ab7b3b1a6ee4d52848b622d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2020
ms.locfileid: "49714253"
---
# <a name="itemreference-resource-type"></a>Tipo de recurso ItemReference

Namespace: microsoft.graph

O recurso **ItemReference** proporciona as informações necessárias para enviar um [DriveItem](driveitem.md) pela API.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "path", "shareId", "sharepointIds" ],
  "@odata.type": "microsoft.graph.itemReference"
}-->

```json
{
  "driveId": "string",
  "driveType": "personal | business | documentLibrary",
  "id": "string",
  "name": "string",
  "path": "string",
  "shareId": "string",
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "siteId": "string"
}
```

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo              | Descrição
|:--------------|:------------------|:-----------------------------------------
| driveId       | String            | O identificador exclusivo da instância da unidade que contém o item. Somente leitura.
| driveType     | String            | Identifica o tipo de unidade. Consulte o recurso [unidade][] para obter os valores.
| id            | Cadeia de caracteres            | Identificador exclusivo do item na unidade. Somente leitura.
| nome          | Cadeia de caracteres            | O nome do item ao qual se faz referência. Somente leitura.
| caminho          | String            | Caminho que pode ser usado para navegar até o item. Somente leitura.
| shareId       | Cadeia de caracteres            | Um identificador exclusivo para um recurso compartilhado que pode ser acessado através da API [Shares][].
| sharepointIds | [sharepointIds][] | Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.
| siteId        | Cadeia de caracteres            | Para o OneDrive for Business e o SharePoint, essa propriedade representa a ID do site que contém a biblioteca de documentos pai do recurso driveItem. O valor é o mesmo que a propriedade ID do recurso [site][] . É uma [cadeia de caracteres opaca que consiste em três identificadores](/graph/api/resources/site#id-property) do site. <br>Para o OneDrive, essa propriedade não é preenchida.

[unidade]: ../resources/drive.md
[sharepointIds]: ../resources/sharepointids.md
[Shares]: ../api/shares-get.md
[site]: ../resources/site.md

## <a name="remarks"></a>Comentários

Para lidar com um **driveItem** de um recurso **itemReference**, crie uma URL no formato:

```http
GET https://graph.microsoft.com/v1.0/drives/{driveId}/items/{id}
```

O valor **path** é um caminho da API relativo à unidade de destino, por exemplo: `/drive/root:/Documents/myfile.docx`.

Para recuperar o caminho legível para a navegação estrutural, ignore tudo até o primeiro `:` na cadeia de caracteres do caminho.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ItemReference returns a pointer to another item.",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/itemreference.md:
      Found potential enums in resource example that weren't defined in a table:(personal,business,documentLibrary) are in resource, but () are in table"
  ],
  "tocPath": "Resources/ItemReference"
} -->

