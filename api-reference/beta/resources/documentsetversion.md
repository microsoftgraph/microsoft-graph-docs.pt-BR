---
title: Tipo de recurso documentSetVersion
description: Representa a versão de um item de conjunto de documentos em uma lista.
author: swapnil1993
ms.localizationpriority: medium
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: c86cad9d0e5fe251c3d67145f56c9de2578b22c3
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2022
ms.locfileid: "65061164"
---
# <a name="documentsetversion-resource-type"></a>Tipo de recurso documentSetVersion

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a versão de um item de conjunto de documentos em uma lista.

Herda de [listItemVersion](../resources/listitemversion.md).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar documentSetVersions](../api/listitem-list-documentsetversions.md)|[coleção documentSetVersion](../resources/documentsetversion.md)|Obtenha os [recursos documentSetVersion](../resources/documentsetversion.md) da **propriedade de navegação documentSetVersions** .|
|[Criar documentSetVersion](../api/listitem-post-documentsetversions.md)|[documentSetVersion](../resources/documentsetversion.md)|Crie um novo [objeto documentSetVersion](../resources/documentsetversion.md) .|
|[Obter documentSetVersion](../api/documentsetversion-get.md)|[documentSetVersion](../resources/documentsetversion.md)|Leia as propriedades e as relações de um [objeto documentSetVersion](../resources/documentsetversion.md) .|
|[Excluir documentSetVersion](../api/documentsetversion-delete.md)|Nenhum|[Exclua um objeto documentSetVersion](../resources/documentsetversion.md).|
|[Restaurar](../api/documentsetversion-restore.md)|[documentSetVersion](../resources/documentsetversion.md)|Restaure [um documentSetVersion](../resources/documentsetversion.md).|


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
| comment | string | Comente sobre a versão capturada.|
| createdBy   | [identitySet](../resources/identityset.md) | Usuário que capturou a versão.|
| createdDateTime     | dateTime | Data e hora em que esta versão foi criada.|
| id                  | string                                               | A ID da versão. Somente leitura. Herdado de [listItemVersion](../resources/listitemversion.md).|
| items     | [Coleção documentSetVersionItem](../resources/documentsetversionitem.md) | Itens dentro do conjunto de documentos capturados como parte desta versão.|
| lastModifiedBy       | [identitySet](../resources/identityset.md)           | Identidade do usuário que modificou a versão pela última vez. Somente leitura. Herdado de [listItemVersion](../resources/listitemversion.md).|
| lastModifiedDateTime | [Datetimeoffset](../resources/timestamp.md)          | Data e hora em que a versão foi modificada pela última vez. Somente leitura. Herdado de [listItemVersion](../resources/listitemversion.md).     |
| Publicado            | [publicationFacet](../resources/publicationfacet.md) | Indica o status de publicação desta versão específica. Somente leitura. Herdado de [listItemVersion](../resources/listitemversion.md).| 
| shouldCaptureMinorVersion | booliano  | Se `true`, versões secundárias de itens também forem capturadas; caso contrário, somente as versões principais serão capturadas. O valor padrão é `false`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
| campos        | [fieldValueSet](../resources/fieldvalueset.md) | Uma coleção de campos e valores para esta versão do item da lista. |

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.documentSetVersion",
  "baseType": "microsoft.graph.listItemVersion",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.documentSetVersion",
  "comment": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "id": "String (identifier)",
  "items": [
    {
      "@odata.type": "microsoft.graph.documentSetVersionItem"
    }
  ],
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "publication": {
    "@odata.type": "microsoft.graph.publicationFacet"
  },
  "shouldCaptureMinorVersion": "Boolean"
}
```

