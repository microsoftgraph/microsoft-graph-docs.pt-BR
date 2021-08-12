---
title: tipo de recurso de configuração
description: Especifica IDs de aplicativo adicionais que podem gerenciar o externalConnection e indexar conteúdo em um externalConnection.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 213c24c9388f555d772f2c0243b1d55d023239922d059b63478a8953ac6d5b25
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54141669"
---
# <a name="configuration-resource-type"></a>tipo de recurso de configuração

Namespace: microsoft.graph.externalConnectors



Especifica IDs de aplicativo adicionais que podem gerenciar o externalConnection e indexar conteúdo em [um externalConnection](../resources/externalconnectors-externalconnection.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|authorizedAppIds|Coleção de cadeias de caracteres|Uma coleção de IDs de aplicativos para aplicativos Azure Active Directory registrados que podem gerenciar o externalConnection e indexar conteúdo no externalConnection.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.externalConnectors.configuration"
}
-->
``` json
{
  "authorizedAppIds": [
    "String"
  ]
}
```

