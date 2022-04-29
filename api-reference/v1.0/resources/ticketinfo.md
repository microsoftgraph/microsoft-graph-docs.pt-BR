---
title: Tipo de recurso ticketInfo
description: Representa informações de tíquete relacionadas a solicitações de qualificação e atribuição de função.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e2356ef6fdbf0d1832d79fc2b68ecbef69db1ede
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133857"
---
# <a name="ticketinfo-resource-type"></a>Tipo de recurso ticketInfo

Namespace: microsoft.graph

Representa informações de tíquete relacionadas a solicitações de qualificação e atribuição de função. Use este objeto para definir parâmetros de tíquete para uma atribuição de função ou solicitação de qualificação é iniciada por outra solicitação feita em um sistema externo.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ticketNumber|Cadeia de caracteres|O número do tíquete.|
|ticketSystem|Cadeia de caracteres|A descrição do sistema de tíquetes.|

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

