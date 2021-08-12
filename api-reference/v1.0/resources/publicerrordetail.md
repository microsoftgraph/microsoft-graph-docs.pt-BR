---
title: Tipo de recurso publicErrorDetail
description: Representa os detalhes de um erro.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 123655f1f75d9d05ec95d1e9e0c15815c341aa11fffb72c6f59c34bf1572bd8b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54138343"
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
