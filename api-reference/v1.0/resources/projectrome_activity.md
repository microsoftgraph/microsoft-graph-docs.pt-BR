# <a name="activity-resource-type"></a>tipo de recurso de atividade

Representa uma atividade dentro única de um aplicativo - por exemplo, um programa de TV, um documento ou uma campanha em andamento em um videogame. Quando um usuário se envolve com a atividade, o envolvimento é capturado como um [item do histórico](projectrome_historyitem.md) que indica a hora de início e término para a atividade. À medida que o usuário se envolve novamente com essa atividade ao longo do tempo, vários itens do histórico são registrados para cada atividade do usuário.

Você pode usar as atividades no Microsoft Graph para habilitar os usuários a voltarem para o que eles estavam fazendo em seus aplicativos, em vários dispositivos. As atividades que seu aplicativo cria, aparecem nos dispositivos de todos os usuários e são expostas aos usuários como links profundos para conteúdos específicos dentro de seu aplicativo. Você pode expressar o conteúdo específico dentro de seu aplicativo como um destino que é exibido no Windows e acessível em dispositivos iOS e Android por meio de notificações de Cortana.

Como cada aplicativo é diferente, cabe a você a entender a melhor maneira de mapear as ações dentro de seu aplicativo para as atividades do usuário que serão exibidas em Cortana e Timeline. Por exemplo, jogos podem criar uma atividade para cada campanha, aplicativos de criação de documentos podem criar uma atividade para cada documento único e aplicativos de linha de negócios podem criar uma atividade para cada fluxo de trabalho.

Suas atividades de usuário serão exibidas em experiências de usuário do Cortana e do Timeline do Windows, que estão voltados a aumentar a eficiência e a produtividade dos usuários, ajudando-os a voltar ao conteúdo em que eles estavam trabalhando anteriormente.

## <a name="methods"></a>Métodos

|Método | Tipo de retorno | Descrição|
|:------|:------------|:-----------|
|[Criar ou substituir uma atividade](../api/projectrome_put_activity.md) | [atividade](projectrome_activity.md) |Cria ou substitui uma atividade existente (upsert). O appActivityId na URL precisa ser URL-safe (todos os caracteres, com exceção de caracteres não reservados RFC 2396 devem ser convertidos para sua representação hexadecimal), mas o appActivityId original não precisa ser URL-safe. |
|[Excluir uma atividade](../api/projectrome_delete_activity.md) | Nenhum conteúdo | Exclui a atividade especificada para esse usuário do seu aplicativo.|
|[Obter atividades](../api/projectrome_get_activities.md) | Coleção de [atividades](projectrome_activity.md) | Obtém as atividades para seu aplicativo para um determinado usuário.|
|[Obter atividades recentes](../api/projectrome_get_recent_activities.md) | Coleção de [atividades](projectrome_activity.md) | Obtém as atividades mais recentes para o seu aplicativo para um usuário específico, classificadas e baseadas no [historyItems](projectrome_historyitem.md) criado ou atualizado mais recentemente.|

## <a name="properties"></a>Propriedades

|Nome | Tipo | Descrição|
|:----|:-----|:-----------|
|userTimezone | Sequência de caracteres | Opcional. O fuso horário no qual o dispositivo do usuário usado para gerar a atividade foi localizado no momento da criação de atividade; valores fornecidos como Olson IDs para suportar a representação de plataforma cruzada.|
|createdDateTime | DateTimeOffset | Definido pelo servidor. DateTime em UTC quando o objeto foi criado no servidor. |
|lastModifiedDateTime | DateTimeOffset | Definido pelo servidor. DateTime em UTC quando o objeto foi modificado no servidor. |
|id | Sequência de caracteres | ID gerado pelo servidor usado para o endereçamento de URL.|
|appActivityId | Sequência de caracteres | Obrigatório. O ID único de atividade no contexto do aplicativo - fornecido por pessoa que chama e imutável depois disso.|
|activitySourceHost | Sequência de caracteres | Obrigatório. URL para o domínio que representa o mapeamento de identidade de plataforma cruzada para o aplicativo. O mapeamento é armazenado como um arquivo JSON hospedado no domínio ou configurável via Windows Dev Center. O arquivo JSON é chamado plataforma cruzada-aplicativo-identificadores e está hospedado na raiz do seu domínio HTTPS, no domínio de nível superior ou inclui um subdomínio. Por exemplo: https://contoso.com ou https://myapp.contoso.com mas NÃO https://myapp.contoso.com/somepath. Você deve ter um arquivo exclusivo e um domínio (ou subdomínio) por identidade do aplicativo de plataforma cruzada. Por exemplo, um arquivo separado e um domínio é necessário para o Word versus PowerPoint.|
|appDisplayName | Sequência de caracteres | Opcional. Descrição de texto curta do aplicativo usado para gerar a atividade para uso em casos quando o aplicativo não está instalado no dispositivo local do usuário.|
|activationUrl | Sequência de caracteres | Obrigatório. URL usada para iniciar a atividade na melhor experiência nativa representada pelo appId. Pode iniciar um aplicativo baseado na web senão existe um aplicativo nativo.|
|fallbackUrl | Sequência de caracteres | Opcional. URL usada para iniciar a atividade em um aplicativo baseado na web, se disponível.|
|contentUrl | Sequência de caracteres | Opcional. Usado quando o conteúdo pode ser renderizado fora de uma experiência de aplicativo nativo ou baseado na web (por exemplo, um ponteiro para um item em um feed RSS).|
|visualElements| [visualInfo](../resources/projectrome_visualinfo.md) | Obrigatório. O objeto que contém informações para renderizar a atividade na UX.|
|contentInfo | Objeto JSON não digitado | Opcional. Um parte personalizada dos dados - descrição extensível do conteúdo JSON-LD de acordo com a sintaxe [schema.org](http://schema.org).|
|expirationDateTime | DateTimeOffset | Definido pelo servidor. DateTime em UTC quando o objeto expira no servidor.|
|status | status | Definido pelo servidor. Um código de status usado para identificar objetos válidos. Valores: ativo, atualizado, excluídos, ignorado.|

## <a name="relationships"></a>Relações

|Relação | Tipo | Descrição|
|:------------|:-----|:-----------|
|historyItems| coleção [activityHistoryItem](../resources/projectrome_historyitem.md) | Opcional. NavigationProperty/Containment; propriedade de navegação para a atividade historyItems.|

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
