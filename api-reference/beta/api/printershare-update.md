---
title: Atualizar o printershare
description: Atualize as propriedades do compartilhamento de impressora. Esse método pode ser usado para "trocar" impressoras.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 9f1ef05b9fc3aed734e5f69a920fe63cdc82c9f1
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61028031"
---
# <a name="update-printershare"></a>Atualizar o printershare

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades de um compartilhamento de impressora. Esse método pode ser usado para trocar [impressoras](../resources/printer.md).

Por exemplo, se um dispositivo de impressora física [](../resources/printer.md) quebra, um administrador pode registrar um novo dispositivo de impressora e atualizar essa [impressoraShare](../resources/printerShare.md) para apontar para a nova impressora sem exigir que os usuários tomem qualquer ação.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

Além das permissões a seguir, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa. O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)

|Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:---------------|:--------------------------------------------|
|Delegado (conta corporativa ou de estudante)| PrinterShare.ReadWrite.All |
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/shares/{id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Descrição|
|:-----------|:-----------|
| Autorização | {token} de portador. Obrigatório. |
| Content-type  | application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece os valores para campos [printerShare](../resources/printershare.md) relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.

As seguintes propriedades podem ser atualizadas: 

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|impressora|microsoft.graph.printer|A impressora à que essa impressora está relacionada. Use a sintaxe conforme mostrado no exemplo a seguir para atualizar a impressora à qual esse compartilhamento de impressora `printer@odata.bind` está associado.|
|displayName|Cadeia de caracteres|O nome do compartilhamento de impressora que os clientes de impressão devem exibir.|
|allowAllUsers|Booliano| Se for true, todos os usuários e grupos terão acesso a esse compartilhamento de impressora. Isso sobressalta as listas de permissão definidas pelas propriedades de navegação allowedUsers e allowedGroups.|

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` objeto [printerShare](../resources/printershare.md) atualizado no corpo da resposta.
## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_printershare"
}-->
```http
PATCH https://graph.microsoft.com/beta/print/shares/{id}
Content-type: application/json

{
  "displayName": "ShareName",
  "allowAllUsers": true,
  "printer@odata.bind": "https://graph.microsoft.com/beta/print/printers/{id}"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-printershare-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-printershare-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-printershare-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-printershare-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-printershare-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>Resposta
Este é um exemplo de resposta.
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printerShare"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/shares/$entity",
  "id": "d837c17b-3296-4384-a053-828d56e10f50",
  "displayName": "ShareName",
  "createdDateTime": "2020-02-04T00:00:00.0000000Z",
  "isAcceptingJobs": true,
  "allowAllUsers": true,
  "status": {
    "state": "stopped",
    "details": ["disconnected"],
    "description": ""
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update printershare",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
