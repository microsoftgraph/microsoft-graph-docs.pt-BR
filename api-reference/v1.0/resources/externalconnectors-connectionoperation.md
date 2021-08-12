---
title: Tipo de recurso connectionOperation
description: Descreve o status de uma solicitação assíncrona para criar um Pesquisa da Microsoft de conexão.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 7cf9310eef057bbd4bcda57273089f05a24501986c90b6bffbc072d39932cac2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54121281"
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

