---
title: tipo de recurso de dataPolicyOperation
description: Representa uma operação de diretiva de dados enviados. Ele contém as informações necessárias para rastrear o status de uma operação. Por exemplo, um administrador da empresa pode enviar uma solicitação de operação de política de dados para exportar os dados da empresa de um funcionário e, em seguida, rastrear mais tarde que a solicitação.
localization_priority: Normal
ms.openlocfilehash: b56cfe766bbfcae9339805dd61ce816e372d02f4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876003"
---
# <a name="datapolicyoperation-resource-type"></a>tipo de recurso de dataPolicyOperation

Representa uma operação de diretiva de dados enviados. Ele contém as informações necessárias para rastrear o status de uma operação. Por exemplo, um administrador da empresa pode enviar uma solicitação de operação de política de dados para exportar os dados da empresa de um funcionário e, em seguida, rastrear mais tarde que a solicitação.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter dataPolicyOperation](../api/datapolicyoperation-get.md) | [dataPolicyOperation](datapolicyoperation.md) |Leia as propriedades do objeto dataPolicyOperation.|

## <a name="properties"></a>Propriedades

> **Observação:** Todas as propriedades desse recurso são somente leitura.

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|completedDateTime|DateTimeOffset|Representa quando a solicitação para esta operação de política de dados foi concluída, em tempo de UTC, usando o formato ISO 8601. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Nulo até que a operação seja concluída.|
|id|Cadeia de caracteres| Chave exclusiva para essa operação. |
|status|string| Os valores possíveis são: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.|
|storageLocation|Cadeia de caracteres|O local da URL para onde os dados está sendo exportados para solicitações de exportação.|
|userId|Cadeia de caracteres|A identificação do usuário no qual a operação é executada.|
|submittedDateTime|DateTimeOffset|Representa quando a solicitação para esta operação de dados foi enviada, em tempo de UTC, usando o formato ISO 8601. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
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
