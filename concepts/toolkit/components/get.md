---
title: Obter componente no Microsoft Graph Toolkit
description: Um componente Get permite que você faça qualquer consulta GET do Microsoft Graph diretamente no HTML.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 77beb3940eb29a2c9158fba88d78084639e433ed
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39921694"
---
# <a name="get-component-in-the-microsoft-graph-toolkit"></a>Obter componente no Microsoft Graph Toolkit

Você pode usar `mgt-get` o para tornar qualquer consulta Get do Microsoft Graph diretamente no HTML. O componente não fornece uma interface do usuário padrão e requer que você escreva um modelo.

## <a name="example"></a>Exemplo

```html
<mgt-get resource="/me/messages" version="beta" scopes="mail.read" max-pages="2">
  <template>
    emails: {{value.length}}
  </template>
  <template data-type="loading">
    loading
  </template>
</mgt-get>
```

## <a name="properties-and-attributes"></a>Propriedades e atributos

Você pode usar vários atributos para alterar o comportamento do componente. O único atributo obrigatório é `resource`.

| Atributo | Propriedade  | Descrição |
| --- | --- | --- |
| recurso | recurso | O recurso a ser obtido do Microsoft Graph (por exemplo `/me`,). |
| escopos | escopos | Matriz opcional de cadeias de caracteres se você usar a propriedade ou um escopo delimitado por vírgula se estiver usando o atributo. O componente usará esses escopos (com um provedor suportado) para garantir que o usuário tenha sido aceito para a permissão correta. |
| versão | versão | Versão da API opcional a ser usada ao fazer a solicitação GET. O padrão é `v1.0`.  |
| Max-Pages | maxPages | Número opcional de páginas (para recursos que dão suporte à paginação). O padrão é 3. Definir esse valor como 0 receberá todas as páginas.  |
| Não disponível | response | Somente leitura resposta do Microsoft Graph se a solicitação tiver sido bem-sucedida.  |
| Não disponível |erro| Somente leitura erro do Microsoft Graph se a solicitação não tiver sido bem-sucedida. |

## <a name="events"></a>Eventos
| Evento | Detalhe | Descrição |
| --- | --- | --- |
| dataChange | O detalhe contém os `response` objetos `error` e. | Acionado quando a resposta ou erro é alterada. |

## <a name="templates"></a>Modelos

O `mgt-get` componente suporta vários [modelos](../templates.md) que você pode usar para definir a aparência. Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina `data-type` o valor como um dos seguintes.

| Tipo de dados | Contexto de dados | Descrição |
| --- | --- | --- |
| Padrão. | A resposta do Microsoft Graph. | O modelo padrão é necessário para renderizar os dados provenientes do Microsoft Graph. |
| erro | O erro do Microsoft Graph. | Este modelo será usado se houver um erro ao fazer a solicitação. |
| carregando | Não disponível | Este modelo é usado enquanto a solicitação é feita. |

## <a name="microsoft-graph-permissions"></a>Permissões do Microsoft Graph

Para obter mais informações sobre permissões, consulte a [referência de permissões](https://docs.microsoft.com/graph/permissions-reference)do Microsoft Graph. 

## <a name="authentication"></a>Autenticação

O controle usa o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md) para buscar os dados necessários.
