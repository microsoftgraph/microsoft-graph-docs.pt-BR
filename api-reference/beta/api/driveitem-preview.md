---
title: 'driveItem: visualização'
description: Esta ação permite que você obtenha URLs que podem ser inseridas de curta duração em um item para renderizar uma visualização temporária.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5a49a05e1e01616bc9bbbb713fd05805d9af3070
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454367"
---
# <a name="driveitem-preview"></a>driveItem: visualização

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Esta ação permite que você obtenha URLs que podem ser inseridas de curta duração em um item para renderizar uma visualização temporária.

Se você quiser obter links incorporáveis de longa duração, use a API [CreateLink][] em vez disso.

> **Observação:** No momento, a ação de **Visualização** só está disponível no SharePoint e no onedrive for Business.

[createLink]: driveitem-createlink.md

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)
|:---------------------------------------|:-------------------------------------------
| Delegado (conta corporativa ou de estudante)     | Files. Read, files. ReadWrite, files. ReadWrite. All, sites. ReadWrite. All
| Delegado (conta pessoal da Microsoft) | Files. Read, files. ReadWrite, files. ReadWrite. All
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

O corpo da solicitação define as propriedades da URL incorporável que seu aplicativo está solicitando.
A solicitação deve ser um objeto JSON com as seguintes propriedades.

|   Name      |  Tipo         | Descrição
|:------------|:--------------|:-----------------------------------------------
| visor      | string        | Opcional. Aplicativo de visualização a ser usado. `onedrive` ou `office`. Se for NULL, um visualizador adequado será escolhido automaticamente.
| Não Chrome  | booliano       | Opcional. Se `true` (padrão), o modo de exibição incorporado não incluirá nenhum controle.
| allowEdit   | booliano       | Opcional. Se `true`, o arquivo pode ser editado a partir da interface do usuário incorporada.
| page        | Cadeia de caracteres/número | Opcional. Número de página do documento para iniciar em, se aplicável. Especificado como cadeia de caracteres para casos de uso futuros em relação a tipos de arquivo como ZIP.
| zoom        | number        | Opcional. Nível de zoom para iniciar em, se aplicável.

## <a name="response"></a>Resposta

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

A resposta será um objeto JSON que contém as seguintes propriedades:

| Name           | Tipo   | Descrição
|:---------------|:-------|:---------------------------------------------------
| getUrl         | string | URL adequada para incorporação usando HTTP GET (IFrames, etc.)
| postUrl        | string | URL adequada para incorporação usando HTTP POST (Form Post, JS, etc.)
| postparameters | string | LANÇAR parâmetros para incluir se estiver usando postUrl

GetUrl, postUrl ou ambos podem ser retornados, dependendo do estado atual do suporte de embed para as opções especificadas.

postparameters é uma cadeia de caracteres `application/x-www-form-urlencoded`formatada como e, se estiver executando uma postaGem no postUrl, o tipo de conteúdo deve ser definido de acordo. Por exemplo:
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="viewers"></a>Visualizadores

Os valores a seguir são permitidos para o parâmetro **Viewer** .

| Valor do tipo | Descrição
|:-----------|:----------------------------------------------------------------
| vazio     | Escolhe um aplicativo apropriado para renderizar o arquivo. Na maioria dos casos, isso usará o visualizador, mas pode variar de acordo com o tipo de `onedrive` arquivo.
| `onedrive` | Use o aplicativo de visualização do OneDrive para renderizar o arquivo.
| `office`   | Use o WAC (Office Online) para renderizar o arquivo. Só é válido para documentos do Office.

### <a name="chrome-vs-chromeless"></a>Cromado vs não monocromático

Se `chromeless` for true, a visualização será uma renderização Bare do arquivo.
Caso contrário, poderão existir barras de ferramentas/botões adicionais exibidos para interagir com o documento/modo de exibição.

### <a name="viewedit"></a>Exibir/editar

Se `allowEdit` for true, o documento poderá ser modificado pela interação do usuário com a visualização incorporada.
Esse recurso pode não estar disponível para todos os aplicativos de visualização ou tipos de arquivo.

### <a name="pagezoom"></a>Página/zoom

As `page` opções `zoom` e podem não estar disponíveis para todos os aplicativos de visualização, mas serão aplicadas se o aplicativo de visualização oferecer suporte a ela.
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-preview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
