---
title: tipo de recurso atividade
description: Representa uma única atividade dentro de um aplicativo, por exemplo, um programa de TV, um documento ou uma campanha atual em um jogo de vídeo. Quando um usuário participa dessa atividade, o contrato é capturado como um item de histórico que indica a hora de início e término da atividade. À medida que o usuário se reencaixa com essa atividade ao longo do tempo, vários itens de histórico são registrados para uma única atividade do usuário.
localization_priority: Normal
ms.prod: project-rome
doc_type: resourcePageType
author: ailae
ms.openlocfilehash: f72a63280df3cb32d7814cd00f28ac457880d67e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026520"
---
# <a name="activity-resource-type"></a>tipo de recurso atividade

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma única atividade dentro de um aplicativo, por exemplo, um programa de TV, um documento ou uma campanha atual em um jogo de vídeo. Quando um usuário participa dessa atividade, o contrato é capturado como um item de [histórico](projectrome-historyitem.md) que indica a hora de início e término da atividade. À medida que o usuário se reencaixa com essa atividade ao longo do tempo, vários itens de histórico são registrados para uma única atividade do usuário.

Você pode usar atividades no Microsoft Graph para permitir que os usuários voltem ao que estavam fazendo em seus aplicativos, em vários dispositivos. As atividades que seu aplicativo cria aparecem em todos os dispositivos do usuário e são expostas aos usuários como links mais detalhados para conteúdo específico no seu aplicativo. Você pode expressar conteúdo específico no seu aplicativo como um destino que é ativado no Windows e acessível em dispositivos iOS e Android por meio de notificações da Cortana.

Como cada aplicativo é diferente, você deve entender a melhor maneira de mapear ações no seu aplicativo para as atividades do usuário que aparecerão na Cortana e na linha do tempo. Por exemplo, os jogos podem criar uma atividade para cada campanha, os aplicativos de criação de documentos podem criar uma atividade para cada documento exclusivo, e os aplicativos de linha de negócios podem criar uma atividade para cada fluxo de trabalho.

Suas atividades de usuário serão incluídas nas experiências do usuário da Cortana e do Windows Timeline, que estão voltadas para aumentar a produtividade e a eficiência dos usuários, ajudando-os a voltar ao conteúdo em que eles trabalharam no passado.

## <a name="methods"></a>Métodos

|Método | Tipo de retorno | Descrição|
|:------|:------------|:-----------|
|[Criar ou substituir atividade](../api/projectrome-put-activity.md) | [atividade](projectrome-activity.md) |Cria ou substitui uma atividade existente (Upsert). O appActivityId precisa ser uma URL segura (todos os caracteres, exceto os caracteres não reservados da RFC 2396, devem ser convertidos em sua representação hexadecimal), mas o appActivityId original não precisa ser URL-seguro. |
|[Excluir uma atividade](../api/projectrome-delete-activity.md) | Sem Conteúdo | Exclui a atividade especificada para esse usuário do seu aplicativo.|
|[Obter atividades](../api/projectrome-get-activities.md) | Conjunto de [atividades](projectrome-activity.md) | Obtém as atividades para seu aplicativo para um determinado usuário.|
|[Obter atividades recentes](../api/projectrome-get-recent-activities.md) | Conjunto de [atividades](projectrome-activity.md) | Obtém as atividades mais recentes para o seu aplicativo para um determinado usuário, classificadas e com base no [historyItems](projectrome-historyitem.md)criado ou atualizado recentemente.|

## <a name="properties"></a>Propriedades

|Nome | Tipo | Descrição|
|:----|:-----|:-----------|
|usertimezone | String | Opcional. O fuso horário em que o dispositivo do usuário usado para gerar a atividade estava localizado no momento da criação da atividade; valores fornecidos como IDs de Olson para oferecer suporte à representação de plataforma cruzada.|
|createdDateTime | DateTimeOffset | Definido pelo servidor. DateTime em UTC quando o objeto foi criado no servidor. |
|lastModifiedDateTime | DateTimeOffset | Definido pelo servidor. DateTime em UTC quando o objeto foi modificado no servidor. |
|id | String | ID gerada pelo servidor usada para o endereçamento de URL.|
|appActivityId | String | Obrigatório. A ID da atividade exclusiva no contexto do aplicativo, fornecido pelo chamador e imutável, daí em diante.|
|activitySourceHost | String | Obrigatório. URL para o domínio que representa o mapeamento de identidade de plataforma cruzada para o aplicativo. O mapeamento é armazenado como um arquivo JSON hospedado no domínio ou configurável por meio do centro de desenvolvimento do Windows. O arquivo JSON é denominado Cross-Platform-app-Identifiers e é hospedado na raiz do domínio HTTPS, seja no domínio de nível superior ou incluir um subdomínio. Por exemplo: https://contoso.com ou https://myapp.contoso.com, mas NÃO https://myapp.contoso.com/somepath. Você deve ter um arquivo exclusivo e domínio (ou subdomínio) por identidade de aplicativo de plataforma cruzada. Por exemplo, um arquivo e domínio separados é necessário para o Word versus o PowerPoint.|
|appDisplayName | String | Opcional. Descrição de texto curto do aplicativo usado para gerar a atividade para uso em casos em que o aplicativo não está instalado no dispositivo local do usuário.|
|activationUrl | String | Obrigatório. URL usada para iniciar a atividade na melhor experiência nativa representada pela appId. Pode iniciar um aplicativo baseado na Web se nenhum aplicativo nativo existir.|
|fallbackUrl | String | Opcional. URL usada para iniciar a atividade em um aplicativo baseado na Web, se disponível.|
|contentUrl | String | Opcional. Usada no evento o conteúdo pode ser renderizado fora de uma experiência de aplicativo nativa ou baseada na Web (por exemplo, um ponteiro para um item em um RSS feed).|
|visualElements| [visualInfo](../resources/projectrome-visualinfo.md) | Obrigatório. O objeto que contém informações para renderizar a atividade no UX.|
|contentInfo | Objeto JSON não digitado | Opcional. Uma parte personalizada da descrição extensível de dados-JSON-LD do conteúdo de acordo com a sintaxe [Schema.org](https://schema.org) .|
|expirationDateTime | DateTimeOffset | Definido pelo servidor. DateTime em UTC quando o objeto expirou no servidor.|
|status | cadeia de caracteres | Definido pelo servidor. Um código de status usado para identificar objetos válidos. Valores: ativo, atualizado, excluído, ignorado.|

## <a name="relationships"></a>Relações

|Relação | Tipo | Descrição|
|:------------|:-----|:-----------|
|historyItems| coleção [historyItem](../resources/projectrome-historyitem.md) | Opcional. NavigationProperty/confinamento; Propriedade Navigation para o historyItems da atividade.|

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
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.activity"
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
    "status": "string",
    "contentInfo": { "@data.type": "microsoft.graph.Json" },
    "visualElements": { "@data.type": "microsoft.graph.visualInfo" },
    "historyItems": [{ "@odata.type": "microsoft.graph.historyItem" }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "activity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


