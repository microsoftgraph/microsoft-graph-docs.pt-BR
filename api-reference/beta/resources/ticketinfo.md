---
title: Tipo de recurso ticketInfo
description: O objeto que representa informações de tíquete relacionadas a solicitações de atribuição de função
author: shauliu1
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b3a330071fa6d17ff510901376d1fb3b0c1c0cdb
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59023112"
---
# <a name="ticketinfo-resource-type"></a>Tipo de recurso ticketInfo

Namespace: microsoft.graph

O objeto que representa informações de tíquete relacionadas a solicitações de atribuição de função

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ticketNumber|Cadeia de caracteres|Metadados de número de tíquete|
|ticketSystem|String|Dados de meta do sistema de tíquetes|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.ticketInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.ticketInfo",
  "ticketNumber": "String",
  "ticketSystem": "String"
}
```

