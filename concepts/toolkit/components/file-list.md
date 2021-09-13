---
title: Componente de lista de arquivos no microsoft Graph Toolkit
description: O componente de lista de arquivos é usado para exibir uma lista de arquivos mostrando seu ícone e nome
ms.localizationpriority: medium
author: beth-panx
ms.openlocfilehash: 1f3aea2c4d012cd4627167523540fcfeaaaf7651
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59035343"
---
# <a name="file-list-component-in-the-microsoft-graph-toolkit"></a>Componente de lista de arquivos no microsoft Graph Toolkit

O componente Lista [](/graph/api/resources/onedrive) de Arquivos exibe uma lista de várias pastas e arquivos usando o nome do arquivo/pasta, um ícone e outras propriedades que você especificar. Esse componente usa o [componente mgt-file.](./file.md) Você pode especificar uma unidade ou site específico, exibir uma lista de arquivos com base no tipo de insight (tendência, usado ou compartilhado) ou fornecer consultas para uma lista personalizada de arquivos. O componente também fornece a opção de permitir que os usuários carreguem arquivos em um local especificado no One Drive ou SharePoint.

## <a name="example"></a>Exemplo

O exemplo a seguir exibe um arquivo usando o `mgt-file-list` componente. Você pode usar o editor de código para ver como as [propriedades](#properties) alteram o comportamento do componente.

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-file-list--file-list&source=docs" height="250"></iframe>

[Abrir este exemplo no mgt.dev](https://mgt.dev/?path=/story/components-mgt-file-list--file-list&source=docs)

## <a name="properties"></a>Propriedades

Você pode usar várias propriedades para personalizar o componente.

| Atributo | Propriedade | Descrição |
| --------- | -------- | ----------- |
| file-list-query | fileListQuery | A consulta completa ou o caminho para a unidade ou site que contém a lista de arquivos a ser renderização. |
| file-queries | fileQueries | Uma matriz de consultas de arquivo a serem renderizadas pelo componente. |
| Nenhuma | arquivos | Uma matriz de arquivos para obter ou definir a lista de arquivos renderizados pelo componente. Use isso para acessar os arquivos carregados pelo componente. De definir esse valor para carregar seus próprios arquivos. |
| tipo de insight | insightType | Definido para mostrar os arquivos de tendência, usados ou compartilhados do usuário. |
| drive-id | driveId | ID da unidade à que a pasta pertence. Também deve fornecer um `item-id` ou `item-path` . |
| group-id | groupId | ID do grupo ao que a pasta pertence. Também deve fornecer um `item-id` ou `item-path` . |
| site-id | siteId | ID do site ao que a pasta pertence. Também deve fornecer um `{item-id}` ou `{item-path}` . Forneça `{list-id}` se você estiver fazendo referência a um arquivo de uma lista específica. |
| item-id | itemId | ID da pasta. A consulta padrão é `/me/drive/items` . Forneça `{drive-id}` , , ou para consultar um local `{group-id}` `{site-id}` `{user-id}` específico. |
| item-path | itemPath | Caminho do item da pasta (em relação à raiz). A consulta padrão é `/me/drive/root` . Forneça `{drive-id}` , , ou para consultar um local `{group-id}` `{site-id}` `{user-id}` específico. |
| tamanho da página | pageSize | Um valor de número para indicar o número máximo de arquivos a renderizar em cada página. **Observação:** `page-size` não tem suporte com `insight-type` . |
| file-extensions | fileExtensions | Uma matriz de extensões de arquivo usadas para filtrar arquivos para mostrar. |
| hide-more-files-button | hideMoreFilesButton | Boolean para indicar se deve mostrar um botão para renderizar mais arquivos. |
| enable-file-upload | enableFileUpload | Boolean para habilitar ou desabilitar a funcionalidade de carregamento de arquivo. O valor padrão é `false`.  |
| excluded-file-extensions | excludedFileExtensions | Matriz de cadeias de caracteres de extensões de arquivo a serem excluídas do carregamento de arquivo. Também deve definir o `enable-file-upload` atributo como `true` . |
| max-file-size | maxFileSize | Um número que representa o tamanho máximo de carregamento de arquivo (KB). Também deve definir o `enable-file-upload` atributo como `true` . |
| max-upload-file | maxUploadFile | Um número que representa o número máximo de arquivos permitidos para serem carregados. O valor padrão são `10` arquivos. Também deve definir o `enable-file-upload` atributo como `true` . |

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

O exemplo a seguir habilita o recurso de carregamento de arquivo.

```html
<mgt-file-list enable-file-upload></mgt-file-list>
```

O exemplo a seguir limita o número máximo de arquivos que podem ser carregados para 5.

```html
<mgt-file-list max-upload-file="5" enable-file-upload></mgt-file-list>
```

O exemplo a seguir limita o tamanho máximo de arquivo que pode ser carregado para 10.000 KB.

```html
<mgt-file-list max-file-size="10000" enable-file-upload></mgt-file-list>
```

O exemplo a seguir exclui o carregamento de arquivos com extensões de arquivo ".doc,.pdf".

```html
<mgt-file-list excluded-file-extensions=".doc,.pdf" enable-file-upload></mgt-file-list>
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

  --file-upload-border: 4px dotted #ffbdc3;
  --file-upload-background-color: rgba(255, 0, 0, 0.1);
  --file-upload-button-float: left;
  --file-upload-button-color: #323130;
  --file-upload-button-background-color: #fef8dd;
  --file-upload-dialog-content-background-color: #ffe7c7;
  --file-upload-dialog-primarybutton-background-color: #ffe7c7;
  --file-upload-dialog-primarybutton-color: #323130;
}
```

Para saber mais, confira [componentes de estilo](../customize-components/style.md).

## <a name="microsoft-graph-apis-and-permissions"></a>ApIs Graph Microsoft e permissões

| Configuração | Permissões | API |
| ------------- | ----------------- | --- |
| Padrão (nenhum identificador ou consulta fornecida) | Files.Read, Files.Read.All, Sites.Read.All | `GET /me/drive/root/children` |
| Fornecer `enable-file-upload` | Files.Read, Files.Read.All, Sites.Read.All, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All | `GET /me/drive/root/children` <br /> `PUT /me/drive/root:/{filename}:/content` <br /> `POST /me/drive/root:/{filename}:/createUploadSession` |
| Fornecer `{drive-id}` AND `{item-id}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /drives/{drive-id}/items/{item-id}/children`|
| Fornecer `{drive-id}` E `{item-id}` E `enable-file-upload` | Files.Read, Files.Read.All, Sites.Read.All, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All | `GET /drives/{drive-id}/items/{item-id}/children` <br /> `PUT /drives/{drive-id}/items/{item-id}:/{filename}:/content` <br /> `POST /drives/{drive-id}/items/{item-id}:/{filename}:/createUploadSession` |
| Fornecer `{group-id}` AND `{item-id}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /groups/{group-id}/drive/items/{item-id}/children` |
| Fornecer `{group-id}` E `{item-id}` E `enable-file-upload` | Files.Read, Files.Read.All, Sites.Read.All, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All | `GET /groups/{group-id}/drive/items/{item-id}/children` <br /> `PUT /groups/{group-id}/drive/items/{item-id}:/{filename}:/content` <br /> `POST /groups/{group-id}/drive/items/{item-id}:/{filename}:/createUploadSession` |
| Fornecer SOMENTE `{item-id}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /me/drive/items/{item-id}/children` |
| Fornecer SOMENTE `{item-id}` E `enable-file-upload` | Files.Read, Files.Read.All, Sites.Read.All, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All | `GET /me/drive/items/{item-id}/children` <br /> `PUT /me/drive/items/{item-id}:/{filename}:/content` <br /> `POST /me/drive/items/{item-id}:/{filename}:/createUploadSession` |
| Fornecer `{site-id}` AND `{item-id}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /sites/{site-id}/drive/items/{item-id}/children` |
| Fornecer `{site-id}` E `{item-id}` E `enable-file-upload` | Files.Read, Files.Read.All, Sites.Read.All, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All | `GET /sites/{site-id}/drive/items/{item-id}/children` <br /> `PUT /sites/{site-id}/drive/items/{item-id}:/{filename}:/content` <br /> `POST /sites/{site-id}/drive/items/{item-id}:/{filename}:/createUploadSession` |
| Fornecer `{user-id}` AND `{item-id}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /users/{user-id}/drive/items/{item-id}/children` |
| Fornecer `{user-id}` E `{item-id}` E `enable-file-upload` | Files.Read, Files.Read.All, Sites.Read.All, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All | `GET /users/{user-id}/drive/items/{item-id}/children` <br /> `PUT /users/{user-id}/drive/items/{item-id}:/{filename}:/content` <br /> `POST /users/{user-id}/drive/items/{item-id}:/{filename}:/createUploadSession` |
| Fornecer `{drive-id}` AND `{item-path}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /drives/{drive-id}/root:/{item-path}:/children` |
| Fornecer `{drive-id}` E `{item-path}` E `enable-file-upload` | Files.Read, Files.Read.All, Sites.Read.All, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All | `GET /drives/{drive-id}/root:/{item-path}:/children` <br /> `PUT /drives/{drive-id}/root:/{item-path}/{filename}:/content` <br /> `POST /drives/{drive-id}/root:/{item-path}/{filename}:/createUploadSession` |
| Fornecer `{group-id}` AND `{item-path}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /groups/{group-id}/root:/{item-path}:/children` |
| Fornecer `{group-id}` E `{item-path}` E `enable-file-upload` | Files.Read, Files.Read.All, Sites.Read.All, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All | `GET /groups/{group-id}/root:/{item-path}:/children` <br /> `PUT /groups/{group-id}/root:/{item-path}/{filename}:/content` <br /> `POST /groups/{group-id}/root:/{item-path}/{filename}:/createUploadSession` |
| Fornecer `{site-id}` AND `{item-path}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /sites/{site-id}/root:/{item-path}:/children` |
| Fornecer `{site-id}` E `{item-path}` E `enable-file-upload` | Files.Read, Files.Read.All, Sites.Read.All, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All | `GET /sites/{site-id}/root:/{item-path}:/children` <br /> `PUT /sites/{site-id}/root:/{item-path}/{filename}:/content` <br /> `POST /sites/{site-id}/root:/{item-path}/{filename}:/createUploadSession` |
| Fornecer `{user-id}` AND `{item-path}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /users/{user-id}/root:/{item-path}:/children` |
| Fornecer `{user-id}` E `{item-path}` E `enable-file-upload` | Files.Read, Files.Read.All, Sites.Read.All, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All | `GET /users/{user-id}/root:/{item-path}:/children` <br /> `PUT /users/{user-id}/root:/{item-path}/{filename}:/content` <br /> `POST /users/{user-id}/root:/{item-path}/{filename}:/createUploadSession` |
| Fornecer somente `{item-path}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /me/drive/root:/{item-path}:/children` |
| Fornecer somente `{item-path}` AND `enable-file-upload` | Files.Read, Files.Read.All, Sites.Read.All, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All | `GET /me/drive/root:/{item-path}:/children` <br /> `PUT /me/drive/root:/{item-path}/{filename}:/content` <br /> `POST /me/drive/root:/{item-path}/{filename}:/createUploadSession` |
| `insight-type` é definido como tendência | Sites.Read.All | `GET /me/insights/trending` |
| Fornecer `{user-id or upn}` AND está definido `insight-type` como `trending` | Sites.Read.All | `GET /users/{id or userPrincipalName}/insights/trending` |
| `insight-type` está definido como `used` | Sites.Read.All | `GET /me/insights/used` |
| Fornecer `{user-id or upn}` AND está definido `insight-type` como `used` | Sites.Read.All | `GET /users/{id or userPrincipalName}/insights/used` |
| `insight-type` é definido como compartilhado | Sites.Read.All | `GET /me/insights/shared` |
| Fornecer `{user-id or upn}` AND está definido `insight-type` como `shared` | Sites.Read.All | `GET /users/{id or userPrincipalName}/insights/shared?$filter=((lastshared/sharedby/id eq '${user-id}') and (resourceReference/type eq 'microsoft.graph.driveItem'))` |

## <a name="events"></a>Events

Evento | Quando é emitido | Dados personalizados | Cancelável | Bolhas | Funciona com modelo personalizado
------|-------------------|--------------|:-----------:|:---------:|:---------------------------:|
`itemClick` | Disparado quando o usuário clica em um arquivo. | Arquivo [selecionado](/graph/api/resources/driveItem) | Não | Não | Sim, com modelo de **arquivo** personalizado

Para obter mais informações sobre como lidar com eventos, consulte [eventos](../customize-components/events.md).

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
