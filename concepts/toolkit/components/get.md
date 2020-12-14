---
title: Obter componente no Microsoft Graph Toolkit
description: Um componente Get permite que você faça qualquer consulta GET do Microsoft Graph diretamente no HTML.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 7ce33d231b02603c953a57df8ae8751f8544ee7a
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659377"
---
# <a name="get-component-in-the-microsoft-graph-toolkit"></a>Obter componente no Microsoft Graph Toolkit

Você pode usar `mgt-get` o para tornar qualquer consulta Get do Microsoft Graph diretamente no HTML. O componente não fornece uma interface do usuário padrão e requer que você escreva um modelo.

## <a name="example"></a>Exemplo

O exemplo a seguir mostra o uso do `mgt-get` componente para exibir os emails de um usuário. Você pode usar o editor de código para ver como [as propriedades e os atributos](#properties-and-attributes) alteram o comportamento do componente.

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-get--get-email&source=docs" height="500"></iframe>

[Abra este exemplo em gerenciamento de. dev](https://mgt.dev/?path=/story/components-mgt-get--get-email&source=docs)

## <a name="properties-and-attributes"></a>Propriedades e atributos

Você pode usar vários atributos para alterar o comportamento do componente. O único atributo obrigatório é `resource` .

| Atributo | Propriedade  | Descrição |
| --- | --- | --- |
| recurso | recurso | O recurso a ser obtido do Microsoft Graph (por exemplo, `/me` ). |
| escopos | escopos | Matriz opcional de cadeias de caracteres se você usar a propriedade ou um escopo delimitado por vírgula se estiver usando o atributo. O componente usará esses escopos (com um provedor suportado) para garantir que o usuário tenha sido aceito para a permissão correta. |
| versão | versão | Versão da API opcional a ser usada ao fazer a solicitação GET. O padrão é `v1.0`.  |
| Max-Pages | maxPages | Número opcional de páginas (para recursos que dão suporte à paginação). O padrão é 3. Definir esse valor como 0 receberá todas as páginas.  |
| taxa de sondagem | pollingRate | Número opcional de miliseconds. Quando definido, o componente irá sondar o URI de solicitação para atualizações no intervalo definido. Se você estiver usando uma consulta Delta, a pesquisa sempre consultará a API Delta. O modelo só será atualizado quando os dados forem alterados. |
| habilitado para cache | cacheEnabled | Boolean opcional. Quando definido, ele indica que a resposta do recurso será armazenada em cache. Overrideed se `refresh()` for chamado ou se `pollingRate` estiver em uso. O padrão é `false`. |
| cache-Invalidation-period | cacheInvalidationPeriod | Número opcional de miliseconds. Quando definido em combinação com `cacheEnabled` , o atraso antes de o cache atingir o período de invalidação será modificado por esse valor. O padrão é `0` e usará o período de invalidação padrão. |
| type | type | Tipo opcional da resposta esperada. O padrão é `json`. Suporta `json` ou `image` (só tem suporte em pontos de extremidade terminados com `/photo/value$` ). |
| N/D | response | Somente leitura resposta do Microsoft Graph se a solicitação tiver sido bem-sucedida.  |
| N/D |erro| Somente leitura erro do Microsoft Graph se a solicitação não tiver sido bem-sucedida. |

## <a name="methods"></a>Métodos
| Método | Descrição |
| --- | --- |
| atualizar (forçar?: Boolean) | Chame o método para atualizar os dados. Por padrão, a interface do usuário só será atualizada se os dados forem alterados. Passe `true` para forçar o componente a atualizar.  |


## <a name="events"></a>Eventos
| Evento | Detalhe | Descrição |
| --- | --- | --- |
| dataChange | O detalhe contém os `response` `error` objetos e. | Acionado quando a resposta ou erro é alterada. |

## <a name="templates"></a>Modelos

O `mgt-get` componente suporta vários [modelos](../customize-components/templates.md) que você pode usar para definir a aparência. Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina o `data-type` valor como um dos seguintes.

| Tipo de dados | Contexto de dados | Descrição |
| --- | --- | --- |
| Padrão. | A resposta do Microsoft Graph. | O modelo padrão é necessário para renderizar os dados provenientes do Microsoft Graph. |
| valor | Item de dados da `value` matriz retornada | Use o `value` modelo em vez do `default` modelo ao esperar a resposta do gráfico para conter uma matriz de itens, como **mensagens**, **arquivos** ou **usuários**. O `value` modelo será repetido automaticamente para cada item retornado pelo recurso. O `value` modelo também começará a renderizar os itens assim que eles estiverem prontos (ao contrário do modelo padrão).|
| erro | O erro do Microsoft Graph. | Este modelo será usado se houver um erro ao fazer a solicitação. |
| carregando | N/D | Este modelo é usado enquanto a solicitação é feita. |

## <a name="microsoft-graph-permissions"></a>Permissões do Microsoft Graph

Para obter mais informações sobre permissões, consulte a [referência de permissões](../../permissions-reference.md)do Microsoft Graph. 

## <a name="authentication"></a>Autenticação

O controle usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md) para buscar os dados necessários.
