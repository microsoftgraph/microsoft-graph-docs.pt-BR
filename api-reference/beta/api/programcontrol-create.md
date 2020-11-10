---
title: Criar programControl
description: No recurso de revisões do Azure AD Access, crie um novo objeto programControl.  Isso vincula uma revisão do Access a um programa.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: f5a6fd297422c946b1764626828780a0cb32643f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48967723"
---
# <a name="create-programcontrol"></a>Criar programControl

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , crie um novo objeto [programControl](../resources/programcontrol.md) .  Isso vincula uma revisão do Access a um programa.

Antes de fazer essa solicitação, o chamador deve ter sido

- [criou um programa](program-create.md) ou [recuperou um programa](program-list.md), para que o valor de `programId` a ser incluído na solicitação,
- [criou uma revisão do Access](accessreview-create.md) ou [recuperou uma revisão do Access](accessreview-get.md), para que o valor de `controlId` seja incluído na solicitação e
- [recuperada a lista de tipos de controle de programa](programcontroltype-list.md)para que o valor de `controlTypeId` seja incluído na solicitação.


## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | ProgramControl.ReadWrite.All  |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Application                            |  ProgramControl.ReadWrite.All  |

O usuário conectado também deve estar em uma função de diretório que permite que eles criem um **programControl**. 

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
No corpo da solicitação, forneça uma representação JSON de um objeto [programControl](../resources/programcontrol.md) .

A tabela a seguir mostra as propriedades que são necessárias ao criar um controle de programa.

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| `programId`              |`String`                | O ProgramId do programa para o qual esse controle se tornará parte.                             |
| `controlId`              |`String`                | O controlId do controle, em particular, o identificador de uma revisão do Access.                                                |
| `controlTypeId`          |`String`                | O programControlType identifica o tipo de controle de programa-por exemplo, um controle vinculando a revisões de acesso de convidados. |

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `201, Created` código de resposta e um objeto [programControl](../resources/programcontrol.md) no corpo da resposta.


## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [programControl](../resources/programcontrol.md) .


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

---


##### <a name="response"></a>Resposta
>**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.
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
|[Listar programControlTypes](../api/programcontroltype-list.md) | coleção [programControlType](../resources/programcontroltype.md)| Listar tipos de controle de programa. |


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


