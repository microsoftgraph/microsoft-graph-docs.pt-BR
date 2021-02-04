---
title: Obter componente no Microsoft Graph Toolkit
description: Um componente Get permite que você faça qualquer consulta GET do Microsoft Graph diretamente em seu HTML.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 4ef24d5b5eac0b53029c67dd723ba80c7d0f5bff
ms.sourcegitcommit: d02c438bcd58e8f64bfcd5fba0b40e436b46570e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/04/2021
ms.locfileid: "50101871"
---
# <a name="get-component-in-the-microsoft-graph-toolkit"></a>Obter componente no Microsoft Graph Toolkit

Você pode usar `mgt-get` para fazer qualquer consulta GET do Microsoft Graph diretamente em seu HTML. O componente não fornece uma interface do usuário padrão e exige que você escreva um modelo.

## <a name="example"></a>Exemplo

O exemplo a seguir mostra o uso do `mgt-get` componente para exibir emails de um usuário. Você pode usar o editor de código para ver como propriedades [e atributos](#properties-and-attributes) alteram o comportamento do componente.

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-get--get-email&source=docs" height="500"></iframe>

[Abra este exemplo em mgt.dev](https://mgt.dev/?path=/story/components-mgt-get--get-email&source=docs)

## <a name="properties-and-attributes"></a>Propriedades e atributos

Você pode usar vários atributos para alterar o comportamento do componente. O único atributo necessário é `resource` .

| Atributo | Propriedade  | Descrição |
| --- | --- | --- |
| recurso | recurso | O recurso a ser obter do Microsoft Graph (por exemplo, `/me` ). |
| escopos | escopos | Matriz opcional de cadeias de caracteres se estiver usando a propriedade ou um escopo delimitado por vírgula se estiver usando o atributo. O componente usará esses escopos (com um provedor suportado) para garantir que o usuário tenha consentido com a permissão correta. |
| versão | versão | Versão da API opcional a ser usada ao fazer a solicitação GET. O padrão é `v1.0`.  |
| max-pages | maxPages | Número opcional de páginas (para recursos que suportam paginação). O padrão é 3. Definir esse valor como 0 obterá todas as páginas.  |
| polling-rate | pollingRate | Número opcional de milissegundos. Quando definido, o componente sonda o URI da solicitação para atualizações no intervalo definido. Se estiver usando uma consulta delta, a sondagem sempre consultará a API delta. O modelo será atualizado somente quando os dados mudarem. |
| habilitado para cache | cacheEnabled | Boolean opcional. Quando definido, indica que a resposta do recurso será armazenada em cache. Substituir se `refresh()` for chamado ou se estiver em `pollingRate` uso. O padrão é `false`. |
| cache-invalidation-period | cacheInvalidationPeriod | Número opcional de milissegundos. Quando definido em combinação com `cacheEnabled` , o atraso antes de o cache atingir seu período de invalidação será modificado por esse valor. O padrão `0` é e usará o período de invalidação padrão. |
| type | type | Tipo opcional da resposta esperada. O padrão é `json`. Oferece `json` suporte `image` ou (só tem suporte em pontos de extremidade terminando com `/photo/value$` ). |
| Não disponível | response | Resposta somente leitura do Microsoft Graph se a solicitação foi bem-sucedida.  |
| Não disponível |erro| Erro somente leitura do Microsoft Graph se a solicitação não tiver sido bem-sucedida. |

## <a name="methods"></a>Métodos
| Método | Descrição |
| --- | --- |
| refresh(force?:boolean) | Chame o método para atualizar os dados. Por padrão, a interface do usuário será atualizada somente se os dados mudarem. Passe `true` para forçar o componente a ser atualizado.  |


## <a name="events"></a>Eventos
| Event | Detalhe | Descrição |
| --- | --- | --- |
| dataChange | Os detalhes contêm `response` os objetos e os `error` objetos. | Disparado quando a resposta ou o erro mudar. |

## <a name="templates"></a>Modelos

O `mgt-get` componente dá suporte a vários [modelos](../customize-components/templates.md) que você pode usar para definir a aparência. Para especificar um modelo, inclua um elemento dentro de um componente e de definir `<template>` o valor como um dos `data-type` seguintes.

| Tipo de dados | Contexto de dados | Descrição |
| --- | --- | --- |
| Padrão. | A resposta do Microsoft Graph. | O modelo padrão é necessário para renderizar os dados provenientes do Microsoft Graph. |
| valor | Item de dados da matriz `value` retornada | Use o modelo em vez do modelo ao esperar que a resposta do gráfico contenha uma matriz de itens - como mensagens , arquivos `value` `default` ou **usuários**.   O `value` modelo será repetido automaticamente para cada item retornado pelo recurso. O `value` modelo também começará a renderizar os itens assim que eles estão prontos (ao contrário do modelo padrão).|
| erro | O erro do Microsoft Graph. | Esse modelo será usado se houver um erro ao fazer a solicitação. |
| carregando | Não disponível | Esse modelo é usado enquanto a solicitação está sendo feita. |

## <a name="microsoft-graph-permissions"></a>Permissões do Microsoft Graph

Para obter mais informações sobre permissões, consulte a referência de [permissões do](../../permissions-reference.md)Microsoft Graph. 

## <a name="authentication"></a>Autenticação

O controle usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md) para buscar os dados necessários.
