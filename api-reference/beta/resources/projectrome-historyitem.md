---
title: tipo de recurso historyItem
description: Representa um item de histórico de uma atividade em um aplicativo. As atividades do usuário representam um único destino dentro de seu aplicativo, por exemplo, um programa de TV, um documento ou uma campanha atual em um jogo de vídeo. Quando um usuário participa dessa atividade, o contrato é capturado como um item de histórico que indica a hora de início e término da atividade. À medida que o usuário se reencaixa com essa atividade ao longo do tempo, vários itens de histórico são registrados para uma única atividade do usuário.
localization_priority: Normal
ms.prod: project-rome
doc_type: resourcePageType
author: ''
ms.openlocfilehash: d5d71d36a2a88492c51e06670815ceec323790b7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965590"
---
# <a name="historyitem-resource-type"></a>tipo de recurso historyItem

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um item de histórico de uma [atividade](projectrome-activity.md) em um aplicativo. As atividades do usuário representam um único destino dentro de seu aplicativo, por exemplo, um programa de TV, um documento ou uma campanha atual em um jogo de vídeo. Quando um usuário participa dessa atividade, o contrato é capturado como um item de histórico que indica a hora de início e término da atividade. À medida que o usuário se reencaixa com essa atividade ao longo do tempo, vários itens de histórico são registrados para uma única atividade do usuário.

Quando um aplicativo cria uma sessão, um objeto **historyItem** deve ser adicionado ao objeto **Activity** para refletir o período do contrato do usuário. Cada vez que um usuário reparticipa de uma atividade, um novo **historyItem** é adicionado à atividade para acumular o envolvimento do usuário.

## <a name="methods"></a>Métodos

|Método | Tipo de retorno | Descrição|
|:------|:------------|:-----------|
|[Criar ou substituir historyItem](../api/projectrome-put-historyitem.md) | [historyItem](projectrome-historyitem.md) | Cria ou substitui um **historyItem** existente para aquela atividade (Upsert). A ID precisa ser um GUID.|
|[Excluir um historyItem](../api/projectrome-delete-historyitem.md) | Sem Conteúdo | Exclui o **historyItem** especificado para essa atividade.|

## <a name="properties"></a>Propriedades

|Nome | Tipo | Descrição|
|:----|:-----|:-----------|
|status | cadeia de caracteres | Definido pelo servidor. Um código de status usado para identificar objetos válidos. Valores: ativo, atualizado, excluído, ignorado.|
|usertimezone | String | Opcional. O fuso horário em que o dispositivo do usuário usado para gerar a atividade estava localizado no momento da criação da atividade. Valores fornecidos como IDs de Olson para oferecer suporte à representação de plataforma cruzada.|
|createdDateTime | DateTimeOffset | Definido pelo servidor. DateTime em UTC quando o objeto foi criado no servidor.|
|lastModifiedDateTime | DateTimeOffset | Definido pelo servidor. DateTime em UTC quando o objeto foi modificado no servidor.|
|id | String | Obrigatório. Client-set GUID para o objeto **historyItem** .|
|startedDateTime | DateTimeOffset | Obrigatório. DateTime UTC quando o **historyItem** (sessão de atividade) foi iniciado. Obrigatório para histórico de linha do tempo.|
|lastActiveDateTime | DateTimeOffset | Opcional. DateTime UTC quando o **historyItem** (sessão de atividade) foi compreendido pela última vez como ativo ou concluído-se nulo, o status do **HistoryItem** deve ser contínuo.|
|expirationDateTime | DateTimeOffset | Opcional. DateTime UTC quando o **historyItem** passará pela exclusão permanente. Pode ser definido pelo cliente.|
|activeDurationSeconds | int | Opcional. A duração do contrato de usuário ativo. Se não for fornecido, isso será calculado a partir do **startedDateTime** e do **lastActiveDateTime**.|

## <a name="relationships"></a>Relações

|Relação | Tipo | Descrição|
|:------------|:-----|:-----------|
|atividade| [atividade](../resources/projectrome-activity.md) | Opcional. NavigationProperty/confinamento; Propriedade de navegação para a atividade associada.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "userTimezone",
    "lastActiveDateTime",
    "activeDurationSeconds"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.historyItem"
}-->

```json
{
    "status": "String (EnumType)",
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
<!--
{
  "type": "#page.annotation",
  "description": "historyitem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
