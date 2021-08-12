---
title: Tipo de recurso dataPolicyOperation
description: Representa uma operação de política de dados enviada. Ele contém informações necessárias para controlar o status de uma operação. Por exemplo, um administrador da empresa pode enviar uma solicitação de operação de política de dados para exportar dados da empresa de um funcionário e, em seguida, rastrear essa solicitação.
author: dkershaw10
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: c96650636e385eeddeecd9ab8c22ff2ee986108deadf973b2cfed9973134c6a2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54178525"
---
# <a name="datapolicyoperation-resource-type"></a>Tipo de recurso dataPolicyOperation

Namespace: microsoft.graph

Representa uma operação de política de dados enviada. Ele contém informações necessárias para controlar o status de uma operação. Por exemplo, um administrador da empresa pode enviar uma solicitação de operação de política de dados para exportar dados da empresa de um funcionário e, em seguida, rastrear essa solicitação.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter dataPolicyOperation](../api/datapolicyoperation-get.md) | [dataPolicyOperation](datapolicyoperation.md) |Recupere propriedades do **objeto dataPolicyOperation.**|
|[Exportar dados pessoais](../api/user-exportpersonaldata.md) | None |Enviar uma solicitação de operação de política de dados para exportar os dados do usuário organizacional que podem ser lidos posteriormente usando [Get dataPolicyOperation](../api/datapolicyoperation-get.md)|

## <a name="properties"></a>Propriedades

> **Observação:** Todas as propriedades desse recurso são somente leitura.

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|completedDateTime|DateTimeOffset|Representa quando a solicitação para essa operação de política de dados foi concluída, em tempo UTC, usando o formato ISO 8601. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Nulo até que a operação seja concluída.|
|id|String| Chave exclusiva para essa operação. |
|status|dataPolicyOperationStatus| Os valores possíveis são: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.|
|storageLocation|Cadeia de caracteres|O local da URL para onde os dados estão sendo exportados para solicitações de exportação.|
|userId|Cadeia de caracteres|A id do usuário no qual a operação é executada.|
|submittedDateTime|DateTimeOffset|Representa quando a solicitação para essa operação de dados foi enviada, em tempo UTC, usando o formato ISO 8601. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|progresso|Cadeia de caracteres|Especifica o andamento de uma operação.|

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

