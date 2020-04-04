---
title: Obter componente no Microsoft Graph Toolkit
description: Um componente Get permite que você faça qualquer consulta GET do Microsoft Graph diretamente no HTML.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: b9dcbd5af4c9938dce821c30021a4cf3439fd1b2
ms.sourcegitcommit: 1bc5a0c179dce57e90349610566fb86e1b5fbf95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/04/2020
ms.locfileid: "43144314"
---
# <a name="get-component-in-the-microsoft-graph-toolkit"></a>Obter componente no Microsoft Graph Toolkit

Você pode usar `mgt-get` o para tornar qualquer consulta Get do Microsoft Graph diretamente no HTML. O componente não fornece uma interface do usuário padrão e requer que você escreva um modelo.

## <a name="example"></a>Exemplo

O exemplo a seguir mostra o uso do `mgt-get` componente para exibir os emails de um usuário. Você pode usar o editor de código para ver como [as propriedades e os atributos](#properties-and-attributes) alteram o comportamento do componente.

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-get--get-email&source=docs" height="500"></iframe>

[Abra este exemplo em gerenciamento de. dev](https://mgt.dev/?path=/story/components-mgt-get--get-email&source=docs)

## <a name="properties-and-attributes"></a>Propriedades e atributos

Você pode usar vários atributos para alterar o comportamento do componente. O único atributo obrigatório é `resource`.

| Atributo | Propriedade  | Descrição |
| --- | --- | --- |
| recurso | recurso | O recurso a ser obtido do Microsoft Graph (por exemplo `/me`,). |
| escopos | escopos | Matriz opcional de cadeias de caracteres se você usar a propriedade ou um escopo delimitado por vírgula se estiver usando o atributo. O componente usará esses escopos (com um provedor suportado) para garantir que o usuário tenha sido aceito para a permissão correta. |
| versão | versão | Versão da API opcional a ser usada ao fazer a solicitação GET. O padrão é `v1.0`.  |
| Max-Pages | maxPages | Número opcional de páginas (para recursos que dão suporte à paginação). O padrão é 3. Definir esse valor como 0 receberá todas as páginas.  |
| taxa de sondagem | pollingRate | Número opcional de miliseconds. Quando definido, o componente irá sondar o URI de solicitação para atualizações no intervalo definido. Se você estiver usando uma consulta Delta, a pesquisa sempre consultará a API Delta. O modelo só será atualizado quando os dados forem alterados. |
| Não disponível | response | Somente leitura resposta do Microsoft Graph se a solicitação tiver sido bem-sucedida.  |
| Não disponível |erro| Somente leitura erro do Microsoft Graph se a solicitação não tiver sido bem-sucedida. |

## <a name="methods"></a>Métodos
| Método | Descrição |
| --- | --- |
| atualizar (forçar?: Boolean) | Chame o método para atualizar os dados. Por padrão, a interface do usuário só será atualizada se os dados forem alterados. Passe `true` para forçar o componente a atualizar.  |


## <a name="events"></a>Eventos
| Evento | Detalhe | Descrição |
| --- | --- | --- |
| dataChange | O detalhe contém os `response` objetos `error` e. | Acionado quando a resposta ou erro é alterada. |

## <a name="templates"></a>Modelos

O `mgt-get` componente suporta vários [modelos](../templates.md) que você pode usar para definir a aparência. Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina `data-type` o valor como um dos seguintes.

| Tipo de dados | Contexto de dados | Descrição |
| --- | --- | --- |
| Padrão. | A resposta do Microsoft Graph. | O modelo padrão é necessário para renderizar os dados provenientes do Microsoft Graph. |
| valor | Item de dados da matriz `value` retornada | Use o `value` modelo em vez do `default` modelo ao esperar a resposta do gráfico para conter uma matriz de itens, como **mensagens**, **arquivos**ou **usuários**. O `value` modelo será repetido automaticamente para cada item retornado pelo recurso. O `value` modelo também começará a renderizar os itens assim que eles estiverem prontos (ao contrário do modelo padrão).|
| erro | O erro do Microsoft Graph. | Este modelo será usado se houver um erro ao fazer a solicitação. |
| carregando | Não disponível | Este modelo é usado enquanto a solicitação é feita. |

## <a name="microsoft-graph-permissions"></a>Permissões do Microsoft Graph

Para obter mais informações sobre permissões, consulte a [referência de permissões](https://docs.microsoft.com/graph/permissions-reference)do Microsoft Graph. 

## <a name="authentication"></a>Autenticação

O controle usa o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md) para buscar os dados necessários.
