---
title: Criar programControl (preterido)
description: No recurso Azure AD revisões de acesso, crie um novo objeto programControl.  Isso vincula uma revisão de acesso a um programa.
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: f1a2e919a24d71d50fe0af26dc7f766fd4c0a8d1
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2022
ms.locfileid: "65820900"
---
# <a name="create-programcontrol-deprecated"></a>Criar programControl (preterido)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

No recurso Azure AD [revisões de acesso](../resources/accessreviews-root.md), crie um novo [objeto programControl](../resources/programcontrol.md).  Isso vincula uma revisão de acesso a um programa.

Antes de fazer essa solicitação, o chamador deve ter feito isso anteriormente

- [criou um programa](program-create.md) [ou recuperou um programa](program-list.md), para ter o valor de `programId` incluir na solicitação,
- [criou uma revisão de](accessreview-create.md) acesso [ou recuperou uma revisão](accessreview-get.md) de acesso, para ter o valor de `controlId` incluir na solicitação e
- [recuperou a lista de tipos de controle de](programcontroltype-list.md) programa, para ter o valor de `controlTypeId` incluir na solicitação.


## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante)     | ProgramControl.ReadWrite.All  |
|Delegada (conta pessoal da Microsoft) | Sem suporte. |
|Application                            |  ProgramControl.ReadWrite.All  |

O usuário conectado também deve estar em uma função de diretório que permita que ele crie um **programControl**. 

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /programControls
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome         | Tipo        | Descrição |
|:-------------|:------------|:------------|
| Autorização | string | \{token\} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON de um [objeto programControl](../resources/programcontrol.md) .

A tabela a seguir mostra as propriedades que são necessárias ao criar um controle de programa.

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| `programId`              |`String`                | A programId do programa do qual esse controle se tornará parte.                             |
| `controlId`              |`String`                | A controlId do controle, em particular o identificador de uma revisão de acesso.                                                |
| `controlTypeId`          |`String`                | O programControlType identifica o tipo de controle de programa – por exemplo, um controle vinculado a revisões de acesso de convidado. |

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código `201, Created` de resposta e um [objeto programControl](../resources/programcontrol.md) no corpo da resposta.


## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
No corpo da solicitação, forneça uma representação JSON do [objeto programControl](../resources/programcontrol.md) .


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_programControl_from_programControls"
}-->
```http
POST https://graph.microsoft.com/beta/programControls
Content-type: application/json

{
    "controlId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
    "controlTypeId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "programId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-programcontrol-from-programcontrols-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-programcontrol-from-programcontrols-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-programcontrol-from-programcontrols-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-programcontrol-from-programcontrols-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-programcontrol-from-programcontrols-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-programcontrol-from-programcontrols-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.programControl"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "63b2302c-7e62-43b7-aefb-063ba5bdb853",
  "controlId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
  "programId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
  "controlTypeId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
  "displayName": "test",
  "status": "Active",
  "createdDateTime": "2018-05-18T20:26:05.2976279Z"
}
```

## <a name="see-also"></a>Confira também

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar programControlTypes](../api/programcontroltype-list.md) | [coleção programControlType](../resources/programcontroltype.md)| Listar tipos de controle de programa. |


<!--
{
  "type": "#page.annotation",
  "description": "Create programControl",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


