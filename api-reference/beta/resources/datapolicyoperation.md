---
title: tipo de recurso dataPolicyOperation
description: Representa uma operação de política de dados enviada. Ele contém informações necessárias para controlar o status de uma operação. Por exemplo, um administrador da empresa pode enviar uma solicitação de operação de política de dados para exportar os dados da empresa de um funcionário e, posteriormente, rastrear essa solicitação.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 07c708ac2d46e23cc4bdcea233587c910d30fc3e
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657711"
---
# <a name="datapolicyoperation-resource-type"></a>tipo de recurso dataPolicyOperation

Representa uma operação de política de dados enviada. Ele contém informações necessárias para controlar o status de uma operação. Por exemplo, um administrador da empresa pode enviar uma solicitação de operação de política de dados para exportar os dados da empresa de um funcionário e, posteriormente, rastrear essa solicitação.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter dataPolicyOperation](../api/datapolicyoperation-get.md) | [dataPolicyOperation](datapolicyoperation.md) |Leia as propriedades do objeto dataPolicyOperation.|

## <a name="properties"></a>Propriedades

> **Observação:** Todas as propriedades deste recurso são somente leitura.

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|completedDateTime|DateTimeOffset|Representa quando a solicitação para esta operação de política de dados foi concluída, em horário UTC, usando o formato ISO 8601. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Nulo até que a operação seja concluída.|
|id|String| Chave exclusiva para esta operação. |
|status|cadeia de caracteres| Os valores possíveis são: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.|
|storageLocation|String|O local da URL para o qual os dados estão sendo exportados para solicitações de exportação.|
|userId|Cadeia de caracteres|A ID do usuário em que a operação é executada.|
|submittedDateTime|DateTimeOffset|Representa quando a solicitação para esta operação de dados foi enviada, em horário UTC, usando o formato ISO 8601. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|progresso|Duplo|Especifica o progresso de uma operação.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.dataPolicyOperation"
}-->

```json
{
  "completedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "status": "string",
  "storageLocation": "String",
  "userId": "String",
  "submittedDateTime": "String (timestamp)",
  "progress": "Double"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "dataPolicyOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
