---
title: 'bloco de anotações: getNotebookFromWebUrl'
description: Recupere as propriedades e os relacionamentos de um objeto Notebook usando seu caminho de URL.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: b5067f50b1e03c124af8323709fc7b3f70af871b
ms.sourcegitcommit: 3615f9475d57bfbb3a8c4402af863897f592dfbd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2019
ms.locfileid: "30789645"
---
# <a name="notebook-getnotebookfromweburl"></a>bloco de anotações: getNotebookFromWebUrl

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere as propriedades e os relacionamentos de um objeto [Notebook](../resources/notebook.md) usando seu caminho de URL.

O local pode ser blocos de anotações de usuário no Office 365, em blocos de anotações de grupo ou em blocos de anotações de equipe hospedados no site do SharePoint no Office 365.
## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Notes. Create, Notes. Read, Notes. ReadWrite, Notes. Read. All, Notes. ReadWrite. All    |
|Aplicativo | Notes.Read.All, Notes.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/GetNotebookFromWebUrl
POST /users/{id | userPrincipalName}/onenote/notebooks/GetNotebookFromWebUrl
POST /groups/{id}/onenote/notebooks/GetNotebookFromWebUrl
POST /sites/{id}/onenote/notebooks/GetNotebookFromWebUrl
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Tipo | Descrição|
|:-----------|:------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |
| Aceitar | string | `application/json` |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do caminho de URL completo para o bloco de anotações que você deseja recuperar.

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| `webUrl`     |`String`     | O caminho da URL do bloco de anotações a ser recuperado. Também pode conter um prefixo "OneNote:".|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [Notebook](../resources/notebook.md) no corpo da resposta.
## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
<!-- {
  "blockType": "request",
  "name": "notebook_fromweburl"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/notebooks/GetNotebookFromWebUrl
Content-type: application/json

{"webUrl":"webUrl value"}
```
##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. 

>**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json; odata.metadata=minimal
Content-Length: 544

{
    "isDefault": true,
    "userRole": "userRole-value",
    "isShared": true,
    "sectionsUrl": "sectionUrl-value",
    "sectionGroupsUrl": "sectionGroupUrl-value",
    "links": {
        "oneNoteClientUrl": {
            "href": "href-value"
        },
        "oneNoteWebUrl": {
            "href": "href-value"
        }
    },
    "id": "id-value",
    "self": "self-value",
}
```
<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Error:{notebook-getnotebookfromweburl.md}:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
}-->
