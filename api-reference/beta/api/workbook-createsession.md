---
title: Criar sessão
description: 'Crie uma nova sessão de workbook. '
author: lumine2008
ms.localizationpriority: medium
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 8175bc48847aaa4349b6b2b1f44950b396bdaa3b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59076135"
---
# <a name="create-session"></a>Criar sessão

Namespace: microsoft.graph

Crie uma nova sessão de workbook. 

As APIs do Excel podem ser chamadas em um destes dois modos: 

1. Sessão persistente – Todas as alterações feitas na pasta de trabalho são persistentes (salvas). Este é o modo normal de operação. 
2. Sessão não persistente – As alterações feitas pela API não são salvas na localização de origem. Em vez disso, o servidor back-end do Excel mantém uma cópia temporária do arquivo que reflete as alterações feitas durante essa sessão de API específica. Quando a sessão do Excel expirar, as alterações serão perdidas. Esse modo é útil para aplicativos que precisam fazer uma análise ou obter os resultados de um cálculo ou de uma imagem de gráfico, mas não afeta o estado do documento.   

Para representar a sessão na API, use o cabeçalho `workbook-session-id: {session-id}`. 

>**Observação:** o cabeçalho de sessão não é obrigatório para uma API do Excel funcionar. No entanto, recomendamos que você use o cabeçalho de sessão para melhorar o desempenho. Se você não usar um cabeçalho de sessão, as alterações feitas durante a chamada à API _serão_ mantidas como persistentes no arquivo.  

Em alguns casos, criar uma nova sessão requer um tempo indeterminado para ser concluído. A Microsoft Graph também fornece um padrão de operações em execução longa. Esse padrão fornece uma maneira de sondar atualizações de status de criação, sem aguardar a conclusão da criação. Veja a seguir as etapas:

1. Um `Prefer: respond-async` header é adicionado à solicitação para indicar que é uma operação de longa duração.
2. A resposta retorna um `Location` header para especificar a URL para sondar o status da operação de criação. Você pode obter o status da operação acessando a URL especificada. O status será um dos seguintes: `notStarted` , `running` , ou `succeeded` `failed` .
3. Depois que a operação é concluída, você pode solicitar o status novamente e a resposta mostrará ou `succeeded` `failed` .

### <a name="error-handling"></a>Tratamento de erros

Essa solicitação poderá, ocasionalmente, receber uma mensagem de erro HTTP 504. A resposta apropriada para esta mensagem de erro é repetir a solicitação.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Files.ReadWrite    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/createSession
POST /me/drive/root:/{item-path}:/workbook/createSession
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Descrição|
|:---------------|:----------|
| Autorização  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON do [objeto WorkbookSessionInfo.](../resources/workbooksessioninfo.md)

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de `201 Created` resposta e um objeto [workbookSessionInfo](../resources/workbooksessioninfo.md) no corpo da resposta. Para uma operação de longa duração, ele retorna um código de resposta e um `202 Accepted ` `Location` header com um corpo vazio na resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-basic-session-creation"></a>Exemplo 1: Criação de sessão básica
#### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_excel_session"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/createSession
Content-type: application/json
Content-length: 52

{
  "persistChanges": true
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-excel-session-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-excel-session-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-excel-session-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-excel-session-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Resposta

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade. 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookSessionInfo"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "persistChanges": true
}
```
### <a name="example-2-session-creation-with-long-running-operation-pattern"></a>Exemplo 2: Criação de sessão com padrão de operação de longa duração

#### <a name="request"></a>Solicitação

```http
POST https://graph.microsoft.com/beta/me/drive/items/{drive-item-id}/workbook/worksheets({id})/createSession
Prefer: respond-async
Content-type: application/json
{
    "persistChanges": true
}
```

#### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade. 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookSessionInfo"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/operations/{operation-id}
Content-type: application/json
{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


