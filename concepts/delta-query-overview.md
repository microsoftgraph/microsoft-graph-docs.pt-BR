---
title: Usar a consulta delta para controlar alterações nos dados do Microsoft Graph
description: A consulta delta permite que aplicativos localizem entidades recém-criadas, atualizadas ou excluídas sem executar uma leitura completa do recurso de destino com cada solicitação. Os aplicativos do Microsoft Graph podem usar consulta delta para sincronizar, com eficiência, alterações com armazenamento de dados local.
ms.openlocfilehash: 4732cabed3595738b70c54a7a029f19400edbe6f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091715"
---
# <a name="use-delta-query-to-track-changes-in-microsoft-graph-data"></a>Usar a consulta delta para controlar alterações nos dados do Microsoft Graph

A consulta delta permite que aplicativos localizem entidades recém-criadas, atualizadas ou excluídas sem executar uma leitura completa do recurso de destino com cada solicitação. Os aplicativos do Microsoft Graph podem usar consulta delta para sincronizar, com eficiência, alterações com armazenamento de dados local.

## <a name="use-delta-query-to-track-changes-in-a-resource-collection"></a>Usar solicitação delta para rastrear alterações em uma coleção resource

O padrão típico de chamada corresponde ao que segue:

1. O aplicativo começa chamando uma solicitação GET com a função delta no recurso desejado.
2. O Microsoft Graph envia uma resposta que contém o recurso solicitado e um [token de estado](#state-tokens).

     a.  Se uma URL `nextLink` é retornada, poderá haver páginas de dados adicionais a serem recuperadas na sessão. O aplicativo continua fazendo solicitações usando a URL `nextLink` para recuperar todas as páginas de dados até que uma URL `deltaLink` seja retornada na resposta.

     b.  Se uma URL `deltaLink` é retornada, não há mais nenhum dado sobre o estado do recurso a ser retornado. Em solicitações futuras, o aplicativo usa a URL `deltaLink` para inteirar-se das alterações feitas no recurso.

3. Quando o aplicativo precisa saber das alterações no recurso, ele faz uma nova solicitação usando a URL `deltaLink` recebida na etapa 2. Esta solicitação *pode* ser feita imediatamente após concluir a etapa 2 ou quando o aplicativo verifica as alterações.
4. O Microsoft Graph retorna uma resposta, descrevendo alterações no recurso desde a solicitação anterior e em uma URL `nextLink` ou uma URL `deltaLink`.

>**Observação:** recursos armazenados no Azure Active Directory (por exemplo, usuários e grupos) dão suporte a cenários do tipo "sincronizar a partir de agora". Isso permite que você ignore as etapas 1 e 2 acima (se você não está interessado em recuperar o estado completo do recurso) e peça para conferir o último `deltaLink` em vez disso. Acrescente `$deltaToken=latest` à função `delta`, e a resposta conterá um `deltaLink` e nenhum dado do recurso.

### <a name="state-tokens"></a>Tokens de estado

Um GET de consulta delta sempre inclui uma URL especificada em um cabeçalho de resposta `nextLink` ou `deltaLink`. A URL `nextLink` inclui um _skipToken_ e uma URL `deltaLink` inclui um _deltaToken_.

Esses tokens são opacos para o cliente. Os seguintes detalhes são o que você precisa saber sobre eles:

- Cada token reflete o estado e representa um instantâneo do recurso dessa fase do controle de alterações.

- Os tokens de estado também codificam e incluem outros parâmetros da consulta (como `$select`) especificados na solicitação de consulta delta inicial. Portanto, ele não é necessário repeti-los em solicitações de consulta delta subsequentes.

- Ao realizar a consulta delta, você pode copiar e aplicar a URL `nextLink` ou `deltaLink` à próxima chamada de função **delta** sem precisar inspecionar o conteúdo da URL, incluindo seu token de estado.

### <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Se um cliente usa um parâmetro de consulta, ele deve ser especificado na solicitação inicial. O Microsoft Graph codifica automaticamente o parâmetro especificado nos parâmetros `nextLink` ou `deltaLink` fornecidos na resposta. O aplicativo de chamada só precisa especificar os parâmetros de consulta desejados uma vez antecipados. O Microsoft Graph adiciona os parâmetros especificados automaticamente para todas as solicitações subsequentes.

Para usuários e grupos, existem restrições sobre como usar alguns parâmetros de consulta:

- Se um parâmetro de consulta `$select` for usado, isso indica que o cliente prefere somente controlar alterações nas propriedades ou relações especificadas na instrução `$select`. Se ocorrer uma alteração em uma propriedade que não esteja selecionada, o recurso por meio do qual essa propriedade foi alterada não aparecerá na resposta delta após uma solicitação subsequente.
- `$expand` tem suporte somente para as propriedades de navegação `manager` e `members` para usuários e grupos, respectivamente.

- Os filtros de escopo permitem controlar alterações para um ou mais usuários ou grupos específicos por objectId. Por exemplo, a seguinte solicitação: https://graph.microsoft.com/beta/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ae5f' or id eq '004d6a07-fe70-4b92-add5-e6e37b8acd8e' retorna alterações dos grupos que correspondem às IDs especificadas no filtro de consulta.

## <a name="resource-representation-in-the-delta-query-response"></a>Representação de recurso na resposta da consulta delta

- Instâncias de um recurso recém-criadas de um recurso para o qual há suporte são representadas na resposta da consulta delta usando sua representação-padrão.

- Instâncias atualizadas são representadas por seus **id** com *pelo menos* as propriedades que foram atualizadas, mas podem ser incluídas propriedades adicionais.

- Relações entre os usuários e os grupos são representadas como anotações na representação do recurso padrão. Essas anotações usam o formato `propertyName@delta`. As anotações são incluídas na resposta da solicitação de consulta inicial delta.

As instâncias removidas são representadas por sua **id** e um objeto `@removed`. O objeto `@removed` pode incluir informações adicionais sobre o porquê de a instância ter sido removida. Por exemplo,  "@removed": {"reason": “changed”}.

Possíveis motivos @removed podem ser *changed* ou *deleted*.

- *Alterado* indica que o item foi excluído e poderá ser restaurado de [deletedItems](/graph/api/resources/directory?view=graph-rest-beta).

- *Deleted* indica que o item foi excluído e não pode ser restaurado.

O objeto `@removed` pode ser retornado na resposta de consulta delta inicial e nas respostas rastreadas (deltaLink). Os clientes que usam solicitações de consulta delta devem ser designados para lidar com esses objetos nas respostas.

## <a name="supported-resources"></a>Recursos com suporte

A consulta delta é compatível atualmente com os seguintes recursos.

| **Coleção de recursos** | **API** |
|:------ | :------ |
| Aplicativos (visualização) | Função [delta](/graph/api/application-delta?view=graph-rest-beta) do recurso [application](/graph/api/resources/application?view=graph-rest-beta) (visualização) |
| Objetos de diretório | Função [delta](/graph/api/directoryobject-delta?view=graph-rest-beta) do recurso [directoryObjects](/graph/api/resources/directoryobject?view=graph-rest-beta) (visualização) |
| Funções de diretório | Função [delta](/graph/api/directoryrole-delta?view=graph-rest-1.0) do recurso [directoryRole](/graph/api/resources/directoryrole?view=graph-rest-1.0) |
| Eventos em um modo de exibição de calendário (intervalo de datas) do calendário principal | função [delta](/graph/api/event-delta?view=graph-rest-1.0) do recurso [evento](/graph/api/resources/event?view=graph-rest-1.0) |
| Grupos | Função [delta](/graph/api/group-delta?view=graph-rest-1.0) do recurso [group](/graph/api/resources/group?view=graph-rest-1.0) |
| Pastas de email | função [delta](/graph/api/mailfolder-delta?view=graph-rest-1.0) do recurso [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0)  |
| Mensagens de uma pasta | função [delta](/graph/api/message-delta?view=graph-rest-1.0) do recurso [mensagem](/graph/api/resources/message?view=graph-rest-1.0)  |
| Pastas de contatos pessoais | função [delta](/graph/api/contactfolder-delta?view=graph-rest-1.0) do recurso [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-1.0) |
| Contatos pessoais em uma pasta | Função [delta](/graph/api/contact-delta?view=graph-rest-1.0) do recurso [contato](/graph/api/resources/contact?view=graph-rest-1.0) |
| Entidades de serviço (visualização) | Função [delta](/graph/api/serviceprincipal-delta?view=graph-rest-beta) do recurso [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta) (visualização) |
| Usuários | função [delta](/graph/api/user-delta?view=graph-rest-1.0) do recurso [usuário](/graph/api/resources/user?view=graph-rest-1.0) |
| Itens de unidade\* | Função [delta](/graph/api/driveitem-delta?view=graph-rest-1.0) do recurso [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0) |
| Itens do Planner\*\* | Função [delta](/graph/api/planneruser-list-delta?view=graph-rest-beta) de todos os segmentos do recurso [plannerUser](/graph/api/resources/planneruser?view=graph-rest-beta) (visualização) |

> \* O padrão de uso dos recursos do OneDrive é semelhante a outros recursos compatíveis com algumas diferenças secundárias de sintaxe. A consulta delta para unidades será atualizada no futuro para serem consistentes com outros tipos de recursos. Confira mais detalhes sobre a sintaxe atual em [Controlar alterações para uma unidade](/graph/api/item-delta?view=graph-rest-1.0).

> \*\* O padrão de uso dos recursos do Planner é semelhante a outros recursos compatíveis, mas com algumas diferenças.  Para saber mais, consulte [Controlar alterações para o Planner](/graph/api/planneruser-list-delta?view=graph-rest-beta).

## <a name="prerequisites"></a>Pré-requisitos

As mesmas [permissões](./permissions-reference.md) necessárias para ler um recurso específico também são necessárias para executar a consulta delta nesse recurso.

## <a name="delta-query-request-examples"></a>Exemplos de solicitação de consulta delta

- [Obter as alterações incrementais para os eventos em um modo de exibição de calendário](delta-query-events.md)
- [Obter as alterações incrementais para as mensagens em uma pasta](./delta-query-messages.md)
- [Obter as alterações incrementais para grupos](./delta-query-groups.md)
- [Obter as alterações incrementais para usuários](./delta-query-users.md)
