---
title: tipo de recurso de atividade
description: Representa uma única atividade dentro de um aplicativo - por exemplo, um programa de TV, um documento ou uma campanha atual em um jogo de vídeo. Quando um usuário se envolve com essa atividade, o envolvimento é capturado como um item de histórico que indica a hora de início e término dessa atividade. À medida que o usuário se envolve com essa atividade ao longo do tempo, vários itens de histórico são gravados para uma única atividade do usuário.
ms.localizationpriority: medium
ms.prod: project-rome
author: ailae
doc_type: resourcePageType
ms.openlocfilehash: 06dfcd951826e65fc8c781b84156d89e542df370
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59028790"
---
# <a name="activity-resource-type"></a>tipo de recurso de atividade

Namespace: microsoft.graph

Representa uma única atividade dentro de um aplicativo - por exemplo, um programa de TV, um documento ou uma campanha atual em um jogo de vídeo. Quando um usuário se envolve com essa atividade, o envolvimento é capturado como um [item](projectrome-historyitem.md) de histórico que indica a hora de início e término dessa atividade. À medida que o usuário se envolve com essa atividade ao longo do tempo, vários itens de histórico são gravados para uma única atividade do usuário.

Você pode usar atividades no Microsoft Graph para permitir que os usuários possam voltar ao que estavam fazendo em seu aplicativo, em vários dispositivos. As atividades que seu aplicativo cria aparecem em todos os dispositivos dos usuários e são expostas aos usuários como links profundos para conteúdo específico em seu aplicativo. Você pode expressar conteúdo específico em seu aplicativo como um destino exibido no Windows e acessível em dispositivos iOS e Android por meio de notificações Cortana.

Como cada aplicativo é diferente, você deve entender a melhor maneira de mapear as ações dentro do aplicativo para as atividades do usuário que aparecerão no Cortana e linha do tempo. Por exemplo, os jogos podem criar uma atividade para cada campanha, os aplicativos de criação de documentos podem criar uma atividade para cada documento exclusivo e aplicativos de linha de negócios podem criar uma atividade para cada fluxo de trabalho.

Suas atividades do usuário serão exibidas em experiências de usuário do Cortana e Windows Linha do Tempo, que são focadas em aumentar a produtividade e a eficiência dos usuários, ajudando-os a voltar ao conteúdo em que trabalharam no passado.

## <a name="methods"></a>Métodos

|Método | Tipo de retorno | Descrição|
|:------|:------------|:-----------|
|[Criar ou substituir atividade](../api/projectrome-put-activity.md) | [atividade](projectrome-activity.md) |Cria ou substitui uma atividade existente (upsert). O appActivityId precisa ser seguro para URL (todos os caracteres, exceto os caracteres não reservados RFC 2396, devem ser convertidos em sua representação hexadecimal), mas o appActivityId original não precisa ser seguro para URL. |
|[Excluir uma atividade](../api/projectrome-delete-activity.md) | Sem Conteúdo | Exclui a atividade especificada para esse usuário do seu aplicativo.|
|[Obter atividades](../api/projectrome-get-activities.md) | Coleção de [atividades](projectrome-activity.md) | Obtém as atividades de seu aplicativo para um determinado usuário.|
|[Obter atividades recentes](../api/projectrome-get-recent-activities.md) | Coleção de [atividades](projectrome-activity.md) | Obtém as atividades mais recentes para seu aplicativo para um determinado usuário, organizado e com base no [historyItems](projectrome-historyitem.md)criado ou atualizado mais recentemente.|

## <a name="properties"></a>Propriedades

|Nome | Tipo | Descrição|
|:----|:-----|:-----------|
|userTimezone | String | Opcional. O timezone no qual o dispositivo do usuário usado para gerar a atividade estava localizado no momento da criação da atividade; valores fornecidos como IDs Olson para dar suporte à representação entre plataformas.|
|createdDateTime | DateTimeOffset | Definido pelo servidor. DateTime em UTC quando o objeto foi criado no servidor. |
|lastModifiedDateTime | DateTimeOffset | Definido pelo servidor. DateTime em UTC quando o objeto foi modificado no servidor. |
|id | String | ID gerada pelo servidor usada para endereçamento de URL.|
|appActivityId | Cadeia de caracteres | Obrigatório. A ID de atividade exclusiva no contexto do aplicativo - fornecida pelo chamador e imutável posteriormente.|
|activitySourceHost | String | Obrigatório. URL do domínio que representa o mapeamento de identidade entre plataformas para o aplicativo. O mapeamento é armazenado como um arquivo JSON hospedado no domínio ou configurável por meio Windows Centro de Desenvolvimento. O arquivo JSON é chamado de identificadores entre plataformas e aplicativos e é hospedado na raiz do seu domínio HTTPS, no domínio de nível superior ou inclui um sub domínio. Por exemplo: https://contoso.com ou https://myapp.contoso.com, mas NÃO https://myapp.contoso.com/somepath. Você deve ter um arquivo exclusivo e domínio (ou sub domínio) por identidade de aplicativo entre plataformas. Por exemplo, um arquivo e domínio separados são necessários para Word vs. PowerPoint.|
|appDisplayName | String | Opcional. Breve descrição de texto do aplicativo usado para gerar a atividade para uso nos casos em que o aplicativo não está instalado no dispositivo local do usuário.|
|activationUrl | String | Obrigatório. URL usada para iniciar a atividade na melhor experiência nativa representada pela appId. Pode iniciar um aplicativo baseado na Web se nenhum aplicativo nativo existir.|
|fallbackUrl | String | Opcional. URL usada para iniciar a atividade em um aplicativo baseado na Web, se disponível.|
|contentUrl | String | Opcional. Usado no caso de o conteúdo poder ser renderizado fora de uma experiência de aplicativo nativa ou baseada na Web (por exemplo, um ponteiro para um item em um feed RSS).|
|visualElements| [visualInfo](../resources/projectrome-visualinfo.md) | Obrigatório. O objeto que contém informações para renderizar a atividade no UX.|
|contentInfo | Objeto JSON sem tipo | Opcional. Uma parte personalizada de dados - Descrição extensível JSON-LD do conteúdo de acordo [com schema.org](https://schema.org) sintaxe.|
|expirationDateTime | DateTimeOffset | Definido pelo servidor. DateTime em UTC quando o objeto expirou no servidor.|
|status | status | Definido pelo servidor. Um código de status usado para identificar objetos válidos. Valores: ativo, atualizado, excluído, ignorado.|

## <a name="relationships"></a>Relações

|Relação | Tipo | Descrição|
|:------------|:-----|:-----------|
|historyItems| [Coleção activityHistoryItem](../resources/projectrome-historyitem.md) | Opcional. NavigationProperty/Containment; propriedade navigation para historyItems da atividade.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "userTimezone",
    "appDisplayName",
    "fallbackUrl",
    "contentUrl",
    "contentInfo",
    "visualElements",
    "historyItems"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.userActivity",
  "@odata.annotations": [
    {
      "capabilities": {
        "countable": false,
        "selectable": false,
        "skippable": false
      }
    }
  ]
}-->

```json
{
    "appActivityId": "String",
    "activitySourceHost": "String (host name/domain/URL)",
    "userTimezone": "String",
    "appDisplayName": "String",
    "activationUrl": "String (URL)",
    "contentUrl": "String (URL)",
    "fallbackUrl": "String (URL)",
    "createdDateTime": "DateTimeOffset",
    "lastModifiedDateTime": "DateTimeOffset",
    "expirationDateTime": "DateTimeOffset",
    "id": "String",
    "status": "active | updated | deleted | ignored",
    "contentInfo": { "@odata.type": "microsoft.graph.Json" },
    "visualElements": { "@odata.type": "microsoft.graph.visualInfo" },
    "historyItems": [{ "@odata.type": "microsoft.graph.activityHistoryItem" }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "activity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

