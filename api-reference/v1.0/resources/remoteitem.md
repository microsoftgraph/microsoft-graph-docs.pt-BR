---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: RemoteItem
ms.openlocfilehash: 549b0804a1d6449a71d2cc870836c0d044099a38
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2018
ms.locfileid: "23264270"
---
# <a name="remoteitem-resource-type"></a>Tipo de recurso RemoteItem

O recurso **remoteItem** indica que um [**driveItem**](driveitem.md) faz referência a um item que existe em outra unidade. Este recurso fornece as IDs exclusivas do da unidade de origem e do item de destino.

[**DriveItems**](driveitem.md) com uma faceta **remoteItem** não nula são recursos que são compartilhados, adicionados ao OneDrive do usuário ou em itens retornados de coleções de itens heterogêneas (como resultados de pesquisa).

**Observação:** Diferentemente de pastas na mesma unidade, um **driveItem** movido para um item remoto pode ter seu valor `id` alterado.

## <a name="json-representation"></a>Representação JSON

<!-- { "blockType": "resource", 
       "@odata.type": "microsoft.graph.remoteItem", 
       "optionalProperties": ["name", "fileSystemInfo", "file", "folder"] } -->

```json
{
  "id": "string",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "timestamp",
  "file": { "@odata.type": "microsoft.graph.file" },
  "fileSystemInfo": { "@odata.type": "microsoft.graph.fileSystemInfo" },
  "folder": { "@odata.type": "microsoft.graph.folder" },
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "name": "string",
  "package": { "@odata.type": "microsoft.graph.package" },
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "shared": { "@odata.type": "microsoft.graph.shared" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "specialFolder": { "@odata.type": "microsoft.graph.specialFolder" },
  "size": 1024,
  "webDavUrl": "url",
  "webUrl": "url"
}
```

## <a name="properties"></a>Propriedades

| Nome da propriedade        | Tipo                                | Descrição                                                                                                                                                       |
| :------------------- | :---------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| createdBy            | [IdentitySet](identityset.md)       | Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.                                                                                  |
| createdDateTime      | Carimbo de data/hora                           | Data e hora de criação do item. Somente leitura.                                                                                                                        |
| file                 | [Arquivo](file.md)                     | Indica que o item remoto é um arquivo. Somente leitura.                                                                                                              |
| fileSystemInfo       | [FileSystemInfo](filesysteminfo.md) | Informações sobre o item remoto do sistema de arquivos local. Somente leitura.                                                                                          |
| folder               | [Pasta](folder.md)                 | Indica que o item remoto é uma pasta. Somente leitura.                                                                                                            |
| id                   | Sequência de caracteres                              | Identificador exclusivo do item remoto em sua unidade. Somente leitura.                                                                                                    |
| lastModifiedBy       | [IdentitySet](identityset.md)       | Identidade do usuário, dispositivo e aplicativo que modificou o item pela última vez. Somente leitura.                                                                            |
| lastModifiedDateTime | Carimbo de data/hora                           | Data e hora em que o item foi modificado pela última vez. Somente leitura.                                                                                                              |
| name                 | Sequência de caracteres                              | Opcional. Nome de arquivo do item remoto. Somente leitura.                                                                                                                 |
| pacote              | [Pacote](package.md)               | Se presente, indica que esse item é um pacote, e não uma pasta ou um arquivo. Pacotes são tratados como arquivos em alguns contextos e como pastas em outros. Somente leitura. |
| parentReference      | [ItemReference](itemreference.md)   | Propriedades do pai do item remoto. Somente leitura.                                                                                                           |
| shared               | [shared](shared.md)                 | Indica que o item foi compartilhado com outras pessoas e fornece informações sobre o estado compartilhado desse item. Somente leitura.                                       |
| sharepointIds        | [SharepointIds](sharepointids.md)   | Fornece interoperabilidade entre itens no OneDrive for Business e no SharePoint com o conjunto completo de identificadores de item. Somente leitura.                                          |
| size                 | Int64                               | Tamanho do item remoto. Somente leitura.                                                                                                                               |
| specialFolder        | [specialFolder][]                   | Se o item atual também estiver disponível como uma pasta especial, essa faceta será retornada. Somente leitura.                                                                     |
| webDavUrl            | URL                                 | URL compatível com DAV para o item.                                                                                                                                  |
| webUrl               | URL                                 | URL que exibe o recurso no navegador. Somente leitura.                                                                                                         |

[specialFolder]: specialFolder.md

## <a name="remarks"></a>Comentários

Para saber mais sobre as facetas de um **driveItem**, confira [driveItem](driveitem.md).

<!-- {
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/RemoteItem"
} -->