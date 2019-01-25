---
title: 'driveItem: visualização'
description: Essa ação permite que você obtenha URLs incorporáveis temporários e para um item para processar uma visualização temporária.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5a49a05e1e01616bc9bbbb713fd05805d9af3070
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508535"
---
# <a name="driveitem-preview"></a>driveItem: visualização

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Essa ação permite que você obtenha URLs incorporáveis temporários e para um item para processar uma visualização temporária.

Se você quiser obter links incorporável vida útil longa, use o [createLink][] API.

> **Observação:** Atualmente, a ação de **visualização** só está disponível no SharePoint e o OneDrive for Business.

[createLink]: driveitem-createlink.md

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)
|:---------------------------------------|:-------------------------------------------
| Delegado (conta corporativa ou de estudante)     | Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All
| Delegado (conta pessoal da Microsoft) | Files.Read, Files.ReadWrite, Files.ReadWrite.All
| Aplicativo                            | Sem suporte.

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a>Corpo da solicitação

O corpo da solicitação define as propriedades da URL incorporável está solicitando o seu aplicativo.
A solicitação deve ser um objeto JSON com as seguintes propriedades.

|   Nome      |  Tipo         | Descrição
|:------------|:--------------|:-----------------------------------------------
| Visualizador      | string        | Opcional. Aplicativo de visualização para usar. `onedrive` ou `office`. Se for null, um visualizador adequado será escolhido automaticamente.
| sem cromo  | booliano       | Opcional. Se `true` (padrão), o modo de exibição incorporado não incluirá todos os controles.
| AllowEdit   | booliano       | Opcional. Se `true`, o arquivo pode ser editado da interface do usuário incorporado.
| página        | número de sequência de caracteres / | Opcional. Número de página do documento para iniciar em, se aplicável. Especificado como cadeia de caracteres para uso futuro casos em torno de tipos de arquivo como ZIP.
| zoom        | number        | Opcional. Amplie o nível para iniciar em, se aplicável.

## <a name="response"></a>Resposta

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

A resposta será um objeto JSON que contém as seguintes propriedades:

| Nome           | Tipo   | Descrição
|:---------------|:-------|:---------------------------------------------------
| getUrl         | string | URL adequada para incorporação usando HTTP GET (iframes, etc.)
| postUrl        | string | URL adequada para incorporação usando POST HTTP (formulário post, JS, etc.)
| postParameters | string | Parâmetros de POSTAGEM para incluir se usando postUrl

GetUrl, postUrl ou ambos podem ser retornados dependendo do estado atual do suporte de embed para as opções especificadas.

postParameters é uma cadeia de caracteres formatada como `application/x-www-form-urlencoded`, e se realizar uma POSTAGEM para o postUrl o tipo de conteúdo deve ser definida adequadamente. Por exemplo:
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="viewers"></a>Visualizadores

Os seguintes valores são permitidos para o parâmetro do **Visualizador** .

| Valor do tipo | Descrição
|:-----------|:----------------------------------------------------------------
| Null
     | Escolhe um aplicativo apropriado para o arquivo de renderização. Na maioria dos casos isso usará o `onedrive` visualizador, mas pode variar por tipo de arquivo.
| `onedrive` | Use o aplicativo de pré-visualização OneDrive para processá-lo.
| `office`   | Use o WAC (Office online) para processá-lo. Só é válido para documentos do Office.

### <a name="chrome-vs-chromeless"></a>Chrome versus sem cromo

Se `chromeless` for true, a visualização será um processamento bare do arquivo.
Caso contrário, pode haver adicionais barras de ferramentas/botões exibidos para interagir com a exibição de documentos.

### <a name="viewedit"></a>Exibir/editar

Se `allowEdit` for true, o documento pode ser modificado pelo interação do usuário com a visualização incorporada.
Esse recurso pode não estar disponível para todos os aplicativos de visualização ou tipos de arquivo.

### <a name="pagezoom"></a>Página/zoom

O `page` e `zoom` opções podem não estar disponíveis para todos os aplicativos de visualização, mas serão aplicadas se o aplicativo de visualização lhe fornecer apoio.
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-preview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
