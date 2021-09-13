---
title: Tipo de recurso publicErrorDetail
description: Representa os detalhes de um erro.
author: AkJo
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3965fd862fee8e4e571055bdc37ade80909c9e97
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59104065"
---
# <a name="publicerrordetail-resource-type"></a>Tipo de recurso publicErrorDetail

Namespace: microsoft.graph

Representa os detalhes [de publicError](../resources/publicerror.md) ou [publicInnerError](../resources/publicinnererror.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|código|Cadeia de caracteres|O código de erro.|
|mensagem|String|A mensagem de erro.|
|destino|Cadeia de caracteres|O destino do erro.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.publicErrorDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.publicErrorDetail",
  "code": "String",
  "message": "String",
  "target": "String"
}
```
