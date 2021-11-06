---
title: Obter componente no Microsoft Graph Toolkit
description: Um componente Get permite que você faça qualquer consulta GET da Microsoft Graph diretamente em seu HTML.
ms.localizationpriority: medium
author: nmetulev
ms.openlocfilehash: 1d12fbe73daa21221ca95cc50e0ae2aa2d44e642
ms.sourcegitcommit: c00c61ce35a6f204a9907aa6f2644ea7a86a5b6e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2021
ms.locfileid: "60805385"
---
# <a name="get-component-in-the-microsoft-graph-toolkit"></a>Obter componente no Microsoft Graph Toolkit

Você pode usar para fazer qualquer consulta GET da `mgt-get` Microsoft Graph diretamente em seu HTML. O componente não fornece uma interface do usuário padrão e exige que você escreva um modelo.

## <a name="example"></a>Exemplo

O exemplo a seguir mostra o uso do `mgt-get` componente para exibir emails de um usuário. Você pode usar o editor de código para ver como propriedades [e atributos](#properties-and-attributes) alteram o comportamento do componente.

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-get--get-email&source=docs" height="500"></iframe>

[Abrir este exemplo no mgt.dev](https://mgt.dev/?path=/story/components-mgt-get--get-email&source=docs)

## <a name="properties-and-attributes"></a>Propriedades e atributos

Você pode usar vários atributos para alterar o comportamento do componente. O único atributo necessário é `resource` .

| Atributo | Propriedade  | Descrição |
| --- | --- | --- |
| recurso | recurso | O recurso a ser Graph microsoft (por exemplo, `/me` ). |
| escopos | escopos | Matriz opcional de cadeias de caracteres se estiver usando a propriedade ou um escopo delimitado por vírgula se estiver usando o atributo. O componente usará esses escopos (com um provedor com suporte) para garantir que o usuário tenha consentido com a permissão certa. |
| versão | versão | Versão da API opcional a ser usada ao fazer a solicitação GET. O padrão é `v1.0`.  |
| max-pages | maxPages | Número opcional de páginas (para recursos que suportam paginação). O padrão é 3. Definir esse valor como 0 receberá todas as páginas.  |
| polling-rate | pollingRate | Número opcional de milissegundos. Quando definido, o componente sonda o URI de solicitação para atualizações no intervalo definido. Se estiver usando uma consulta delta, a sondagem sempre consultará a API delta. O modelo só será atualizado quando os dados mudarem. |
| habilitado para cache | cacheEnabled | Boolean opcional. Quando definido, indica que a resposta do recurso será armazenada em cache. Substitua se `refresh()` for chamado ou se estiver em `pollingRate` uso. O padrão é `false`. |
| cache-invalidation-period | cacheInvalidationPeriod | Número opcional de milissegundos. Quando definido em combinação com , o atraso antes que o cache atinja seu período `cacheEnabled` de invalidação será modificado por esse valor. O padrão `0` é e usará o período de invalidação padrão. |
| type | type | Tipo opcional da resposta esperada. O padrão é `json`. Suporta `json` ou `image` (só há suporte para pontos de extremidade terminando com `/photo/value$` ). |
| Não disponível | response | Resposta somente leitura da Microsoft Graph se a solicitação foi bem-sucedida.  |
| Não disponível |erro| Erro somente leitura da Microsoft Graph se a solicitação não tiver sido bem-sucedida. |

## <a name="methods"></a>Métodos

| Método | Descrição |
| --- | --- |
| refresh(force?:boolean) | Chame o método para atualizar os dados. Por padrão, a interface do usuário só será atualizada se os dados mudarem. Passe `true` para forçar o componente a atualizar.  |

## <a name="events"></a>Eventos

Evento | Quando é emitido | Dados personalizados | Cancelável | Bolhas | Funciona com modelo personalizado
------|-------------------|--------------|:-----------:|:---------:|:---------------------------:|
`dataChange` | Disparado depois que o componente carregou seus dados. | `{ response: any, error: any }`. A `response` propriedade contém a resposta recuperada do Microsoft Graph. A `error` propriedade contém informações sobre o erro se um ocorreu | Não | Não | Sim

> [!TIP]
> Para obter mais informações sobre os dados retornados na propriedade, consulte a referência de API da API que você usou na propriedade `response` `resource` do componente Get.

Para obter mais informações sobre como lidar com eventos, consulte [eventos](../customize-components/events.md).

## <a name="templates"></a>Modelos

O `mgt-get` componente dá suporte a vários [modelos](../customize-components/templates.md) que você pode usar para definir a aparência. Para especificar um modelo, inclua um elemento dentro de um componente e de definir o `<template>` valor como um dos `data-type` seguintes.

| Tipo de dados | Contexto de dados | Descrição |
| --- | --- | --- |
| Padrão. | A resposta do Microsoft Graph. | O modelo padrão é necessário para renderizar os dados provenientes do Microsoft Graph. |
| valor | Item de dados da matriz `value` retornada | Use o modelo em vez do modelo ao esperar que a resposta do gráfico contenha uma matriz de itens - como mensagens, arquivos `value` `default` ou **usuários**.   O `value` modelo será repetido automaticamente para cada item retornado pelo recurso. O `value` modelo também começará a renderizar os itens assim que eles estão prontos (ao contrário do modelo padrão).|
| erro | O erro da Microsoft Graph. | Esse modelo será usado se houver um erro ao fazer a solicitação. |
| loading | N/D | Esse modelo é usado enquanto a solicitação está sendo feita. |
| no-data | Não disponível | Esse modelo é usado quando a solicitação não retorna dados. |

## <a name="microsoft-graph-permissions"></a>Permissões do Microsoft Graph

As permissões exigidas por esse componente dependem dos dados que você deseja recuperar com eles do Microsoft Graph. Para obter mais informações sobre permissões, consulte a referência de permissões do Microsoft Graph [.](../../permissions-reference.md)

## <a name="authentication"></a>Autenticação

O controle usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md) para buscar os dados necessários.

## <a name="cache"></a>Cache

Para habilitar e configurar o cache, use `cacheEnabled` as propriedades `cacheInvalidationPeriod` e. Por padrão, o `mgt-get` componente não armazena em cache nenhuma resposta.

|Armazenamento de objetos|Dados armazenados em cache|Comentários|
|-----------|-----------|-------|
|`response`|Resposta completa recuperada do Microsoft Graph para a consulta especificada na `resource` propriedade de`mgt-get`|

Consulte [Caching](../customize-components/cache.md) para obter mais detalhes.
