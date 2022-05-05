---
title: Criar, atualizar e excluir conexões no Microsoft Graph
description: Saiba como usar o Microsoft Graph para criar e gerenciar conexões.
ms.localizationpriority: high
author: mecampos
doc_type: conceptualPageType
ms.prod: search
ms.openlocfilehash: 1ea29376e69365724ecea76882c801a9acd807b5
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202039"
---
<!---<author of this doc: rsamai>--->

# <a name="create-update-and-delete-connections-in-microsoft-graph"></a>Criar, atualizar e excluir conexões no Microsoft Graph

As conexões de serviços externos com o serviço da Pesquisa da Microsoft são representadas pelo recurso [externalConnection](/graph/api/resources/externalconnectors-externalconnection?view=graph-rest-1.0&preserve-view=true) no Microsoft Graph.

A plataforma de conectores do Microsoft Graph oferece uma maneira intuitiva de adicionar seus dados externos ao Microsoft Graph. Uma conexão é um contêiner lógico de dados externos que um administrador pode gerenciar como uma única unidade.

Após uma conexão ter sido criada, você pode adicionar seu conteúdo de qualquer fonte de dados externa, como uma fonte de conteúdo local ou um serviço SaaS externo. Só é possível exibir e gerenciar as conexões que você [criou](/graph/api/externalconnectors-external-post-connections?view=graph-rest-1.0&preserve-view=true&tabs=http) ou que foram explicitamente autorizadas para gerenciamento. Um administrador de pesquisa pode exibir e gerenciar todas as conexões no locatário no Centro de Administração Moderna.

<!-- markdownlint-disable MD036 -->
![Amostra de um sistema de assistência técnica personalizado da Estrutura de Conector de Tíquetes.](./images/connectors-images/connecting-external-content-manage-connections-connector-structure.png)

*Amostra de um sistema de assistência técnica personalizado da Estrutura de Conector de Tíquetes.*

![Modo de exibição de administrador das conexões, incluindo o Conector de Tíquetes personalizado.](./images/connectors-images/connecting-external-content-manage-connections-admin-view.svg)

*Modo de exibição de administrador das conexões, incluindo o Conector de Tíquetes personalizado.*

<!-- markdownlint-enable MD036 -->

Você pode modelar uma conexão da maneira que quiser mas criar uma conexão para cada instância do seu conector é o modelo mais comum. Por exemplo, cada vez que você [configurar o conector de compartilhamento de arquivos do Microsoft Windows](/en-us/microsoftsearch/configure-connector), uma nova conexão é criada. Você também pode criar uma única conexão para adicionar todos os itens da fonte de dados. Por exemplo, v pode criar uma única conexão para adicionar todos os tíquetes e incidentes em várias equipes a partir de seu sistema de assistência técnica.

## <a name="states-and-operations"></a>Estados e operações

A conexão pode existir em um dos seguintes estados.

| Estado             | Descrição                |
|-------------------|----------------------------|
| **Rascunho**         | Uma conexão vazia está provisionada. A fonte de dados, esquema ou quaisquer configurações ainda não foram configuradas. |
| **Pronto**         | A conexão é fornecida com o esquema registrado e está pronta para inclusão. |
| **Obsoleto**      | Isso ocorre quando um recurso dependente, como uma API, foi preterido. A exclusão da conexão é a única operação válida. |
| **LimitExceeded** | Se você atingir o limite máximo de uma única conexão ou da cota de nível do locatário em todas as conexões, não poderá adicionar mais itens até que você saia do estado. |

A tabela a seguir especifica quais operações estão disponíveis em cada Estado.

| Operação         | Rascunho              | Pronto              | Obsoleto           | LimitExceeded      |
|-------------------|--------------------|--------------------|--------------------|--------------------|
| Criar conexão | :x:                | :heavy_check_mark: | :x:                | :heavy_check_mark: |
| Ler conexão   | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
| Atualizar conexão | :heavy_check_mark: | :heavy_check_mark: | :x:                | :heavy_check_mark: |
| Excluir conexão | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
| Criar esquema     | :heavy_check_mark: | :x:                | :x:                | :x:                |
| Ler esquema       | :x:                | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
| Atualizar esquema     | :x:                | :x:                | :x:                | :x:                |
| Excluir esquema     | :x:                | :x:                | :x:                | :x:                |
| Criar item       | :x:                | :heavy_check_mark: | :x:                | :x:                |
| Ler item         | :x:                | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
| Atualizar item       | :x:                | :heavy_check_mark: | :x:                | :heavy_check_mark: |
| Excluir item       | :x:                | :heavy_check_mark: | :x:                | :heavy_check_mark: |

Uma conexão permite que seu aplicativo [defina um esquema](/graph/api/externalconnectors-externalconnection-post-schema?view=graph-rest-beta&preserve-view=true&tabs=http&viewFallbackFrom=graph-rest-1.0) para os itens que serão indexados, e que ele forneça um ponto de extremidade para o seu serviço adicionar, atualizar ou excluir itens do índice. 

Criar uma conexão é a primeira etapa para um aplicativo para adicionar itens ao índice de pesquisa.

## <a name="create-a-connection"></a>Criar uma conexão

Antes que um aplicativo possa adicionar itens ao índice de pesquisa, ele deve criar e configurar uma conexão:

1. [Criar uma conexão](/graph/api/externalconnectors-external-post-connections?view=graph-rest-1.0&preserve-view=true&tabs=http) com ID exclusiva, nome de exibição e descrição.
2. [Registre um esquema](/graph/api/externalconnectors-externalconnection-post-schema?view=graph-rest-beta&preserve-view=true&tabs=http&viewFallbackFrom=graph-rest-1.0) para definir os campos que serão incluídos no índice.

> [!NOTE]
> Para obter informações sobre como atualizar o esquema de uma conexão existente, consulte [Recursos da atualização do esquema](/graph/connecting-external-content-manage-schema#schema-update-capabilities).

## <a name="update-a-connection"></a>Atualizar uma conexão

Para alterar o nome de exibição ou a descrição de uma conexão existente, você pode [atualizar a conexão](/graph/api/externalconnectors-externalconnection-update?view=graph-rest-1.0&preserve-view=true&tabs=http).

## <a name="delete-a-connection"></a>Excluir uma conexão

Para remover todos os itens que foram indexados por meio de uma conexão, você pode [excluir uma conexão](/graph/api/externalconnectors-externalconnection-delete?view=graph-rest-1.0&preserve-view=true&tabs=http).

## <a name="next-steps"></a>Próximas etapas

- [Registrar o esquema de conexão](connecting-external-content-manage-schema.md)
- [Revisar a referência da API do conectores do Microsoft Graph](/graph/api/resources/indexing-api-overview?view=graph-rest-1.0&preserve-view=true)
- [Baixar o modelo do conector de pesquisa do GitHub](https://github.com/microsoftgraph/msgraph-search-connector-sample)
