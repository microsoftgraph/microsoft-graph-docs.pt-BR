---
title: Tipo de recurso connectionOperation
description: Descreve o status de uma solicitação assíncrona para criar um Pesquisa da Microsoft de conexão.
author: mecampos
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: dac175f73b517e3f96c6d5e03ce747d32b2b8f64
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59123458"
---
# <a name="connectionoperation-resource-type"></a>Tipo de recurso connectionOperation

Namespace: microsoft.graph.externalConnectors



Descreve o status de uma solicitação assíncrona para criar um Pesquisa da Microsoft [de conexão](externalconnectors-schema.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter connectionOperation](../api/externalconnectors-connectionoperation-get.md)|[connectionOperation](../resources/externalconnectors-connectionoperation.md)|Leia as propriedades e as relações de um [objeto connectionOperation.](../resources/externalconnectors-connectionoperation.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|erro|publicError| Se `status` for , fornece mais informações sobre o erro que causou a `failed` falha.|
|id|Cadeia de caracteres| Identificador exclusivo da connectionOperation. Somente leitura. |
|status|microsoft.graph.externalConnectors.connectionOperationStatus| Indica o status da operação assíncrona. Os valores possíveis são: `unspecified`, `inprogress`, `completed`, `failed`, `unknownFutureValue`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalConnectors.connectionOperation",
  "openType": false
}
-->
``` json
{
  "id": "String (identifier)",
  "status": "String"
}
```

