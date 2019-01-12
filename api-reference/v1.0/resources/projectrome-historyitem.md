---
title: tipo de recurso de historyItem
description: Representa um item de histórico de uma atividade em um aplicativo. As atividades do usuário representam um único destino dentro de seu aplicativo - por exemplo, um programa de TV, um documento ou uma campanha atual em um jogo de vídeo. Quando um usuário emprega com que a atividade, o compromisso é capturado como um item de histórico que indica a hora de início e término para a atividade. À medida que o usuário emprega novamente com que a atividade ao longo do tempo, vários itens de histórico são registrados para atividade de um único usuário.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 029c17e09348977752f3ce5632740b2bdac64e46
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977434"
---
# <a name="historyitem-resource-type"></a>tipo de recurso de historyItem

Representa um item de histórico de uma [atividade](projectrome-activity.md) em um aplicativo. As atividades do usuário representam um único destino dentro de seu aplicativo - por exemplo, um programa de TV, um documento ou uma campanha atual em um jogo de vídeo. Quando um usuário emprega com que a atividade, o compromisso é capturado como um item de histórico que indica a hora de início e término para a atividade. À medida que o usuário emprega novamente com que a atividade ao longo do tempo, vários itens de histórico são registrados para atividade de um único usuário.

Quando um aplicativo cria uma sessão, um objeto **historyItem** deve ser adicionado ao objeto **atividade** para refletir o período de participação do usuário. Cada vez que um usuário emprega-se novamente com uma atividade, um novo **historyItem** é adicionado à atividade acumular compromisso do usuário.

## <a name="methods"></a>Métodos

|Método | Tipo de retorno | Descrição|
|:------|:------------|:-----------|
|[Criar ou substituir historyItem](../api/projectrome-put-historyitem.md) | [historyItem](projectrome-historyitem.md) | Cria ou substitui um existente **historyItem** para a atividade (upsert). A ID deve ser um GUID.|
|[Excluir um historyItem](../api/projectrome-delete-historyitem.md) | Nenhum conteúdo | Exclui o **historyItem** especificado para a atividade.|

## <a name="properties"></a>Propriedades

|Nome | Tipo | Descrição|
|:----|:-----|:-----------|
|status | status | Definido pelo servidor. Um código de status usado para identificar objetos válidos. Valores: ativo, atualizado, excluídos, ignorado.|
|userTimezone | Cadeia de caracteres | Opcional. O fuso horário no qual o dispositivo do usuário usado para gerar a atividade foi localizado no momento da criação de atividade. Valores fornecidos como Olson IDs para suportar a representação de plataforma cruzada.|
|createdDateTime | DateTimeOffset | Definido pelo servidor. Data e hora em UTC quando o objeto foi criado no servidor.|
|lastModifiedDateTime | DateTimeOffset | Definido pelo servidor. Data e hora em UTC quando o objeto foi modificado no servidor.|
|id | Cadeia de caracteres | Obrigatório. GUID do conjunto de cliente para o objeto **historyItem** .|
|startedDateTime | DateTimeOffset | Obrigatório. DateTime UTC quando **historyItem** (sessão atividade) foi iniciado. Necessário para o histórico de linha do tempo.|
|lastActiveDateTime | DateTimeOffset | Opcional. DateTime UTC quando **historyItem** (sessão atividade) foi compreendido última como status ativo ou terminar - se for null, **historyItem** deve ser contínuo.|
|expirationDateTime | DateTimeOffset | Opcional. DateTime UTC quando os **historyItem** passará rígido-delete. Pode ser definido pelo cliente.|
|activeDurationSeconds | int | Opcional. A duração de participação de usuário ativo. Se não fornecido, isso é calculado do **startedDateTime** e **lastActiveDateTime**.|

## <a name="relationships"></a>Relações

|Relação | Tipo | Descrição|
|:------------|:-----|:-----------|
|atividade| [userActivity](../resources/projectrome-activity.md) | Opcional. NavigationProperty/contenção; propriedade de navegação à atividade associada.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "userTimezone",
    "lastActiveDateTime",
    "activeDurationSeconds"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.activityHistoryItem",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "countable": false,
        "selectable": false
      }
    }
  ]
}-->

```json
{
    "status": "active | updated | deleted | ignored",
    "createdDateTime": "DateTimeOffset",
    "lastModifiedDateTime": "DateTimeOffset",
    "id": "String",
    "expirationDateTime": "DateTimeOffset",
    "startedDateTime": "DateTimeOffset",
    "userTimezone": "String",
    "lastActiveDateTime": "DateTimeOffset",
    "activeDurationSeconds":"int"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "historyitem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
