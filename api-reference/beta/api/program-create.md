---
title: Criação de programa
description: No Windows Azure AD para acessar o recurso de revisões, crie um novo objeto de programa.
localization_priority: Normal
ms.openlocfilehash: a6e9ab300cf44a2f3973c468679af7fa48262680
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521296"
---
# <a name="create-program"></a>Criação de programa

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso [acesso analisa](../resources/accessreviews-root.md) Azure AD, cria um novo objeto de [programa](../resources/program.md) .
## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | `ProgramControl.ReadWrite.All`.  O usuário conectado também deve ser uma função de diretório que permite a atualização-los para criar um programa. |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo                            | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /programs
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome         | Tipo        | Descrição |
|:-------------|:------------|:------------|
| Autorização | string | Token de portador Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON de um objeto de [programa](../resources/program.md) .

A tabela a seguir mostra as propriedades que são necessárias quando você criar um programa.

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  O nome do programa.                   |
| `description`               |`String`                              |  A descrição do programa.           |


## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `201, Created` objeto de [programa](../resources/program.md) e código de resposta no corpo da resposta.

## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
No corpo da solicitação, fornece uma representação JSON do objeto de [programa](../resources/program.md) .

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

##### <a name="response"></a>Resposta
>**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.
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
|[Lista de programas](program-list.md) | coleção de [programa](../resources/program.md)|  Obtenha uma coleção de todos os programas.|
|[Lista programControls de um programa](program-listcontrols.md) |     coleção [programControl](../resources/programcontrol.md)|    Obter uma coleção dos controles de um programa.|
|[Programa de atualização](program-update.md) |  [programa](../resources/program.md)| Atualize um programa.|
|[Criar programControl](programcontrol-create.md) |        [programControl](../resources/programcontrol.md)    |   Adicione um programControl a um programa.|

<!--
{
  "type": "#page.annotation",
  "description": "Create program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/program-create.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
