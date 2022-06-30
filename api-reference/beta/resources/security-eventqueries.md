---
title: Tipo de recurso eventQuery
description: Representa a carga de trabalho (SharePoint Online, OneDrive for Business, Exchange Online) e informações de identificação associadas a um evento de retenção.
author: sseth
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: bfdb65f2609947b6cc820c5c4937925c5b340115
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447535"
---
# <a name="eventquery-resource-type"></a>Tipo de recurso eventQuery

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a carga de trabalho (SharePoint Online, OneDrive for Business, Exchange Online) e informações de identificação associadas a um evento de retenção.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|queryType|microsoft.graph.security.queryType|Representa o tipo de consulta associado a um evento. 'files' para SPO e ODB e 'mensagens' para EXO. Os valores possíveis são: `files`, `messages`, `unknownFutureValue`.|
|consulta|Cadeia de caracteres|Representa a identificação exclusiva da consulta. 'ID do ativo' para o SharePoint Online e OneDrive for Business, 'palavras-chave' para Exchange Online.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.security.eventQueries"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.eventQuery",
  "queryType": "String",
  "query": "String"
}
```


