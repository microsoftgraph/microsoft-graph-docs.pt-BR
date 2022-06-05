---
title: Tipo de recurso ticketInfo
description: Representa informações de tíquete relacionadas a solicitações de qualificação e atribuição de função.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e2356ef6fdbf0d1832d79fc2b68ecbef69db1ede
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900461"
---
# <a name="ticketinfo-resource-type"></a>Tipo de recurso ticketInfo

Namespace: microsoft.graph

Representa informações de tíquete relacionadas a solicitações de qualificação e atribuição de função. Use este objeto para definir parâmetros de tíquete para uma atribuição de função ou solicitação de qualificação é iniciada por outra solicitação feita em um sistema externo.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ticketNumber|Cadeia de Caracteres|O número do tíquete.|
|ticketSystem|String|A descrição do sistema de tíquetes.|

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

