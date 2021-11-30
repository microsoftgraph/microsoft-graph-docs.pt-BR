---
title: Fazer chamadas de API usando o Microsoft Graph SDKs
description: Fornece instruções para criar solicitações HTTP Graph Microsoft usando os SDKs.
ms.localizationpriority: medium
author: DarrelMiller
ms.openlocfilehash: d2d7b1f1a19c1a0a890bab6ab6a8c51ba7ec47a0
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61226348"
---
<!-- markdownlint-disable MD025 -->

# <a name="make-api-calls-using-the-microsoft-graph-sdks"></a>Fazer chamadas de API usando o Microsoft Graph SDKs

As bibliotecas de serviços do Microsoft Graph SDK fornecem uma classe de cliente que você pode usar como ponto de partida para criar todas as solicitações de API. Há dois estilos de classe de cliente: um usa uma interface fluente para criar a solicitação (por exemplo) e o outro aceita uma cadeia de `client.Users["user-id"].Manager` caracteres de caminho (por exemplo, `api("/users/user-id/manager")` ). Quando você tem um objeto request, você pode especificar uma variedade de opções, como filtragem e classificação, e, por fim, você seleciona o tipo de operação que deseja executar.

Há também o [Microsoft Graph PowerShell SDK](../powershell/get-started.md), que não tem classe de cliente. Em vez disso, todas as solicitações são representadas como comandos do PowerShell. Por exemplo, para obter o gerente de um usuário, o comando é `Get-MgUserManager` . Para obter mais informações sobre como localizar comandos para chamadas de API, consulte [Navegando o SDK](../powershell/navigating.md)do Microsoft Graph PowerShell .

## <a name="read-information-from-microsoft-graph"></a>Ler informações do Microsoft Graph

Para ler informações do Microsoft Graph, primeiro você precisa criar um objeto de solicitação e, em seguida, executar o `GET` método na solicitação.

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-read.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-read.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-read.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-read.md)]

# <a name="go"></a>[Ir](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

[!INCLUDE [sample-code](includes/snippets/go/create-requests-read.md)]

---

## <a name="use-select-to-control-the-properties-returned"></a>Use $select para controlar as propriedades retornadas

Ao recuperar uma entidade, nem todas as propriedades são recuperadas automaticamente; às vezes, eles precisam ser explicitamente selecionados. Além disso, em alguns cenários, não é necessário retornar o conjunto padrão de propriedades. Selecionar apenas as propriedades necessárias pode melhorar o desempenho da solicitação. Você pode personalizar a solicitação para incluir o `$select` parâmetro de consulta com uma lista de propriedades.

<!-- markdownlint-disable MD024 -->
# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-select.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-select.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-select.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-select.md)]

# <a name="go"></a>[Ir](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

[!INCLUDE [sample-code](includes/snippets/go/create-requests-select.md)]

---

## <a name="retrieve-a-list-of-entities"></a>Recuperar uma lista de entidades

Recuperar uma lista de entidades é semelhante à recuperação de uma única entidade, exceto que há várias outras opções para configurar a solicitação. O parâmetro de consulta pode ser usado para reduzir o conjunto de resultados apenas para as linhas que `$filter` corresponderem à condição fornecida.  O parâmetro de consulta solicitará que o servidor forneça a lista de entidades `$orderBy` classificação pelas propriedades especificadas.

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-list.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-list.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-list.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-list.md)]

# <a name="go"></a>[Ir](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

[!INCLUDE [sample-code](includes/snippets/go/create-requests-list.md)]

---

O objeto retornado ao recuperar uma lista de entidades provavelmente será uma coleção de páginas. Para obter detalhes sobre como obter a lista completa de entidades, consulte [paging through a collection](../paging.md).

## <a name="access-an-item-of-a-collection"></a>Acessar um item de uma coleção

Para SDKs que suportam um estilo fluente, coleções de entidades podem ser acessadas usando um índice de matriz. Para SDKs baseados em modelo, é suficiente inserir o identificador de item no segmento de caminho após a coleção. Para o PowerShell, os identificadores são passados como parâmetros.

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-index.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-index.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-index.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-index.md)]

# <a name="go"></a>[Ir](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

[!INCLUDE [sample-code](includes/snippets/go/create-requests-index.md)]

---

## <a name="use-expand-to-access-related-entities"></a>Usar $expand para acessar entidades relacionadas

Você pode usar o filtro para solicitar uma entidade relacionada ou uma coleção de entidades, ao mesmo tempo em que `$expand` solicita a entidade principal.

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-expand.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-expand.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-expand.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-expand.md)]

# <a name="go"></a>[Ir](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

[!INCLUDE [sample-code](includes/snippets/go/create-requests-expand.md)]

---

## <a name="delete-an-entity"></a>Excluir uma entidade

As solicitações de exclusão são construídas da mesma forma que as solicitações para recuperar uma entidade, mas usam uma `DELETE` solicitação em vez de `GET` um .

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-delete.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-delete.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-delete.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-delete.md)]

# <a name="go"></a>[Ir](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

[!INCLUDE [sample-code](includes/snippets/go/create-requests-delete.md)]

---

## <a name="make-a-post-request-to-create-a-new-entity"></a>Fazer uma solicitação POST para criar uma nova entidade

Para SDKs que suportam um estilo fluente, novos itens podem ser adicionados a coleções com um `Add` método. Para SDKs baseados em modelo, o objeto request expõe um `post` método. Para o PowerShell, `New-*` um comando está disponível que aceita parâmetros que mapeiam para a entidade a ser acrescentada. A entidade criada geralmente é retornada da chamada.

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-create.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-create.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-create.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-create.md)]

# <a name="go"></a>[Ir](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

[!INCLUDE [sample-code](includes/snippets/go/create-requests-create.md)]

---

## <a name="updating-an-existing-entity-with-patch"></a>Atualizando uma entidade existente com PATCH

A maioria das atualizações no Microsoft Graph são executadas usando um método e, portanto, só é necessário incluir as propriedades que você deseja alterar no `PATCH` objeto que você passar.

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-update.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-update.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-update.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-update.md)]

# <a name="go"></a>[Ir](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

[!INCLUDE [sample-code](includes/snippets/go/create-requests-update.md)]

---

## <a name="use-http-headers-to-control-request-behavior"></a>Usar cabeçalhos HTTP para controlar o comportamento da solicitação

Você pode usar uma `Header()` função para anexar os headers personalizados a uma solicitação. Para o PowerShell, a adição de headers só é possível com o `Invoke-GraphRequest` método. Vários cenários da Microsoft Graph usam headers personalizados para ajustar o comportamento da solicitação.

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-headers.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-headers.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-headers.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-headers.md)]

# <a name="go"></a>[Ir](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

[!INCLUDE [sample-code](includes/snippets/go/create-requests-headers.md)]

---

## <a name="provide-custom-query-parameters"></a>Fornecer parâmetros de consulta personalizados

Para SDKs que oferecem suporte a um estilo fluente, você pode fornecer valores de parâmetro de consulta personalizados usando uma lista de `QueryOptions` objetos. Para SDKs baseados em modelo, os parâmetros são codificados por URL e adicionados ao URI de solicitação. Para o PowerShell e o Go, os parâmetros de consulta definidos para uma determinada API são expostos como parâmetros para o comando correspondente.

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-queryparams.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-queryparams.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-queryparams.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-queryparams.md)]

# <a name="go"></a>[Ir](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

[!INCLUDE [sample-code](includes/snippets/go/create-requests-queryparams.md)]

---
