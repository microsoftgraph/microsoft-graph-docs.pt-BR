---
title: Criar programControl
description: No Windows Azure AD para acessar o recurso de revisões, crie um novo objeto programControl.  Isso vincula uma revisão de acesso a um programa.
localization_priority: Normal
ms.openlocfilehash: 4dfbb76244a41867b8a57faa42f63dc728f59136
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851531"
---
# <a name="create-programcontrol"></a>Criar programControl

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

O recurso [acesso analisa](../resources/accessreviews-root.md) Azure AD, cria um novo objeto [programControl](../resources/programcontrol.md) .  Isso vincula uma revisão de acesso a um programa.

Antes de fazer essa solicitação, o chamador deve ter anteriormente

 - [criado um programa](program-create.md) ou [recuperados de um programa](program-list.md), para que o valor de `programId` para incluir na solicitação,
 - [criada uma revisão de acesso](accessreview-create.md) ou [recuperado uma revisão de acesso](accessreview-get.md), para que o valor de `controlId` para incluir na solicitação, e
 - [recuperou a lista de tipos de controle de programas](programcontroltype-list.md), para que o valor de `controlTypeId` para incluir na solicitação.


## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | `ProgramControl.ReadWrite.All`.  O usuário conectado também deve ser uma função de diretório que permite a atualização-los para criar um programControl. |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo                            | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /programControls
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome         | Tipo        | Descrição |
|:-------------|:------------|:------------|
| Autorização | string | Portador \{token\}. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON de um objeto [programControl](../resources/programcontrol.md) .

A tabela a seguir mostra as propriedades que são necessárias quando você criar um controle de programa.

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| `programId`              |`String`                | O programId do programa esse controle vai se tornar uma parte do.                             |
| `controlId`              |`String`                | ControlId do controle, em especial o identificador de uma revisão de acesso.                                                |
| `controlTypeId`          |`String`                | O programControlType identifica o tipo de controle do programa - por exemplo, um controle de vinculação para o acesso de convidado analisa. |

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `201, Created` código de resposta e um objeto [programControl](../resources/programcontrol.md) no corpo da resposta.


## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
No corpo da solicitação, fornece uma representação JSON do objeto [programControl](../resources/programcontrol.md) .

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
|[Lista programControlTypes](../api/programcontroltype-list.md) | coleção [programControlType](../resources/programcontroltype.md)| Lista os tipos de controle do programa. |


<!-- {
  "type": "#page.annotation",
  "description": "Create programControl",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
