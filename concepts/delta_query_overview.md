#  <a name="use-delta-query-to-track-changes-in-microsoft-graph-data-preview"></a>Usar consulta delta para rastrear as alterações nos dados do Microsoft Graph (visualização)

A consulta delta permite que aplicativos localizem entidades recém-criadas, atualizadas ou excluídas sem executar uma leitura completa do recurso de destino com cada solicitação. Os aplicativos do Microsoft Graph podem usar consulta delta para sincronizar, com eficiência, alterações com armazenamento de dados local.

## <a name="use-delta-query-to-track-changes-in-a-resource-collection"></a>Usar solicitação delta para rastrear alterações em um conjunto de recursos

O padrão típico de chamada corresponde ao que segue:

1.  O aplicativo começa chamando uma solicitação GET com a função delta no recurso desejado.
2.  O Microsoft Graph enviará uma resposta que contém o recurso solicitado e um [token de estado](#state-tokens).

     a.  Se uma URL `nextLink` é retornada, existem páginas de dado adicionais a serem recuperadas na sessão. O aplicativo continua fazendo solicitações usando a URL `nextLink` até uma URL `deltaLink` ser incluída na resposta.

     b.  Se uma URL `deltaLink` é retornada, não há mais nenhum dado sobre o estado do recurso a ser retornado. Em solicitações futuras, o aplicativo usa a URL `deltaLink` para inteirar-se das alterações feitas no recurso.
     
3.  Quando o aplicativo precisa saber das alterações no recurso, ele faz uma nova solicitação usando a URL `deltaLink` recebida na etapa 2. Esta solicitação *pode* ser feita imediatamente após concluir a etapa 2 ou quando o aplicativo verifica as alterações.
4.  O Microsoft Graph retorna uma resposta descrevendo alterações no recurso desde a solicitação anterior e em uma URL `nextLink` ou uma URL `deltaLink`.

### <a name="state-tokens"></a>Tokens de estado

Um GET de consulta delta sempre inclui uma URL especificada em um cabeçalho de resposta `nextLink` ou `deltaLink`. A URL `nextLink` inclui um _skipToken_ e uma URL `deltaLink` inclui um _deltaToken_. 

 Esses tokens são completamente opacos para o cliente. Isso é tudo o que você precisa saber sobre eles:

- Cada token reflete o estado e representa um instantâneo do recurso dessa fase do rastreamento de alterações. 
- Esses tokens de estado também codificam e incluem outros parâmetros da consulta (como `$select` se o recurso o aceita) especificados na solicitação de consulta delta inicial, para que você não tenha repeti-los em solicitações de consulta delta subsequentes.
- Ao realizar a consulta delta, você poderá simplesmente copiar e aplicar a URL `nextLink` ou `deltaLink`, assim como é para a próxima chamada de função **delta** sem precisar inspecionar o conteúdo da URL, incluindo seu token de estado.


### <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Se um cliente usa um parâmetro de consulta, ele deve ser especificado na solicitação inicial. O Microsoft Graph codifica automaticamente os parâmetros de especificados nos parâmetros `nextLink` ou `deltaLink` fornecidos na resposta. O aplicativo de chamada só precisa especificar os parâmetros de consulta desejados uma vez antecipados. O Microsoft Graph adiciona os parâmetros especificados automaticamente para todas as solicitações subsequentes.

Para usuários e grupos, existem restrições sobre como usar alguns parâmetros de consulta:

-   Se um `$select` parâmetro de consulta é usado, isso indica que o cliente prefere somente controlar alterações no rastreamento das propriedades ou das relações especificadas na instrução `$select`. Isso significa que se ocorrer uma alteração em uma propriedade que não esteja selecionada, o recurso por meio do qual essa propriedade foi alterada não aparecerá na resposta delta após uma solicitação subsequente.
-   Não há suporte para `$expand`.

## <a name="resource-representation-in-the-delta-query-response"></a>Representação de recurso na resposta da consulta delta

-   Instâncias de um recurso recém-criadas de um recurso para o qual há suporte são representadas na resposta da consulta delta usando sua representação-padrão.

-   Instâncias atualizadas são representadas por seus **id** com *pelo menos* as propriedades que foram atualizadas, mas podem ser incluídas propriedades adicionais.

-   As alterações nos relacionamentos entre os usuários e os grupos são representadas como anotações na representação do recurso padrão. Essas anotações usarão o formato `propertyName@delta`, e aparecerão apenas quando o cliente optar explicitamente por rastrear as alterações no relacionamento usando o parâmetro `$select`.

-   As instâncias removidas são representadas usando apenas sua **id** e um nó `@removed`.  O nó `@removed` pode incluir informações adicionais sobre o porquê de a instância ter sido removida.

> **Observação sobre alteração futura**: Instâncias removidas no momento aparecem com o nó `@removed` no seguinte formato *"@removida": "razão para a remoção"* Entretanto, haverá uma alteração significativa introduzida no futuro. Antes de a consulta delta seja movida da versão /beta para a /v1.0, um objeto será aninhado dentro do nó removido para fornecer mais informações. Por exemplo, *@ removido {motivo: "motivo para remoção"}*. Esse objeto pode ser estendido no futuro para incluir metadados adicionais sobre a remoção.

## <a name="supported-resources"></a>Recursos com suporte

A consulta delta é suportada atualmente no modo de visualização no ponto de extremidade /beta do Microsoft Graph para os seguintes recursos.

| **Coleção de recursos** | **API** |
|:------ | :------ |
| Eventos em um modo de exibição de calendário (intervalo de datas) do calendário principal | função [delta](../api-reference/beta/api/event_delta.md) do recurso [evento](../api-reference/beta/resources/event.md) |
| Grupos | Função [delta](../api-reference/beta/api/group_delta.md) do recurso [group](../api-reference/beta/resources/group.md) |
| Pastas de email | função [delta](../api-reference/beta/api/mailfolder_delta.md) do recurso [mailFolder](../api-reference/beta/resources/mailFolder.md)  |
| Mensagens de uma pasta | função [delta](../api-reference/beta/api/message_delta.md) do recurso [mensagem](../api-reference/beta/resources/message.md)  | 
| Pastas de contatos pessoais | função [delta](../api-reference/beta/api/contactfolder_delta.md) do recurso [contactFolder](../api-reference/beta/resources/contactfolder.md) |
| Contatos pessoais em uma pasta | função [delta](../api-reference/beta/api/contact_delta.md) do recurso [contato](../api-reference/beta/resources/contact.md) |
| Usuários | função [delta](../api-reference/beta/api/user_delta.md) do recurso [usuário](../api-reference/beta/resources/user.md) | 
| Itens de unidade\* | função [delta](../api-reference/beta/api/item_delta.md) do recurso [driveItem](../api-reference/beta/resources/driveItem.md) |


> \*O rastreamento de alterações em unidades e seus filhos já constam na versão 1.0. O padrão de uso é semelhante a outros recursos compatíveis com algumas diferenças secundárias de sintaxe. A consulta delta para unidades será atualizada no futuro para serem consistentes com outros tipos de recursos. Para obter mais detalhes sobre a sintaxe atual, veja: <https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/item_delta>

## <a name="prerequisites"></a>Pré-requisitos

As mesmas [permissões](../authorization/permission_scopes.md) necessárias para ler um recurso específico também são necessárias para executar a consulta delta nesse recurso.

## <a name="known-limitations"></a>Limitações conhecidas

Só há suporte para o controle de alterações nos relacionamentos em usuários e grupos dentro da classe de recursos específicos para os quais as alterações estão sendo controladas. Por exemplo, se um cliente estiver rastreando alterações em *grupos* e tiver selecionado o relacionamento **membros**, ele só receberá atualizações de associação na resposta da consulta delta se esses membros também forem *grupos*. Em outras palavras, o rastreamento de associação a um grupo para os usuários ainda não é suportado. A equipe do Microsoft Graph entende que esse é um cenário de alta prioridade. Há uma atualização prevista março de 2017.

## <a name="delta-query-request-examples"></a>Exemplos de solicitação de consulta delta 

- [Obter as alterações incrementais para os eventos em um modo de exibição de calendário (visualização)](../Concepts/delta_query_events.md)
- [Obter as alterações incrementais para as mensagens em uma pasta (visualização)](./delta_query_messages.md)
- [Obter as alterações incrementais para grupos (visualização)](./delta_query_groups.md)
- [Obter as alterações incrementais para usuários (visualização)](./delta_query_users.md)