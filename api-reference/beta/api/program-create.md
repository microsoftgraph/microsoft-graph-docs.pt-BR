---
title: Criar programa
description: No recurso de análises de acesso do Azure AD, crie um novo objeto de programa.
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: 1bcf52b32f4501c3fcf738ff03df0ac99e140053
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61032120"
---
# <a name="create-program"></a>Criar programa

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No recurso de análises de acesso do Azure [AD,](../resources/accessreviews-root.md) crie um novo [objeto de](../resources/program.md) programa.
## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | ProgramControl.ReadWrite.All   |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo                            | Sem suporte. |

O usuário inscreveu também deve estar em uma função de diretório que permita que ele crie um programa.

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /programs
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome         | Tipo        | Descrição |
|:-------------|:------------|:------------|
| Autorização | string | \{token\} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON de um [objeto program.](../resources/program.md)

A tabela a seguir mostra as propriedades necessárias ao criar um programa.

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  O nome do programa.                   |
| `description`               |`String`                              |  A descrição do programa.           |


## <a name="response"></a>Resposta
Se tiver êxito, este método retornará `201, Created` um código de resposta e um objeto [program](../resources/program.md) no corpo da resposta.

## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
No corpo da solicitação, fornece uma representação JSON do [objeto program.](../resources/program.md)


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_program_from_programs"
}-->
```http
POST https://graph.microsoft.com/beta/programs
Content-type: application/json

{
    "displayName": "testprogram3",
    "description": "test description"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-program-from-programs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-program-from-programs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-program-from-programs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-program-from-programs-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-program-from-programs-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.program"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
    "displayName": "testprogram3",
    "description": "test description"
}
```

## <a name="see-also"></a>Confira também

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar programas](program-list.md) | [conjunto de](../resources/program.md) programas|  Obter uma coleção de todos os programas.|
|[Listar programControls de um programa](program-listcontrols.md) |     [Coleção programControl](../resources/programcontrol.md)|    Obter uma coleção dos controles de um programa.|
|[Atualizar programa](program-update.md) |  [program](../resources/program.md)| Atualize um programa.|
|[Criar programControl](programcontrol-create.md) |        [programControl](../resources/programcontrol.md)    |   Adicione um programControl a um programa.|

<!--
{
  "type": "#page.annotation",
  "description": "Create program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


