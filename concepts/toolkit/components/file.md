---
title: Componente de arquivo no Microsoft Graph Toolkit
description: O componente de arquivo é usado para exibir um arquivo mostrando o ícone e o nome
localization_priority: Normal
author: beth-panx
ms.openlocfilehash: 314f08d396421c3b0afe0cf049e91cca9daa03fd
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579790"
---
# <a name="file-component-in-the-microsoft-graph-toolkit"></a>Componente de arquivo no Microsoft Graph Toolkit

O componente File é usado para representar um [arquivo/pasta](/graph/onedrive-concept-overview) individual do OneDrive ou SharePoint exibindo informações como o nome do arquivo/pasta, um ícone que indica o tipo de arquivo e outras propriedades, como o autor, data da última modificação ou outros detalhes. Você pode fornecer os identificadores de um arquivo e o componente gerará a consulta para recuperar o arquivo com base nos identificadores fornecidos. Esse componente pode ser usado por conta própria ou como parte dos [componentes mgt-file-list.](./file-list.md)

## <a name="example"></a>Exemplo

O exemplo a seguir exibe um arquivo usando o `mgt-file` componente. Você pode usar o editor de código para ver como as [propriedades](#properties) alteram o comportamento do componente.

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-file--file&source=docs" height="250"></iframe>

[Abra este exemplo em mgt.dev](https://mgt.dev/?path=/story/components-mgt-file--file&source=docs)

## <a name="properties"></a>Propriedades

Você pode usar várias propriedades para personalizar o componente.

| Atributo | Propriedade | Descrição |
| --------- | -------- | ----------- |
| file-query | fileQuery | A consulta completa ou o caminho para o arquivo a ser recuperado. |
| drive-id | driveId | A ID da unidade à que o arquivo pertence. Também deve fornecer um `item-id` ou `item-path` . |
| group-id | groupId | ID do grupo ao que o arquivo pertence. Também deve fornecer um `item-id` ou `item-path` . |
| site-id | siteId | ID do site ao que o arquivo pertence. Também deve fornecer um `{item-id}` ou `{item-path}` . Forneça o `{list-id}` também se você estiver fazendo referência a um arquivo de uma lista específica. |
| list-id | listId | ID da lista à que o arquivo pertence. Também deve fornecer `{site-id}` e `{item-id}` . |
| item-id | itemId | ID do arquivo. A consulta padrão é `/me/drive/items` . Forneça `{drive-id}` , , ou para consultar um local `{group-id}` `{site-id}` `{user-id}` específico. |
| item-path | itemPath | Caminho do item do arquivo. A consulta padrão é `/me/drive/root` . Forneça `{drive-id}` , , ou para consultar um local `{group-id}` `{site-id}` `{user-id}` específico. |
| tipo de insight | insightType | Tipo de insight do qual o arquivo é recuperado. Pode `trending` ser `used` , ou `shared` . |
| insight-id | insightId | ID do recurso insight. |
| file-details | fileDetails | Definir como um objeto que representa um arquivo |
| file-icon | fileIcon | Definir como um ícone para mostrar o arquivo |
| modo de exibição | modo de exibição | Definir para controlar como o arquivo é renderizado. O padrão é `oneline`. <br>`image` - mostrar apenas o ícone <br>`oneline` - mostrar o ícone e uma linha de texto (o padrão é arquivo `name` ) <br>`twolines` - mostrar o ícone e duas linhas de texto ( `name` `lastModifiedDateTime` e por padrão)<br> `threelines` - mostrar o ícone e três linhas de texto ( `name` , e do autor por `lastModifiedDateTime` `displayName` padrão) |
| line1-property | line1Property | Define a propriedade de `fileDetails` usar para a primeira linha de texto. O padrão `name` é do arquivo. |
| line2-property | line2Property | Define a propriedade de `fileDetails` usar para a segunda linha de texto. O padrão é `lastModifiedDateTime`. |
| line3-property | line3Property | Define a propriedade de `fileDetails` usar para a terceira linha de texto. O padrão `size` é do arquivo. |

O exemplo a seguir altera o comportamento do componente para buscar dados de uma consulta específica.

```html
<mgt-file file-query="/me/drive/items/01BYE5RZZFWGWWVNHHKVHYXE3OUJHGWCT2"></mgt-file>
```

O exemplo a seguir altera o comportamento do componente para buscar dados de uma consulta específica, mostrar três linhas de informações - nome do arquivo, última data modificada e tamanho do arquivo por padrão - e definir o ícone de arquivo.

```html
<mgt-file file-query="/me/drive/items/01BYE5RZZFWGWWVNHHKVHYXE3OUJHGWCT2" view="threeLines" file-icon="ICON_PATH"></mgt-file>
```

O exemplo a seguir altera o comportamento do componente para buscar dados de uma unidade específica.

```html
<mgt-file drive-id="b!-RIj2DuyvEyV1T4NlOaMHk8XkS_I8MdFlUCq1BlcjgmhRfAj3-Z8RY2VpuvV_tpd" item-id="01BYE5RZ5MYLM2SMX75ZBIPQZIHT6OAYPB"></mgt-file>
```

O exemplo a seguir altera o behabior do componente para buscar dados de um SharePoint site e caminho.

```html
  <mgt-file site-id="m365x214355.sharepoint.com,5a58bb09-1fba-41c1-8125-69da264370a0,9f2ec1da-0be4-4a74-9254-973f0add78fd" item-Path="/DemoDocs/AdminDemo"></mgt-file>
```

O exemplo a seguir altera o comportamento do componente para buscar dados por tipo de insight.

```html
<mgt-file insight-type="shared" insight-id="AW1GxMvkOztMkJX-SCppUSRPF5EvyPDHRZVAqtQZXI4JoUXwI9_mfEWNlabr1f7aXRBWDMt2C2FDop4fP1vsUw9tRsTL5Ds7TJCV_kgqaVEkBA"></mgt-file>
```

## <a name="css-custom-properties"></a>Propriedades personalizadas CSS

O `mgt-file` componente define as seguintes propriedades personalizadas CSS.

```css
mgt-file {
  --file-type-icon-size: 28px;
  --file-border: none;
  --file-box-shadow: none;
  --file-background-color: #ffffff;

  --font-family: 'Segoe UI';
  --font-size: 14px;
  --font-weight: 400;
  --text-transform: none;
  --color: #323130;

  --line2-font-size: 12px;
  --line2-font-weight: 400;
  --line2-color: #797775;
  --line2-text-transform: none;

  --line3-font-size: 12px;
  --line3-font-weight: 400;
  --line3-color: #797775;
  --line3-text-transform: none;
}
```

Para saber mais, confira [componentes de estilo](../customize-components/style.md).

## <a name="microsoft-graph-apis-and-permissions"></a>ApIs Graph Microsoft e permissões

Esse controle usa as seguintes APIs Graph Microsoft e permissões.

| Configuração | Escopos de permissão | API |
| ------------- | ----------------- | --- |
| Desenvolvedor fornece `{drive-id}` AND `{item-id}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /drives/{drive-id}/items/{item-id}` |
| Desenvolvedor fornece `{drive-id}` AND `{item-path}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /drives/{drive-id}/root:/{item-path}` |
| Desenvolvedor fornece `{group-id}` AND `{item-id}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /groups/{group-id}/drive/items/{item-id}` |
| Desenvolvedor fornece `{group-id}` AND `{item-path}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /groups/{group-id}/drive/root:/{item-path}` |
| Desenvolvedor fornece SOMENTE `{item-id}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /me/drive/items/{item-id}` |
| Desenvolvedor fornece SOMENTE `{item-path}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /me/drive/root:/{item-path}` |
| Desenvolvedor fornece `{site-id}` AND `{item-id}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /sites/{site-id}/drive/items/{item-id}` |
| Desenvolvedor fornece `{site-id}` AND `{item-path}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /sites/{site-id}/drive/root:/{item-path}` |
| Desenvolvedor fornece `{site-id}` AND `{list-id}` AND `{item-id}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /sites/{site-id}/lists/{list-id}/items/{item-id}/driveItem` |
| Desenvolvedor fornece `{user-id}` AND `{item-id}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /users/{user-id}/drive/items/{item-id}` |
| Desenvolvedor fornece `{user-id}` AND `{item-path}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /users/{user-id}/drive/root:/{item-path}` |
| `insight-type` está definido como `trending` e o desenvolvedor fornece `{insight-id}` | Sites.Read.All | `GET /me/insights/trending/{insight-id}/resource` |
| O desenvolvedor fornece `{user-id or upn}` AND e está definido `{insight-id}` `insight-type` como `trending` | Sites.Read.All | `GET /users/{id or userPrincipalName}/insights/trending/{insight-id}/resource` |
| `insight-type` está definido como `used` e o desenvolvedor fornece `{insight-id}` | Sites.Read.All | `GET /me/insights/used/{id}/resource` |
| O desenvolvedor fornece `{user-id or upn}` AND e está definido `{insight-id}` `insight-type` como `used` | Sites.Read.All | `GET /users/{id or userPrincipalName}/insights/used/{id}/resource` |
| `insight-type` is `shared` AND developer provides `{insight-id}` | Sites.Read.All | `GET /me/insights/shared/{id}/resource` |
| O desenvolvedor fornece `{user-id or upn}` AND e está definido `{insight-id}` `insight-type` como `shared` | Sites.Read.All | `GET /users/{id or userPrincipalName}/insights/shared/{id}/resource` |

## <a name="templates"></a>Modelos

O `mgt-file` componente dá suporte a vários [modelos](../customize-components/templates.md) que permitem substituir determinadas partes do componente. Para especificar um modelo, inclua um elemento dentro de um componente e de definir o `<template>` valor como um dos `data-type` seguintes:

| Tipo de Dados | Contexto de dados | Descrição |
| ----------- | -------------- | ------------- |
| loading | nenhuma | O modelo a ser render enquanto o componente está em um estado de carregamento. |
| no-data | nenhuma | O modelo a ser renderização quando nenhum dado de arquivo estiver disponível. |
| Padrão. | file: o objeto de detalhes do arquivo | O modelo padrão substitui todo o componente por seu próprio. |

## <a name="authentication"></a>Autenticação

O controle usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md) para buscar os dados necessários.

## <a name="cache"></a>Cache

|Armazenamento de objetos|Dados armazenados em cache|Comentários|
|---------|-----------|-------|
|`driveFiles`|Lista de arquivos por id de unidade|Usado quando `driveId` é fornecido|
|`groupFiles`|Lista de arquivos por id de grupo|Usado quando `groupId` é fornecido|
|`siteFiles`|Lista de arquivos por id de site|Usado quando `siteId` é fornecido|
|`userFiles`|Lista de arquivos por ID do usuário|Usado quando `userId` é fornecido|
|`insightFiles`|Lista de arquivos por insights|Usado quando `insightType` e `insightId` são fornecidos|
|`fileQueries`|Lista de arquivos por consultas|Usado quando `fileQuery` é fornecido|

Para obter detalhes sobre como configurar o cache, [consulte Caching](../customize-components/cache.md).