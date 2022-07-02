---
title: Práticas recomendadas para trabalhar com o Microsoft Graph
description: Aplique essas melhores práticas para melhorar o desempenho do seu aplicativo Microsoft Graph e tornar seu aplicativo mais confiável para os usuários finais.
ms.localizationpriority: high
ms.custom: graphiamtop20
ms.openlocfilehash: b2cb4b928db17817bf2543a425adde0827d75008
ms.sourcegitcommit: af9489bd42a25dff04836dcfcc57369259fda587
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2022
ms.locfileid: "66577571"
---
# <a name="best-practices-for-working-with-microsoft-graph"></a>Práticas recomendadas para trabalhar com o Microsoft Graph

Este artigo descreve as melhores práticas que você pode aplicar para ajudar seus aplicativos a tirar o máximo proveito do Microsoft Graph&mdash;, quer isso envolva saber mais sobre o Microsoft Graph, melhorar o desempenho do aplicativo ou tornar seu aplicativo mais confiável para os usuários finais.

## <a name="use-graph-explorer-to-get-to-know-the-api"></a>Usar o Graph Explorer para saber mais sobre a API

A melhor maneira de começar a explorar os dados disponíveis pelo Microsoft Graph é usando o [Graph Explorer](https://aka.ms/ge). O Graph Explorer permite criar solicitações REST (com suporte completo para CRUD), adaptar os cabeçalhos de solicitação HTTP e ver as respostas dos dados. Para ajudar você a começar, o Graph Explorer também oferece um conjunto de consultas de exemplo.

Experimente novas APIs antes de integrá-las em seu aplicativo.

## <a name="authentication"></a>Autenticação

Para acessar dados por meio do Microsoft Graph, seu aplicativo precisará adquirir um token de acesso OAuth 2.0 e apresentá-lo ao Microsoft Graph em uma das seguintes opções:

- O cabeçalho de solicitação HTTP *Authorization*, como um token de *Portador*
- O construtor do cliente gráfico ao usar uma biblioteca de cliente do Microsoft Graph

Use a API da Biblioteca de Autenticação Microsoft, [MSAL](/azure/active-directory/develop/active-directory-v2-libraries), para adquirir o token de acesso para o Microsoft Graph.

## <a name="consent-and-authorization"></a>Consentimento e autorização

Aplique as seguintes práticas recomendadas de consentimento e autorização ao aplicativo:

- **Aplicar privilégios mínimos**. Conceda aos usuários e aplicativos apenas a permissão com privilégios mínimos necessário para chamar a API. Verifique a seção de permissões nos tópicos do método (por exemplo, confira [criando um usuário](/graph/api/user-post-users)) e escolha as permissões com privilégios mínimos. Por exemplo, se o aplicativo ler apenas o perfil do usuário conectado no momento, conceda *User.Read* em vez de *User.ReadBasic.All*. Se um aplicativo não ler o calendário do usuário, não conceda a permissão *Calendars.Read*. Uma ver uma lista completa de permissões, confira [referência de permissões](permissions-reference.md).

- **Use o tipo de permissão correto com base nos cenários**. Evite usar tanto o aplicativo quanto as permissões delegadas no mesmo aplicativo. Se você estiver criando um aplicativo interativo em que um usuário conectado esteja presente, seu aplicativo deverá usar as *permissões delegadas*. Se, no entanto, seu aplicativo for executado sem um usuário conectado, como um serviço ou daemon em segundo plano, seu aplicativo deverá usar as *permissões de aplicativo*.

  > [!CAUTION]
  > O uso de permissões de aplicativo em cenários interativos pode colocar seu aplicativo em risco de conformidade e segurança. Ele pode elevar inadvertidamente os privilégios de um usuário para acessar dados, ignorando as políticas configuradas por um administrador.

- **Esteja atento ao configurar seu aplicativo**. Isso afetará diretamente as experiências do usuário final e do administrador, além da adoção e segurança do aplicativo. Por exemplo:

  - O nome, logotipo, domínio, status de verificação do editor, declaração de privacidade e termos de uso do seu aplicativo aparecerão no consentimento e em outras experiências. Defina essas configurações com cuidado para que sejam compreendidas pelos usuários finais.
  - Leve em consideração quem consentirá com seu aplicativo, seja o usuário final ou administrador, e configure seu aplicativo para [solicitar permissões de forma adequada](/azure/active-directory/develop/active-directory-v2-scopes).
  - Certifique-se de entender a diferença entre [consentimento estático, dinâmico e incremental](/azure/active-directory/develop/v2-permissions-and-consent#consent-types).

- **Considere aplicativos multilocatário**. Tenha em mente que os clientes podem ter vários controles de aplicativo e consentimentos em diferentes estados. Por exemplo:

  - os administradores de locatários podem desabilitar a capacidade dos usuários finais permitirem os aplicativos. Nesse caso, um administrador precisaria consentir em nome de seus usuários.
  - Os administradores de locatários podem definir políticas de autorização personalizadas, como impedir que os usuários leiam perfis de outros usuários ou limitar a criação de grupos de autoatendimento a um conjunto limitado de usuários. Nesse caso, seu aplicativo deve esperar lidar com a resposta de erro `403 Forbidden` ao agir em nome de um usuário.

## <a name="handle-responses-effectively"></a>Controlar as respostas com eficiência

Dependendo das solicitações feitas ao Microsoft Graph, seus aplicativos devem estar preparados para lidar com diferentes tipos de respostas. Veja a seguir algumas das práticas mais importantes a seguir para garantir que seu aplicativo se comporte de maneira confiável e previsível para seus usuários finais.

### <a name="pagination"></a>Paginação

Ao consultar uma coleção de recursos, você deve esperar que o Microsoft Graph retorne o conjunto de resultados em várias páginas, devido aos limites de tamanho da página do lado do servidor. Quando um conjunto de resultados se estende por várias páginas, o Microsoft Graph retorna uma propriedade `@odata.nextLink` na resposta que contém uma URL para a próxima página de resultados.

Por exemplo, listar as mensagens de usuários conectados:

```http
GET https://graph.microsoft.com/v1.0/me/messages
```

retornaria uma resposta contendo uma propriedade `@odata.nextLink`, se o conjunto de resultados exceder o limite de tamanho de página do lado do servidor.

```json
"@odata.nextLink": "https://graph.microsoft.com/v1.0/me/messages?$skip=23"
```

> [!NOTE]
> Seu aplicativo deve **sempre** lidar com a possibilidade das respostas serem paginadas sem processamento e usar a propriedade `@odata.nextLink` para obter o próximo conjunto paginado de resultados, até que todas as páginas do conjunto de resultados sejam lidas. A página final não conterá uma propriedade `@odata.nextLink`. Você deve incluir a URL inteira na propriedade `@odata:nextLink` na solicitação da próxima página de resultados, tratando toda a URL como uma cadeia de caracteres opaca.

Para saber mais, confira [paginação](paging.md).

### <a name="handling-expected-errors"></a>Como tratar erros esperados

Como seu aplicativo tem que lidar com todas as respostas de erro (nos intervalos 400 e 500), dê especial atenção a determinados erros e respostas esperados que estão listados na tabela a seguir.

| Tópico   | Código de erro HTTP    | Prática recomendada|
|:-----------|:--------|:----------|
| O usuário não tem acesso | 403 | Se seu aplicativo estiver em execução, ele poderá encontrar esse erro, mesmo que tenha recebido as permissões necessárias por meio de uma experiência de consentimento.  Nesse caso, é mais provável que o usuário conectado não tenha privilégios para acessar o recurso solicitado. Seu aplicativo deve fornecer um erro genérico de "Acesso negado" para o usuário conectado. |
|Não encontrado| 404 | Em certos casos, um recurso solicitado pode não ser encontrado. Por exemplo, um recurso pode não existir porque ainda não foi provisionado (como a foto de um usuário) ou porque foi excluído. Alguns recursos excluídos *podem* ser totalmente restaurados em até 30 dias após a exclusão, como recursos de usuários, grupos e aplicativos, portanto, o aplicativo também deve levar isso em consideração.|
|Limitação|429|As APIs podem limitar a qualquer momento por diversos motivos, portanto, seu aplicativo deve **sempre** estar preparado para manipular 429 respostas. Essa resposta de erro inclui o campo *Retry-After* no cabeçalho de resposta HTTP. Desativar solicitações usando o atraso *Retry-After* é a forma mais rápida de se recuperar da limitação. Para saber mais, confira [limitação](throttling.md).|
|Serviço indisponível| 503 | O motivo mais provável é que os serviços estejam ocupados. Você deve empregar uma estratégia de retirada similar à 429. Além disso, você deve **sempre** fazer novas solicitações de novas tentativas em uma nova conexão HTTP.|

### <a name="handling-future-members-in-evolvable-enumerations"></a>Manipular futuros membros em enumerações evolutivas

Adicionar membros a enumerações existentes pode interromper aplicativos que já usam essas enumerações. Enumeração evolutiva é um mecanismo que o Microsoft Graph API usa para adicionar novos membros às enumerações existentes sem causar uma mudança radical aos aplicativos.

As enumeração evolutivas possuem um membro chamado _sentinela_ que `unknownFutureValue` demarca membros conhecidos que foram definidos inicialmente na enumeração, e membros desconhecidos que são acrescentados posteriormente ou que serão definidos no futuro. Internamente, os membros conhecidos são mapeados para valores numéricos que são menores que o membro sentinela, e os membros desconhecidos são maiores que o membro sentinela. A documentação de uma enumeração evolutiva lista os possíveis valores de _cadeia de caracteres_ em ordem crescente: membros conhecidos, seguidos por `unknownFutureValue`, seguidos por membros desconhecidos. Como outros tipos de enumerações, você deve _sempre_ fazer referência aos membros de enumeração evolutiva por seus valores de cadeia.de _cadeia de caracteres_.

Por padrão, uma operação GET retorna apenas membros conhecidos por propriedades de tipos de enumeração evolutiva e seu aplicativo precisa lidar apenas com os membros conhecidos. Se você projetar seu aplicativo para também lidar com membros desconhecidos, poderá optar por receber esses membros usando um cabeçalho de solicitação `Prefer` HTTP:
```http
Prefer: include-unknown-enum-members
```


## <a name="storing-data-locally"></a>Armazenamento de dados no local

Idealmente, seu aplicativo deveria fazer chamadas para o Microsoft Graph para recuperar dados em tempo real conforme necessário. Você só deve armazenar em cache ou armazenar dados localmente se um cenário específico assim o exigir e, se esse caso de uso for abrangido pelos seus termos de uso e pela política de privacidade e não violar os [termos de uso das APIs da Microsoft](/legal/microsoft-apis/terms-of-use?context=/graph/context). O aplicativo também deve implementar políticas adequadas de retenção e de exclusão.

## <a name="optimizations"></a>Otimizações

Em geral, por motivos de desempenho e até mesmo segurança ou privacidade, você só deve obter os dados que seu aplicativo realmente precisar e nada mais.

### <a name="use-projections"></a>Usar projeções

Escolha apenas as propriedades que seu aplicativo realmente precisa e nada mais já que isso evitará tráfego de rede e processamento de dados desnecessários em seu aplicativo (e no serviço).

> [!NOTE]
> Use o parâmetro de consulta `$select` para limitar as propriedades devolvidas por uma consulta àquelas exigidas pelo aplicativo.

Por exemplo, ao recuperar as mensagens do usuário conectado, você pode especificar que somente as propriedades **from** e **subject** sejam retornadas:

```http
GET https://graph.microsoft.com/v1.0/me/messages?$select=from,subject
```

### <a name="getting-minimal-responses"></a>Como obter respostas mínimas

Para algumas operações, como PUT e PATCH (e, em alguns casos, POST), se seu aplicativo não precisa usar uma carga de resposta, solicite à API que retorne dados mínimos. Observe que alguns serviços já retornam uma resposta 204 No Content para operações PUT e PATCH.

> [!NOTE]
> Solicitar respostas de representação mínima usando um cabeçalho de solicitação HTTP onde for apropriado: *Prefer: return=minimal*. Observe que, em operações de criação, isso pode não ser adequado já que o aplicativo pode estar esperando receber o serviço gerado `id` para o objeto recém-criado na resposta.

### <a name="track-changes-delta-query-and-webhook-notifications"></a>Controlar alterações: consulta delta e notificações de webhook

Se for preciso que o aplicativo saiba quais alterações foram feitas nos dados, você provavelmente receberá uma notificação de webhook sempre que dados de seu interesse forem alterados. Isso é mais eficiente do que simplesmente fazer pesquisas regularmente.

Use [notificações de webhook](/graph/api/resources/webhooks) para receber notificações por push quando os dados forem alterados.

Use a consulta delta se seu aplicativo tiver que armazenar em cache ou armazenar dados do Microsoft Graph localmente, e mantê-los atualizados, ou tiver que controlar alterações nos dados por qualquer outro motivo. Isso evitará a computação excessiva do aplicativo para recuperar dados que ele já possui, minimizar o tráfego de rede e reduzir a probabilidade de atingir um limite de limitação.

Use a [consulta delta](delta-query-overview.md) para manter os dados atualizados com eficiência.

### <a name="using-webhooks-and-delta-query-together"></a>Usar consultas delta e webhooks em conjunto

Os Webhooks e a consulta delta são geralmente melhor usados juntos, pois se você usa a consulta delta sozinho, você precisa descobrir o intervalo certo da votação - muito curto e isso pode levar a respostas vazias que desperdiçam recursos, muito longas e você pode acabar com dados obsoletos. Se você usar as notificações do Webhook como gatilho para fazer chamadas delta, você obtém o melhor dos dois mundos.

Use as [notificações de webhook](/graph/api/resources/webhooks) como o gatilho para fazer chamadas de consulta delta. Você também deve garantir que seu aplicativo tenha um limite de pesquisa de backstop, caso nenhuma notificação seja acionada.

### <a name="batching"></a>Envio em lote

Os lotes JSON permitem otimizar seu aplicativo combinando várias solicitações em um único objeto JSON. Combinar essas solicitações individuais em uma única solicitação em lote pode economizar latência de rede significativa para o aplicativo e conservar recursos de conexão.

Use o [envio em lote](json-batching.md) onde uma latência de rede significativa pode ter um grande impacto no desempenho.

## <a name="reliability-and-support"></a>Confiabilidade e suporte
Para garantir a segurança e facilitar o suporte do aplicativo:

- Use o TLS 1.2 para dar suporte a todos os recursos do Microsoft Graph. Para obter mais informações sobre a deprecação do Microsoft Graph TLS 1.0 e 1.1, consulte [Habilitar o suporte para TLS 1.2 em seu ambiente](/troubleshoot/azure/active-directory/enable-support-tls-environment).
- Respeite o TTL DNS e defina a conexão TTL para correspondê-lo. Isso garantirá a disponibilidade em caso de failovers.
- Abra conexões para todas as respostas de DNS anunciadas.
- Gerar um GUID exclusivo e o enviar em cada solicitação REST do Microsoft Graph. Isso ajudará a Microsoft a investigar os erros com maior facilidade, caso seja necessário relatar um problema com o Microsoft Graph.
  - Em todas as solicitações do Microsoft Graph, gere um GUID exclusivo, envie-o no cabeçalho de solicitação HTTP do `client-request-id` e também registre-o nos logs dos aplicativos.
  - Registre sempre o `request-id`, o `timestamp` e o `x-ms-ags-diagnostic` dos cabeçalhos de resposta HTTP. Estes, juntamente com o `client-request-id`, são necessários ao relatar problemas em[Microsoft Q&A](/answers/products/m365#microsoft-graph) ou para o Suporte da Microsoft.
