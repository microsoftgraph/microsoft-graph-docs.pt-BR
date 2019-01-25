---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: FileSystemInfo
localization_priority: Normal
ms.openlocfilehash: e2dfac79f5c7d511cab11c076d697940a01f4c7c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524692"
---
# <a name="filesysteminfo-facet"></a>Faceta fileSystemInfo

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso FileSystemInfo contém propriedades que são relatadas pelo sistema de arquivos local do dispositivo para a versão local de um item. Esta faceta pode ser usada para especificar a data da última modificação ou a data de criação do item como estava no dispositivo local.

Ele está disponível na propriedade fileSystemInfo dos recursos [driveItem] [ item-resource].

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "lastAccessedDateTime"
  ],
  "@odata.type": "microsoft.graph.fileSystemInfo"
}-->

```json
{
  "createdDateTime" : "datetime",
  "lastAccessedDateTime": "datetime",
  "lastModifiedDateTime" : "datetime"
}
```

## <a name="properties"></a>Propriedades

| Propriedade                 | Tipo           | Descrição                                                                                                          |
| :----------------------- | :------------- | :------------------------------------------------------------------------------------------------------------------- |
| **createdDateTime**      | DateTimeOffset | A data e a hora UTC da criação do arquivo em um cliente.                                                              |
| **lastAccessedDateTime** | DateTimeOffset | A data e hora UTC em que o arquivo foi acessado pela última vez. Disponível para o lista de arquivos recentes apenas. |
| **lastModifiedDateTime** | DateTimeOffset | A data e hora UTC em que o arquivo foi modificado pela última vez em um cliente.                                                        |

## <a name="notes"></a>Observações

Os valores para createdDateTime e lastModifiedDateTime variam em relação às mesmas propriedades no recurso DriveItem. Os valores no recurso DriveItem são a data e a hora de criação e modificação, como visto do serviço. Os valores armazenados no recurso FileSystemInfo são fornecidos pelo cliente.

Por exemplo, se um arquivo foi criado no dispositivo na segunda-feira, mas não foi carregado no serviço até terça-feira, o cliente que carrega o arquivo deve gravar a faceta `fileSystemInfo` para incluir a data de criação na segunda-feira. Quando os metadados de item forem recuperados, a data de criação do item refletirá terça-feira, mas a faceta `fileSystemInfo` mostrará a data de criação original na segunda-feira.

Estas propriedades são somente leitura. Se estiver carregando um arquivo e souber os valores do cliente local para estes campos, você deverá incluí-los na solicitação.

Se o conteúdo do arquivo for atualizado e estas propriedades não forem fornecidas, **lastModifiedDateTime** será redefinido automaticamente como a hora atual.

## <a name="remarks"></a>Comentários

* **lastAccessedDateTime** não está disponível para itens no SharePoint Online ou OneDrive for Business.

Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).

[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "The fileSystemInfo facet provides information about date created and modified by clients.",
  "keywords": "fileSystemInfo,client,system info,onedrive",
  "section": "documentation",
  "tocPath": "Facets/FileSystemInfo",
  "suppressions": [
    "Error: /api-reference/beta/resources/filesysteminfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
