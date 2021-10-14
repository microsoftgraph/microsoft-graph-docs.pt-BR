---
title: Tipo de recurso driveItemVersion
description: Representa uma versão específica de um DriveItem.
ms.localizationpriority: medium
ms.prod: sharepoint
author: JeremyKelley
doc_type: resourcePageType
ms.openlocfilehash: 9dea3f33013c4d6fe0530c4f65253873ec3a1a69
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2021
ms.locfileid: "60354760"
---
# <a name="driveitemversion-resource-type"></a>Tipo de recurso driveItemVersion

Namespace: microsoft.graph

Representa uma versão específica de [um driveItem](driveitem.md).

As tarefas a seguir estão disponíveis para **recursos driveItemVersion.**

|            Tarefa comum             |         Método HTTP         |
| :--------------------------------- | :-------------------------- |
| [Listar versões][version-list]      | `GET /drive/items/{item-id}/versions`  |
| [Obter versão][version-get]         | `GET /drive/items/{item-id}/versions/{version-id}`     |
| [Obter conteúdo][content-get]        | `GET /drive/items/{item-id}/versions/{version-id}/content` |
| [Restaurar versão][version-restore] | `POST /drive/items/{item-id}/versions/{version-id}/restoreversion` |

[version-list]: ../api/driveitem-list-versions.md
[version-get]: ../api/driveitemversion-get.md
[content-get]: ../api/driveitemversion-get-contents.md
[version-restore]: ../api/driveitemversion-restore.md

Na tabela anterior, os exemplos usam `/drive`, mas há muitas solicitações válidas.

## <a name="properties"></a>Propriedades

|      Nome da propriedade       |                         Tipo                         |                               Descrição                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| **id**                   | string                                               | A ID da versão. Somente leitura.                                       |
| **lastModifiedBy**       | [IdentitySet](../resources/identityset.md)           | Identidade do usuário que modificou a versão pela última vez. Somente leitura.        |
| **lastModifiedDateTime** | [DateTimeOffset](../resources/timestamp.md)          | Data e hora em que a versão foi modificada pela última vez. Somente leitura.                 |
| **publication**          | [PublicationFacet](../resources/publicationfacet.md) | Indica o status de publicação desta versão específica. Somente leitura. |
| **size**                 | Int64                                                | Indica o tamanho do fluxo de conteúdo para esta versão do item.  |
| **content**              | Fluxo                                               | O fluxo de conteúdo para esta versão do item.                        |

## <a name="instance-attributes"></a>Atributos de instância

| Nome da propriedade                     | Tipo   | Descrição
|:----------------------------------|:-------|:--------------------------------
| @microsoft.graph.downloadUrl      | string | Uma URL que pode ser usada para baixar essa versão do conteúdo do arquivo. Uma autenticação não é obrigatória com essa URL. Somente leitura.

>**Observações:** O `@microsoft.graph.downloadUrl` valor é uma URL de curta duração e não pode ser armazenado em cache. A URL só estará disponível por um curto período de tempo (1 hora) antes de ser invalidada.
>Remover permissões de arquivo para um usuário pode não invalidar imediatamente o URL.

## <a name="json-representation"></a>Representação JSON

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.baseItemVersion",
  "@odata.type": "microsoft.graph.driveItemVersion",
  "@type.aka": "oneDrive.driveItemVersion"
}-->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": { "@odata.type": "microsoft.graph.publicationFacet" },
  "size": 12356,

  /* instance annotations */
  "@microsoft.graph.downloadUrl": "url",
}
```


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
