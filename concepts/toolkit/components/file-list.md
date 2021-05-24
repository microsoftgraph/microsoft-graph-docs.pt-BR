---
title: Componente de lista de arquivos no microsoft Graph Toolkit
description: O componente de lista de arquivos é usado para exibir uma lista de arquivos mostrando seu ícone e nome
localization_priority: Normal
author: beth-panx
ms.openlocfilehash: bde548e843170de6cd1234f14096339859d4b99b
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629165"
---
# <a name="file-list-component-in-the-microsoft-graph-toolkit"></a>Componente de lista de arquivos no microsoft Graph Toolkit

O componente Lista [](/graph/api/resources/onedrive) de Arquivos exibe uma lista de várias pastas e arquivos usando o nome do arquivo/pasta, um ícone e outras propriedades que você especificar. Esse componente usa o [componente mgt-file.](./file.md) Você pode especificar uma unidade ou site específico, exibir uma lista de arquivos com base no tipo de insight (tendência, usado ou compartilhado) ou fornecer consultas para uma lista personalizada de arquivos.

## <a name="example"></a>Exemplo

O exemplo a seguir exibe um arquivo usando o `mgt-file-list` componente. Você pode usar o editor de código para ver como as [propriedades](#properties) alteram o comportamento do componente.

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-file-list--file-list&source=docs" height="250"></iframe>

[Abra este exemplo em mgt.dev](https://mgt.dev/?path=/story/components-mgt-file-list--file-list&source=docs)

## <a name="properties"></a>Propriedades

Você pode usar várias propriedades para personalizar o componente.

| Atributo | Propriedade | Descrição |
| --------- | -------- | ----------- |
| file-list-query | fileListQuery | A consulta completa ou o caminho para a unidade ou site que contém a lista de arquivos a ser renderização. |
| file-queries | fileQueries | Uma matriz de consultas de arquivo a serem renderizadas pelo componente. |
| nenhuma | arquivos | Uma matriz de arquivos para obter ou definir a lista de arquivos renderizados pelo componente. Use isso para acessar os arquivos carregados pelo componente. De definir esse valor para carregar seus próprios arquivos. |
| tipo de insight | insightType | Definido para mostrar os arquivos de tendência, usados ou compartilhados do usuário. |
| drive-id | driveId | ID da unidade à que a pasta pertence. Também deve fornecer um `item-id` ou `item-path` . |
| group-id | groupId | ID do grupo ao que a pasta pertence. Também deve fornecer um `item-id` ou `item-path` . |
| site-id | siteId | ID do site ao que a pasta pertence. Também deve fornecer um `{item-id}` ou `{item-path}` . Forneça `{list-id}` se você estiver fazendo referência a um arquivo de uma lista específica. |
| item-id | itemId | ID da pasta. A consulta padrão é `/me/drive/items` . Forneça `{drive-id}` , , ou para consultar um local `{group-id}` `{site-id}` `{user-id}` específico. |
| item-path | itemPath | Caminho do item da pasta (em relação à raiz). A consulta padrão é `/me/drive/root` . Forneça `{drive-id}` , , ou para consultar um local `{group-id}` `{site-id}` `{user-id}` específico. |
| tamanho da página | pageSize | Um valor de número para indicar o número máximo de arquivos a renderizar em cada página. |
| file-extensions | fileExtensions | Uma matriz de extensões de arquivo usadas para filtrar arquivos para mostrar. |
| hide-more-files-button | hideMoreFilesButton | Um booleano para indicar se é preciso mostrar um botão para renderizar mais arquivos. |

O exemplo a seguir altera o comportamento do componente para buscar uma lista de arquivos de uma consulta específica.

```html
<mgt-file-list file-list-query="/me/drive/items/01BYE5RZYJ43UXGBP23BBIFPISHHMCDTOY/children"></mgt-file-list>
```

O exemplo a seguir altera o comportamento do componente para buscar uma lista de arquivos de uma pasta fornecendo a id da pasta.

```html
<mgt-file-list item-id="01BYE5RZYJ43UXGBP23BBIFPISHHMCDTOY"></mgt-file-list>
```

O exemplo a seguir altera o comportamento do componente para buscar a lista de arquivos de um grupo fornecendo a id do grupo e o caminho da pasta.

```html
<mgt-file-list group-id="8090c93e-ba7c-433e-9f39-08c7ba07c0b3" item-path="/Design"></mgt-file-list>
```

O exemplo a seguir altera o comportamento do componente para buscar a lista de arquivos de um usuário, fornecendo a ID do usuário e a id da pasta.

```html
<mgt-file-list user-id="48d31887-5fad-4d73-a9f5-3c356e68a038" item-id="01BYE5RZYFPM65IDVARFELFLNTXR4ZKABD"></mgt-file-list>
```

O exemplo a seguir altera o comportamento do componente para buscar a lista de arquivos fornecendo o tipo de insight.

```html
<mgt-file-list insight-type="shared"></mgt-file-list>
```

## <a name="methods"></a>Métodos
| Método | Descrição |
| --- | --- |
| reload(clearCache = false) | Chame o método para recarregar o componente com novos dados potenciais com base em suas propriedades. Passe `true` para limpar o cache antes de recarregar. |

## <a name="css-custom-properties"></a>Propriedades personalizadas CSS

O `mgt-file-list` componente define as seguintes propriedades personalizadas CSS.

```css
mgt-file-list {
  --font-family: 'Segoe UI';
  --font-size: 14px;

  --file-list-background-color: #ffffff;
  --file-list-border: none;
  --file-list-box-shadow: none;
  --file-list-padding: 4px 0;
  --file-list-margin: 0;

  --file-item-background-color--hover: rgba(0, 0, 0, 0.1);
  --file-item-background-color--active: rgba(0, 0, 0, 0.05);
  --file-item-border-radius: 2px;
  --file-item-margin: 0 4px;

  --file-item-border-top: none;
  --file-item-border-left: none;
  --file-item-border-right: none;
  --file-item-border-bottom: none;

  --show-more-button-background-color: #f3f2f1;
  --show-more-button-background-color--hover: rgba(0, 0, 0, 0.1);
  --show-more-button-font-size: 12px;
  --show-more-button-padding: 6px;
  --show-more-button-border-bottom-right-radius: 4px;
  --show-more-button-border-bottom-left-radius: 4px;
}
```

Para saber mais, confira [componentes de estilo](../customize-components/style.md).

## <a name="microsoft-graph-apis-and-permissions"></a>ApIs Graph Microsoft e permissões

| Configuração | Permissions | API |
| ------------- | ----------------- | --- |
| Padrão (nenhum identificador ou consulta fornecida) | Files.Read, Files.Read.All, Sites.Read.All | `GET /me/drive/root/children`   |
| Fornecer `{drive-id}` AND `{item-id}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /drives/{drive-id}/items/{item-id}/children` |
| Fornecer `{group-id}` AND `{item-id}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /groups/{group-id}/drive/items/{item-id}/children` |
| Fornecer SOMENTE `{item-id}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /me/drive/items/{item-id}/children` | 
| Fornecer `{site-id}` AND `{item-id}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /sites/{site-id}/drive/items/{item-id}/children` |
| Pprovide `{user-id}` AND `{item-id}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /users/{user-id}/drive/items/{item-id}/children` |
| Fornecer `{drive-id}` AND `{item-path}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /drives/{drive-id}/root:/{item-path}:/children` |
| Fornecer `{group-id}` AND `{item-path}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /groups/{group-id}/root:/{item-path}:/children` |
| Fornecer `{site-id}` AND `{item-path}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /sites/{site-id}/root:/{item-path}:/children` |
| Fornecer `{user-id}` AND `{item-path}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /users/{user-id}/root:/{item-path}:/children` |
| Fornecer somente `{item-path}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /me/drive/root:/{item-path}:/children` |
| `insight-type` é definido como tendência | Sites.Read.All | `GET /me/insights/trending` |
| Fornecer `{user-id or upn}` AND está definido `insight-type` como `trending` | Sites.Read.All | `GET /users/{id or userPrincipalName}/insights/trending` | 
| `insight-type` está definido como `used` | Sites.Read.All | `GET /me/insights/used` |
| Fornecer `{user-id or upn}` AND está definido `insight-type` como `used` | Sites.Read.All | `GET /users/{id or userPrincipalName}/insights/used` |
| `insight-type` é definido como compartilhado | Sites.Read.All | `GET /me/insights/shared` |
| Fornecer `{user-id or upn}` AND está definido `insight-type` como `shared` | Sites.Read.All | `GET /users/{id or userPrincipalName}/insights/shared?$filter=((lastshared/sharedby/id eq '${user-id}') and (resourceReference/type eq 'microsoft.graph.driveItem'))` |

## <a name="events"></a>Eventos

| Evento | Descrição |
| ----- | ----------- |
| itemClick | Disparado quando o usuário clica em um arquivo. Retorna os detalhes do arquivo. |

## <a name="templates"></a>Modelos

O `mgt-file-list` componente dá suporte a vários [modelos](../customize-components/templates.md) que permitem substituir determinadas partes do componente. Para especificar um modelo, inclua um elemento dentro de um componente e de definir o valor como um dos tipos de dados `<template>` `data-type` listados na tabela a seguir.

| Tipo de dados | Contexto de dados | Descrição |
| ----------- | -------------- | ------------ |
| Padrão. | `files`: lista de objetos de arquivo | O modelo padrão substitui todo o componente por seu próprio. |
| file | `file`: objeto file | O modelo usado para renderizar cada arquivo. |
| no-data | Nenhum contexto de dados é passado | O modelo usado quando nenhum dado está disponível. |
| loading | Nenhum contexto de dados é passado | O modelo usado enquanto o componente carrega o estado. |

## <a name="authentication"></a>Autenticação

O controle usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md) para buscar os dados necessários.

## <a name="cache"></a>Cache

|Armazenamento de objetos|Dados armazenados em cache|Comentários|
|---------|-----------|-------|
|`fileLists`|Lista de listas de arquivos|Lista de cache padrão para armazenar listas de arquivos.|
|`insightfileLists`|Lista de listas de arquivos de insight|Usado quando `insightType` fornecido.|

> [!NOTE]
> O `mgt-file-list` componente também usa o armazenamento de objetos em `fileQueries` `mgt-file` IndexedDB para armazenar arquivos em cache quando `fileQueries` é fornecido.

Para obter detalhes sobre como configurar o cache, [consulte Caching](../customize-components/cache.md).