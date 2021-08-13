---
title: Tipo de recurso historyItem
description: Representa um item de histórico para uma atividade em um aplicativo. As atividades do usuário representam um único destino em seu aplicativo - por exemplo, um programa de TV, um documento ou uma campanha atual em um jogo de vídeo. Quando um usuário se envolve com essa atividade, o envolvimento é capturado como um item de histórico que indica a hora de início e término dessa atividade. À medida que o usuário se envolve com essa atividade ao longo do tempo, vários itens de histórico são gravados para uma única atividade do usuário.
localization_priority: Normal
ms.prod: project-rome
author: ailae
doc_type: resourcePageType
ms.openlocfilehash: 7e845158dce7b8b3d0ea74eff673e179cda19b78e74d5a20512ea2c786fa1796
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54246623"
---
# <a name="historyitem-resource-type"></a>Tipo de recurso historyItem

Namespace: microsoft.graph

Representa um item de histórico para [uma atividade](projectrome-activity.md) em um aplicativo. As atividades do usuário representam um único destino em seu aplicativo - por exemplo, um programa de TV, um documento ou uma campanha atual em um jogo de vídeo. Quando um usuário se envolve com essa atividade, o envolvimento é capturado como um item de histórico que indica a hora de início e término dessa atividade. À medida que o usuário se envolve com essa atividade ao longo do tempo, vários itens de histórico são gravados para uma única atividade do usuário.

Quando um aplicativo cria uma sessão, um **objeto historyItem** deve ser adicionado ao objeto **de** atividade para refletir o período de envolvimento do usuário. Sempre que um usuário reaja a uma atividade, um **novo historyItem** é adicionado à atividade para acumular o envolvimento do usuário.

## <a name="methods"></a>Métodos

|Método | Tipo de retorno | Descrição|
|:------|:------------|:-----------|
|[Criar ou substituir historyItem](../api/projectrome-put-historyitem.md) | [historyItem](projectrome-historyitem.md) | Cria ou substitui um **historyItem** existente para essa atividade (upsert). A ID precisa ser um GUID.|
|[Excluir um historyItem](../api/projectrome-delete-historyitem.md) | Sem Conteúdo | Exclui o **historyItem** especificado para essa atividade.|

## <a name="properties"></a>Propriedades

|Nome | Tipo | Descrição|
|:----|:-----|:-----------|
|status | status | Definido pelo servidor. Um código de status usado para identificar objetos válidos. Valores: ativo, atualizado, excluído, ignorado.|
|userTimezone | String | Opcional. O timezone no qual o dispositivo do usuário usado para gerar a atividade estava localizado no momento da criação da atividade. Valores fornecidos como IDs Olson para dar suporte à representação entre plataformas.|
|createdDateTime | DateTimeOffset | Definido pelo servidor. DateTime em UTC quando o objeto foi criado no servidor.|
|lastModifiedDateTime | DateTimeOffset | Definido pelo servidor. DateTime em UTC quando o objeto foi modificado no servidor.|
|id | String | Obrigatório. GUID definido pelo cliente para o **objeto historyItem.**|
|startedDateTime | DateTimeOffset | Obrigatório. UTC DateTime quando **o historyItem** (sessão de atividade) foi iniciado. Obrigatório para o histórico da linha do tempo.|
|lastActiveDateTime | DateTimeOffset | Opcional. UTC DateTime quando **o historyItem** (sessão de atividade) foi entendido pela última vez como ativo ou concluído - se nulo, o status **historyItem** deve ser Contínuo.|
|expirationDateTime | DateTimeOffset | Opcional. UTC DateTime quando **historyItem** passará por exclusão permanente. Pode ser definido pelo cliente.|
|activeDurationSeconds | int | Opcional. A duração do envolvimento do usuário ativo. se não for fornecido, isso é calculado a partir do **startedDateTime** e **lastActiveDateTime**.|

## <a name="relationships"></a>Relações

|Relação | Tipo | Descrição|
|:------------|:-----|:-----------|
|atividade| [userActivity](../resources/projectrome-activity.md) | Opcional. NavigationProperty/Containment; propriedade navigation para a atividade associada.|

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

