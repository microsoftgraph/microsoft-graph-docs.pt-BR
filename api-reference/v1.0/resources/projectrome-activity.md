---
title: tipo de recurso de atividade
description: Representa uma única atividade dentro de um aplicativo - por exemplo, um programa de TV, um documento ou uma campanha atual em um jogo de vídeo. Quando um usuário emprega com que a atividade, o compromisso é capturado como um item de histórico que indica a hora de início e término para a atividade. À medida que o usuário emprega novamente com que a atividade ao longo do tempo, vários itens de histórico são registrados para atividade de um único usuário.
localization_priority: Normal
ms.openlocfilehash: 79ed44ef0f6a38fbef8ead233debce3fc9e66b42
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877067"
---
# <a name="activity-resource-type"></a>tipo de recurso de atividade

Representa uma única atividade dentro de um aplicativo - por exemplo, um programa de TV, um documento ou uma campanha atual em um jogo de vídeo. Quando um usuário emprega com que a atividade, o compromisso é capturado como um [item de histórico](projectrome-historyitem.md) que indica a hora de início e término para a atividade. À medida que o usuário emprega novamente com que a atividade ao longo do tempo, vários itens de histórico são registrados para atividade de um único usuário.

Você pode usar as atividades no Microsoft Graph para habilitar usuários voltar para o que eles foram fazendo em seus aplicativos, em vários dispositivos. Atividades que seu aplicativo cria aparecem em dispositivos de todos os usuários e são expostas a usuários como links profundos a conteúdos específicos dentro de seu aplicativo. Você pode expressar o conteúdo específico dentro de seu aplicativo como um destino que é exibido no Windows e acessível no iOS e dispositivos com Android por meio de notificações de Cortana.

Como cada aplicativo é diferente, cabe a você a entender a melhor maneira de mapear ações dentro de seu aplicativo para as atividades do usuário será exibida na linha de tempo e Cortana. Por exemplo, jogos puderem criar uma atividade para cada campanha, documentos de criação de aplicativos podem criar uma atividade para cada documento exclusivo e aplicativos de linha de negócios podem criar uma atividade para cada fluxo de trabalho.

Suas atividades do usuário serão exibidas em experiências do usuário Cortana e a linha do tempo do Windows, que são voltadas para aumentar a eficiência e produtividade dos usuários, ajudando-os voltar ao conteúdo que eles trabalhadas no passado.

## <a name="methods"></a>Métodos

|Método | Tipo de retorno | Descrição|
|:------|:------------|:-----------|
|[Criar ou substituir atividade](../api/projectrome-put-activity.md) | [atividade](projectrome-activity.md) |Cria ou substitui uma atividade existente (upsert). O appActivityId deve ser um URL-safe (todos os caracteres, com exceção do RFC 2396 caracteres não reservadas devem ser convertidos em sua representação hexadecimal), mas o appActivityId original não precisa ser URL-safe. |
|[Excluir uma atividade](../api/projectrome-delete-activity.md) | Nenhum conteúdo | Exclui a atividade especificada para o usuário de seu aplicativo.|
|[Obter atividades](../api/projectrome-get-activities.md) | Coleção de [atividades](projectrome-activity.md) | Obtém as atividades para seu aplicativo para um determinado usuário.|
|[Obter atividades recentes](../api/projectrome-get-recent-activities.md) | Coleção de [atividades](projectrome-activity.md) | Obtém as atividades mais recentes para o seu aplicativo para um usuário específico, classificados e com base no [historyItems](projectrome-historyitem.md)mais recentemente criada ou atualizada.|

## <a name="properties"></a>Propriedades

|Nome | Tipo | Descrição|
|:----|:-----|:-----------|
|userTimezone | Cadeia de caracteres | Opcional. O fuso horário no qual o dispositivo do usuário usado para gerar a atividade foi localizado no momento da criação de atividade; valores fornecidos como Olson IDs para suportar a representação de plataforma cruzada.|
|createdDateTime | DateTimeOffset | Definido pelo servidor. Data e hora em UTC quando o objeto foi criado no servidor. |
|lastModifiedDateTime | DateTimeOffset | Definido pelo servidor. Data e hora em UTC quando o objeto foi modificado no servidor. |
|id | Cadeia de caracteres | ID gerados pelo servidor usado para o endereçamento de URL.|
|appActivityId | Cadeia de caracteres | Obrigatório. A ID de atividade exclusivo no contexto do app - fornecido pelo chamador e imutável depois disso.|
|activitySourceHost | Cadeia de caracteres | Obrigatório. URL para o domínio que representa o mapeamento de identidade de plataforma cruzada para o aplicativo. Mapeamento é armazenado como um arquivo JSON hospedado no domínio ou configurável via Windows Dev Center. O arquivo JSON é chamado cross-plataforma-app-identificadores e está hospedado em raiz do seu domínio HTTPS, seja em que o domínio de nível superior ou incluir um domínio sub. Por exemplo: https://contoso.com ou https://myapp.contoso.com, mas NÃO https://myapp.contoso.com/somepath. Você deve ter um arquivo exclusivo e domínio (ou domínio sub) por identidade do aplicativo de plataforma cruzada. Por exemplo, um arquivo separado e o domínio é necessária para o Word versus PowerPoint.|
|appDisplayName | Cadeia de caracteres | Opcional. Descrição de texto curtas do aplicativo usado para gerar a atividade para uso em casos, quando o aplicativo não está instalado no dispositivo de local do usuário.|
|activationUrl | Cadeia de caracteres | Obrigatório. URL usada para iniciar a atividade na melhor experiência de nativa representada por appId. Pode iniciar um aplicativo baseado na web, não se existir nenhum aplicativo nativo.|
|fallbackUrl | Cadeia de caracteres | Opcional. URL usada para iniciar a atividade em um aplicativo baseado na web, se disponível.|
|contentUrl | String | Opcional. Usado no caso do conteúdo pode ser renderizado fora de uma experiência de aplicativo nativo ou baseado na web (por exemplo, um ponteiro para um item em um RSS feed).|
|visualElements| [visualInfo](../resources/projectrome-visualinfo.md) | Obrigatório. O objeto que contém informações para renderizar a atividade na UX.|
|contentInfo | Objeto sem JSON | Opcional. Um parte personalizada de dados - descrição extensível de longa distância o JSON do conteúdo de acordo com a sintaxe [schema.org](https://schema.org) .|
|expirationDateTime | DateTimeOffset | Definido pelo servidor. Data e hora em UTC quando o objeto expira no servidor.|
|status | status | Definido pelo servidor. Um código de status usado para identificar objetos válidos. Valores: ativo, atualizado, excluídos, ignorado.|

## <a name="relationships"></a>Relações

|Relação | Tipo | Descrição|
|:------------|:-----|:-----------|
|historyItems| coleção [activityHistoryItem](../resources/projectrome-historyitem.md) | Opcional. NavigationProperty/contenção; propriedade de navegação historyItems da atividade.|

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
