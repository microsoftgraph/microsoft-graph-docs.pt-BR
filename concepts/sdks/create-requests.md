---
title: Fazer chamadas de API usando os SDKs do Microsoft Graph
description: Fornece instruções para criar solicitações HTTP do Microsoft Graph usando SDKs.
localization_priority: Normal
author: DarrelMiller
ms.openlocfilehash: d4fdd5fc6c9a5b2fb0e8acd6d5484176ef179333
ms.sourcegitcommit: d189830649794365464e37539e02239f883011da
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/24/2019
ms.locfileid: "37653514"
---
# <a name="make-api-calls-using-the-microsoft-graph-sdks"></a>Fazer chamadas de API usando os SDKs do Microsoft Graph

As bibliotecas de serviço SDK do Microsoft Graph fornecem uma classe de cliente que você pode usar como o ponto de partida para a criação de todas as solicitações de API. Há dois estilos de classe de cliente: um usa uma interface fluente para criar a solicitação (por exemplo, `client.Me.Manager`) e o outro aceita uma cadeia de caracteres de caminho ( `api("/me/manager")`por exemplo,). Quando você tem um objeto Request, é possível especificar uma variedade de opções, como filtragem e classificação, e, por fim, você seleciona o tipo de operação que deseja executar.

## <a name="read-information-from-microsoft-graph"></a>Ler informações do Microsoft Graph

Para ler informações do Microsoft Graph, você precisa primeiro criar um objeto Request e, em seguida, `GET` executar o método na solicitação.

# <a name="ctabcs"></a>[C#](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-read.md)]
# <a name="typescripttabtypescript"></a>[TypeScript](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-read.md)]
---

## <a name="use-select-to-control-the-properties-returned"></a>Use $select para controlar as propriedades retornadas

Ao recuperar uma entidade, nem todas as propriedades são recuperadas automaticamente; às vezes, eles precisam ser explicitamente selecionados. Além disso, em alguns cenários, não é necessário retornar o conjunto de propriedades padrão. Selecionar apenas as propriedades necessárias pode melhorar o desempenho da solicitação. Você pode personalizar o objeto *Request* para emitir o `$select` parâmetro de consulta com uma lista de propriedades.

# <a name="ctabcs"></a>[C#](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-select.md)]
# <a name="typescripttabtypescript"></a>[TypeScript](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-select.md)]
---


## <a name="retrieve-a-list-of-entities"></a>Recuperar uma lista de entidades

A recuperação de uma lista de entidades é semelhante à recuperação de uma única entidade, exceto por várias outras opções de configuração da solicitação. O `$filter` parâmetro de consulta pode ser usado para reduzir o conjunto de resultados apenas às linhas que correspondem à condição fornecida.  O `$orderBy` parâmetro de consulta solicitará que o servidor forneça a lista de entidades classificadas pelas propriedades especificadas.

# <a name="ctabcs"></a>[C#](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-list.md)]
# <a name="typescripttabtypescript"></a>[TypeScript](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-list.md)]
---

O objeto retornado ao recuperar uma lista de entidades provavelmente será uma coleção paginável. Para obter detalhes sobre como obter a lista completa de entidades, consulte [paginação por meio de uma coleção](../paging.md).

## <a name="access-an-item-of-a-collection"></a>Acessar um item de uma coleção

Para SDKs que oferecem suporte a um estilo fluente, as coleções de entidades podem ser acessadas usando um índice de matriz. Para SDKs baseados em modelo, é suficiente incorporar o identificador de item no segmento de caminho após a coleção.

# <a name="ctabcs"></a>[C#](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-index.md)]
# <a name="typescripttabtypescript"></a>[TypeScript](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-index.md)]
---

## <a name="use-expand-to-access-related-entities"></a>Use $expand para acessar entidades relacionadas

Você pode usar o `$expand` filtro para solicitar uma entidade relacionada, ou uma coleção de entidades, ao mesmo que você solicite a entidade principal.  A `Expand()` função no objeto *Request* adiciona o parâmetro de consulta necessário.

# <a name="ctabcs"></a>[C#](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-expand.md)]
# <a name="typescripttabtypescript"></a>[TypeScript](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-expand.md)]
---


## <a name="delete-an-entity"></a>Excluir uma entidade

Para excluir uma entidade, construa a *solicitação* da mesma maneira que você faz para recuperar uma entidade. O método *delete* no objeto *Request* indica o desejo de excluir a entidade.

# <a name="ctabcs"></a>[C#](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-delete.md)]
# <a name="typescripttabtypescript"></a>[TypeScript](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-delete.md)]
---

## <a name="make-a-post-request-to-create-a-new-entity"></a>Fazer uma solicitação POST para criar uma nova entidade

Para criar uma nova entidade em uma coleção, chame um `add` método `post` or e passe um objeto que contém as informações a serem usadas para criar a nova entidade. Uma versão atualizada da entidade criada normalmente é retornada da chamada.

# <a name="ctabcs"></a>[C#](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-create.md)]
# <a name="typescripttabtypescript"></a>[TypeScript](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-create.md)]
---

## <a name="updating-an-existing-entity-with-patch"></a>Atualizando uma entidade existente com PATCH

A maioria das atualizações no Microsoft Graph é realizada `PATCH` usando um método e, portanto, só é necessário incluir as propriedades que você deseja alterar no objeto aprovado.  

# <a name="ctabcs"></a>[C#](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-update.md)]
# <a name="typescripttabtypescript"></a>[TypeScript](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-update.md)]
---


## <a name="use-http-headers-to-control-request-behavior"></a>Usar cabeçalhos HTTP para controlar o comportamento da solicitação

Você pode usar uma `header()` função para anexar cabeçalhos personalizados a uma solicitação. Vários cenários do Microsoft Graph usam cabeçalhos personalizados para ajustar o comportamento da solicitação.
 
# <a name="ctabcs"></a>[C#](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-headers.md)]
# <a name="typescripttabtypescript"></a>[TypeScript](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-headers.md)]
---

## <a name="provide-custom-query-parameters"></a>Fornecer parâmetros de consulta personalizados

Em situações em que uma chamada de API permite parâmetros de consulta personalizados, você pode fornecer esses valores de parâmetro usando `QueryOptions` uma lista de objetos.

# <a name="ctabcs"></a>[C#](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-queryparams.md)]
# <a name="typescripttabtypescript"></a>[TypeScript](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-queryparams.md)]
---
