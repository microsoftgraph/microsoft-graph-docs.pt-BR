---
author: JeremyKelley
ms.date: 09/10/2017
title: FileSystemInfo
ms.localizationpriority: medium
description: O recurso FileSystemInfo contém propriedades que são relatadas pelo sistema de arquivos local do dispositivo para a versão local de um item.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 706128b116a7a8f8b4ff1450096f3335c44b165c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59137676"
---
# <a name="filesysteminfo-facet"></a>Faceta fileSystemInfo

Namespace: microsoft.graph

O recurso **FileSystemInfo** contém propriedades que são relatadas pelo sistema de arquivos local do dispositivo para a versão local de um item. Esta faceta pode ser usada para especificar a data da última modificação ou a data de criação do item como estava no dispositivo local.

Ele está disponível na propriedade fileSystemInfo dos [recursos driveItem.][item-resource]

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
| **lastAccessedDateTime** | DateTimeOffset | A data e hora UTC em que o arquivo foi acessado pela última vez. Disponível para o [lista de arquivos recentes](../api/drive-recent.md) apenas. |
| **lastModifiedDateTime** | DateTimeOffset | A data e hora UTC em que o arquivo foi modificado pela última vez em um cliente.                                                        |

## <a name="notes"></a>Observações

Os valores para **createdDateTime** e **lastModifiedDateTime** variam em relação às mesmas propriedades no recurso [DriveItem](driveitem.md). Os valores no recurso DriveItem são a data e a hora de criação e modificação, como visto do serviço. Os valores armazenados no recurso **FileSystemInfo** são fornecidos pelo cliente.

Por exemplo, se um arquivo foi criado no dispositivo na segunda-feira, mas não foi carregado no serviço até terça-feira, o cliente que carrega o arquivo deve gravar a faceta `fileSystemInfo` para incluir a data de criação na segunda-feira. Quando os metadados de item forem recuperados, a data de criação do item refletirá terça-feira, mas a faceta `fileSystemInfo` mostrará a data de criação original na segunda-feira.

Estas propriedades são somente leitura. Se estiver carregando um arquivo e souber os valores do cliente local para estes campos, você deverá incluí-los na solicitação.

Se o conteúdo do arquivo for atualizado e estas propriedades não forem fornecidas, **lastModifiedDateTime** será redefinido automaticamente como a hora atual.

## <a name="remarks"></a>Comentários

* **lastAccessedDateTime** não está disponível para itens no SharePoint Online ou OneDrive for Business.

Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "The fileSystemInfo facet provides information about date created and modified by clients.",
  "keywords": "fileSystemInfo,client,system info,onedrive",
  "section": "documentation",
  "tocPath&quot;: &quot;Facets/FileSystemInfo"
} -->

