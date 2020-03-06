---
title: tipo de recurso dataPolicyOperation
description: Representa uma operação de política de dados enviada. Ele contém informações necessárias para controlar o status de uma operação. Por exemplo, um administrador da empresa pode enviar uma solicitação de operação de política de dados para exportar os dados da empresa de um funcionário e, posteriormente, rastrear essa solicitação.
author: ''
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 80222ac0ab75d5ca3b67c62401b87882cc5b0209
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531726"
---
# <a name="datapolicyoperation-resource-type"></a>tipo de recurso dataPolicyOperation

Namespace: microsoft.graph

Representa uma operação de política de dados enviada. Ele contém informações necessárias para controlar o status de uma operação. Por exemplo, um administrador da empresa pode enviar uma solicitação de operação de política de dados para exportar os dados da empresa de um funcionário e, posteriormente, rastrear essa solicitação.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter dataPolicyOperation](../api/datapolicyoperation-get.md) | [dataPolicyOperation](datapolicyoperation.md) |Recupere as propriedades do objeto **dataPolicyOperation** .|
|[Exportar dados pessoais](../api/user-exportpersonaldata.md) | Nenhum |Enviar uma solicitação de operação de política de dados para exportar dados do usuário organizacional que podem ser lidas novamente usando [Get dataPolicyOperation](../api/datapolicyoperation-get.md)|

## <a name="properties"></a>Propriedades

> **Observação:** Todas as propriedades deste recurso são somente leitura.

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|completedDateTime|DateTimeOffset|Representa quando a solicitação para esta operação de política de dados foi concluída, em horário UTC, usando o formato ISO 8601. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Nulo até que a operação seja concluída.|
|id|String| Chave exclusiva para esta operação. |
|status|cadeia de caracteres| Os valores possíveis são: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.|
|storageLocation|String|O local da URL para o qual os dados estão sendo exportados para solicitações de exportação.|
|userId|Cadeia de caracteres|A ID do usuário em que a operação é executada.|
|submittedDateTime|DateTimeOffset|Representa quando a solicitação para esta operação de dados foi enviada, em horário UTC, usando o formato ISO 8601. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|progresso|String|Especifica o progresso de uma operação.|

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
  "progress": "String (double)"
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
