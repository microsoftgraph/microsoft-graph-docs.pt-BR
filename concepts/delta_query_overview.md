#  <a name="use-delta-query-to-track-changes-in-microsoft-graph-data"></a>Usar a consulta delta para controlar alterações nos dados do Microsoft Graph

A consulta delta permite que aplicativos localizem entidades recém-criadas, atualizadas ou excluídas sem executar uma leitura completa do recurso de destino com cada solicitação. Os aplicativos do Microsoft Graph podem usar consulta delta para sincronizar, com eficiência, alterações com armazenamento de dados local.

## <a name="use-delta-query-to-track-changes-in-a-resource-collection"></a>Usar solicitação delta para rastrear alterações em uma coleção resource

O padrão típico de chamada corresponde ao que segue:

1.  O aplicativo começa chamando uma solicitação GET com a função delta no recurso desejado.
2.  O Microsoft Graph envia uma resposta que contém o recurso solicitado e um [token de estado](#state-tokens).

     a.  Se uma URL `nextLink` é retornada, poderá haver páginas de dados adicionais a serem recuperadas na sessão. O aplicativo continua fazendo solicitações usando a URL `nextLink` para recuperar todas as páginas de dados até que uma URL `deltaLink` seja retornada na resposta.

     b.  Se uma URL `deltaLink` é retornada, não há mais nenhum dado sobre o estado do recurso a ser retornado. Em solicitações futuras, o aplicativo usa a URL `deltaLink` para inteirar-se das alterações feitas no recurso.
     
3.  Quando o aplicativo precisa saber das alterações no recurso, ele faz uma nova solicitação usando a URL `deltaLink` recebida na etapa 2. Esta solicitação *pode* ser feita imediatamente após concluir a etapa 2 ou quando o aplicativo verifica as alterações.
4.  O Microsoft Graph retorna uma resposta descrevendo alterações no recurso desde a solicitação anterior e em uma URL `nextLink` ou uma URL `deltaLink`.

### <a name="state-tokens"></a>Tokens de estado

Um GET de consulta delta sempre inclui uma URL especificada em um cabeçalho de resposta `nextLink` ou `deltaLink`. A URL `nextLink` inclui um _skipToken_ e uma URL `deltaLink` inclui um _deltaToken_. 

Esses tokens são opacos para o cliente. Os seguintes detalhes são o que você precisa saber sobre eles:

- Cada token reflete o estado e representa um instantâneo do recurso dessa fase do rastreamento de alterações. 
- Os tokens de estado também codificam e incluem outros parâmetros da consulta (como `$select`) especificados na solicitação de consulta delta inicial. Portanto, ele não é necessário repeti-los em solicitações de consulta delta subsequentes.
- Ao realizar a consulta delta, você pode copiar e aplicar a URL `nextLink` ou `deltaLink` à próxima chamada de função **delta** sem precisar inspecionar o conteúdo da URL, incluindo seu token de estado.


### <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Se um cliente usa um parâmetro de consulta, ele deve ser especificado na solicitação inicial. O Microsoft Graph codifica automaticamente o parâmetro especificado nos parâmetros `nextLink` ou `deltaLink` fornecidos na resposta. O aplicativo de chamada só precisa especificar os parâmetros de consulta desejados uma vez antecipados. O Microsoft Graph adiciona os parâmetros especificados automaticamente para todas as solicitações subsequentes.

Para usuários e grupos, existem restrições sobre como usar alguns parâmetros de consulta:

-   Se um parâmetro de consulta `$select` for usado, isso indica que o cliente prefere somente controlar alterações nas propriedades ou relações especificadas na instrução `$select`. Se ocorrer uma alteração em uma propriedade que não esteja selecionada, o recurso por meio do qual essa propriedade foi alterada não aparecerá na resposta delta após uma solicitação subsequente.
-   Não há suporte para `$expand`.

Nas APIs de usuários e grupos beta (prévia), os filtros de escopo permitem controlar alterações para um ou mais usuários ou grupos específicos por objectId. Por exemplo, a seguinte solicitação: https://graph.microsoft.com/beta/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ae5f' or id eq '004d6a07-fe70-4b92-add5-e6e37b8acd8e' retorna alterações dos grupos que correspondem às IDs especificadas no filtro de consulta. 

## <a name="resource-representation-in-the-delta-query-response"></a>Representação de recurso na resposta da consulta delta

-   Instâncias de um recurso recém-criadas de um recurso para o qual há suporte são representadas na resposta da consulta delta usando sua representação-padrão.

-   Instâncias atualizadas são representadas por seus **id** com *pelo menos* as propriedades que foram atualizadas, mas podem ser incluídas propriedades adicionais.

-   Relações entre os usuários e os grupos são representadas como anotações na representação do recurso padrão. Essas anotações usam o formato `propertyName@delta`. As anotações são incluídas na resposta da solicitação de consulta inicial delta.

As instâncias removidas são representadas por sua **id** e um objeto `@removed`. O objeto `@removed` pode incluir informações adicionais sobre o porquê de a instância ter sido removida. Por exemplo,  "@removed": {"reason": “changed”}.

Possíveis motivos @removed podem ser *changed* ou *deleted*.
- *Alterado* indica que o item foi excluído e poderá ser restaurado de [deletedItems](../api-reference/beta/resources/directory.md).
- *Deleted* indica que o item foi excluído e não pode ser restaurado.

O objeto @removed pode ser retornado na resposta da consulta delta inicial e em respostas controladas (deltaLink). Os clientes que usam solicitações de consulta delta devem ser projetados para lidar com esses objetos nas respostas.

## <a name="supported-resources"></a>Recursos com suporte

A consulta Delta é compatível atualmente com os seguintes recursos:

| **Coleção de recursos** | **API** |
|:------ | :------ |
| Eventos em um modo de exibição de calendário (intervalo de datas) do calendário principal | função [delta](../api-reference/v1.0/api/event_delta.md) do recurso [evento](../api-reference/v1.0/resources/event.md) |
| Grupos | Função [delta](../api-reference/v1.0/api/group_delta.md) do recurso [group](../api-reference/v1.0/resources/group.md) |
| Pastas de email | função [delta](../api-reference/v1.0/api/mailfolder_delta.md) do recurso [mailFolder](../api-reference/v1.0/resources/mailFolder.md)  |
| Mensagens de uma pasta | função [delta](../api-reference/v1.0/api/message_delta.md) do recurso [mensagem](../api-reference/v1.0/resources/message.md)  | 
| Pastas de contatos pessoais | função [delta](../api-reference/v1.0/api/contactfolder_delta.md) do recurso [contactFolder](../api-reference/v1.0/resources/contactfolder.md) |
| Contatos pessoais em uma pasta | função [delta](../api-reference/v1.0/api/contact_delta.md) do recurso [contato](../api-reference/v1.0/resources/contact.md) |
| Usuários | função [delta](../api-reference/v1.0/api/user_delta.md) do recurso [usuário](../api-reference/v1.0/resources/user.md) | 
| Itens de unidade\* | Função [delta](../api-reference/v1.0/api/item_delta.md) do recurso [driveItem](../api-reference/v1.0/resources/driveItem.md) |


> \* O padrão de uso dos recursos do OneDrive é semelhante a outros recursos compatíveis com algumas diferenças secundárias de sintaxe. A consulta delta para unidades será atualizada no futuro para serem consistentes com outros tipos de recursos. Para obter mais detalhes sobre a sintaxe atual, veja: <https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/item_delta>

## <a name="prerequisites"></a>Pré-requisitos

As mesmas [permissões](./permissions_reference.md) necessárias para ler um recurso específico também são necessárias para executar a consulta delta nesse recurso.

## <a name="delta-query-request-examples"></a>Exemplos de solicitação de consulta delta 

- [Obter as alterações incrementais para os eventos em um modo de exibição de calendário](../Concepts/delta_query_events.md)
- [Obtenha alterações incrementais para as mensagens em uma pasta](./delta_query_messages.md)
- [Obter as alterações incrementais para grupos](./delta_query_groups.md)
- [Obter as alterações incrementais para usuários](./delta_query_users.md)