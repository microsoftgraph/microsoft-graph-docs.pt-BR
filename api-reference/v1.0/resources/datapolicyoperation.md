---
title: Tipo de recurso dataPolicyOperation
description: Representa uma operação de política de dados enviada. Ele contém informações necessárias para controlar o status de uma operação. Por exemplo, um administrador da empresa pode enviar uma solicitação de operação de política de dados para exportar dados da empresa de um funcionário e, em seguida, rastrear essa solicitação.
author: dkershaw10
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 27843a57190910584bcc09c4f65aa75314e3ab1c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50449009"
---
# <a name="datapolicyoperation-resource-type"></a>Tipo de recurso dataPolicyOperation

Namespace: microsoft.graph

Representa uma operação de política de dados enviada. Ele contém informações necessárias para controlar o status de uma operação. Por exemplo, um administrador da empresa pode enviar uma solicitação de operação de política de dados para exportar dados da empresa de um funcionário e, em seguida, rastrear essa solicitação.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter dataPolicyOperation](../api/datapolicyoperation-get.md) | [dataPolicyOperation](datapolicyoperation.md) |Recupere propriedades do **objeto dataPolicyOperation.**|
|[Exportar dados pessoais](../api/user-exportpersonaldata.md) | Nenhum |Enviar uma solicitação de operação de política de dados para exportar os dados do usuário organizacional que podem ser lidos posteriormente usando [Get dataPolicyOperation](../api/datapolicyoperation-get.md)|

## <a name="properties"></a>Propriedades

> **Observação:** Todas as propriedades desse recurso são somente leitura.

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|completedDateTime|DateTimeOffset|Representa quando a solicitação para essa operação de política de dados foi concluída, em tempo UTC, usando o formato ISO 8601. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Nulo até que a operação seja concluída.|
|id|Cadeia de caracteres| Chave exclusiva para essa operação. |
|status|cadeia de caracteres| Os valores possíveis são: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.|
|storageLocation|Cadeia de caracteres|O local da URL para onde os dados estão sendo exportados para solicitações de exportação.|
|userId|Cadeia de caracteres|A id do usuário no qual a operação é executada.|
|submittedDateTime|DateTimeOffset|Representa quando a solicitação para essa operação de dados foi enviada, em tempo UTC, usando o formato ISO 8601. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
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

