---
title: Fazer chamadas de API usando os SDKs do Microsoft Graph
description: Fornece instruções para criar solicitações HTTP do Microsoft Graph usando SDKs.
localization_priority: Normal
author: DarrelMiller
ms.openlocfilehash: f317b52393378231fb57f2c39c9b9701a9215cf4
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48192881"
---
# <a name="make-api-calls-using-the-microsoft-graph-sdks"></a>Fazer chamadas de API usando os SDKs do Microsoft Graph

As bibliotecas de serviço SDK do Microsoft Graph fornecem uma classe de cliente que você pode usar como o ponto de partida para a criação de todas as solicitações de API. Há dois estilos de classe de cliente: um usa uma interface fluente para criar a solicitação (por exemplo, `client.Users["user-id"].Manager` ) e o outro aceita uma cadeia de caracteres de caminho (por exemplo, `api("/users/user-id/manager")` ). Quando você tem um objeto Request, é possível especificar uma variedade de opções, como filtragem e classificação, e, por fim, você seleciona o tipo de operação que deseja executar.

Há também o [SDK do Microsoft Graph PowerShell](../powershell/get-started.md), que não tem nenhuma classe de cliente. Em vez disso, todas as solicitações são representadas como comandos do PowerShell. Por exemplo, para obter o gerente de um usuário, o comando é `Get-MgUserManager` . Para obter mais informações sobre como localizar comandos para chamadas de API, consulte [navegação no Microsoft Graph PowerShell SDK](../powershell/navigating.md).

## <a name="read-information-from-microsoft-graph"></a>Ler informações do Microsoft Graph

Para ler informações do Microsoft Graph, você precisa primeiro criar um objeto Request e, em seguida, executar o `GET` método na solicitação.

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-read.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-read.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-read.md)]

---

## <a name="use-select-to-control-the-properties-returned"></a>Use $select para controlar as propriedades retornadas

Ao recuperar uma entidade, nem todas as propriedades são recuperadas automaticamente; às vezes, eles precisam ser explicitamente selecionados. Além disso, em alguns cenários, não é necessário retornar o conjunto de propriedades padrão. Selecionar apenas as propriedades necessárias pode melhorar o desempenho da solicitação. Você pode personalizar a solicitação para incluir o `$select` parâmetro de consulta com uma lista de propriedades.

<!-- markdownlint-disable MD024 -->
# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-select.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-select.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-select.md)]

---

## <a name="retrieve-a-list-of-entities"></a>Recuperar uma lista de entidades

A recuperação de uma lista de entidades é semelhante à recuperação de uma única entidade, exceto por várias outras opções de configuração da solicitação. O `$filter` parâmetro de consulta pode ser usado para reduzir o conjunto de resultados apenas às linhas que correspondem à condição fornecida.  O `$orderBy` parâmetro de consulta solicitará que o servidor forneça a lista de entidades classificadas pelas propriedades especificadas.

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-list.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-list.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-list.md)]

---

O objeto retornado ao recuperar uma lista de entidades provavelmente será uma coleção paginável. Para obter detalhes sobre como obter a lista completa de entidades, consulte [paginação por meio de uma coleção](../paging.md).

## <a name="access-an-item-of-a-collection"></a>Acessar um item de uma coleção

Para SDKs que oferecem suporte a um estilo fluente, as coleções de entidades podem ser acessadas usando um índice de matriz. Para SDKs baseados em modelo, é suficiente incorporar o identificador de item no segmento de caminho após a coleção. Para o PowerShell, os identificadores são passados como parâmetros.

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-index.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-index.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-index.md)]

---

## <a name="use-expand-to-access-related-entities"></a>Use $expand para acessar entidades relacionadas

Você pode usar o `$expand` filtro para solicitar uma entidade relacionada, ou uma coleção de entidades, ao mesmo que você solicite a entidade principal.

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-expand.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-expand.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-expand.md)]

---

## <a name="delete-an-entity"></a>Excluir uma entidade

As solicitações Delete são criadas da mesma maneira que as solicitações para recuperar uma entidade, mas usam uma `DELETE` solicitação em vez de um `GET` .

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-delete.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-delete.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-delete.md)]

---

## <a name="make-a-post-request-to-create-a-new-entity"></a>Fazer uma solicitação POST para criar uma nova entidade

Para SDKs que oferecem suporte a um estilo fluente, novos itens podem ser adicionados às coleções com um `Add` método. Para SDKs baseados em modelo, o objeto Request expõe um `post` método. Para o PowerShell, um `New-*` comando disponível que aceita parâmetros que mapeiam a entidade a ser adicionada. A entidade criada é normalmente retornada da chamada.

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-create.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-create.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-create.md)]

---

## <a name="updating-an-existing-entity-with-patch"></a>Atualizando uma entidade existente com PATCH

A maioria das atualizações no Microsoft Graph é realizada usando um `PATCH` método e, portanto, só é necessário incluir as propriedades que você deseja alterar no objeto aprovado.

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-update.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-update.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-update.md)]

---

## <a name="use-http-headers-to-control-request-behavior"></a>Usar cabeçalhos HTTP para controlar o comportamento da solicitação

Você pode usar uma `Header()` função para anexar cabeçalhos personalizados a uma solicitação. Para o PowerShell, a adição de cabeçalhos só é possível com o `Invoke-GraphRequest` método. Vários cenários do Microsoft Graph usam cabeçalhos personalizados para ajustar o comportamento da solicitação.

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-headers.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-headers.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-headers.md)]

---

## <a name="provide-custom-query-parameters"></a>Fornecer parâmetros de consulta personalizados

Para SDKs que oferecem suporte a um estilo fluente, você pode fornecer valores de parâmetro de consulta personalizados usando uma lista de `QueryOptions` objetos. Para SDKs baseados em modelo, os parâmetros são codificados por URL e adicionados à URI de solicitação. Para o PowerShell, os parâmetros de consulta definidos para uma determinada API são expostos como parâmetros para o comando correspondente.

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-queryparams.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-queryparams.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-queryparams.md)]

---
