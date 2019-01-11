---
title: tipo de recurso de programControl
description: No Windows Azure AD access analisa o recurso, o objeto de controle do programa representa um controle, vinculando uma revisão de acesso a um programa.
localization_priority: Normal
ms.openlocfilehash: ddf6e978277ca1801f9126597ac4b3561fe5bfb7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817819"
---
# <a name="programcontrol-resource-type"></a>tipo de recurso de programControl

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

No recurso de [acesso analisa](accessreviews-root.md) Azure AD, o objeto de controle do programa representa um controle, vinculando uma revisão de acesso a um programa.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Criar programControl](../api/programcontrol-create.md) |     [programControl](programcontrol.md) |   Adicione um programControl a um programa.|
|[Excluir programControl](../api/programcontrol-delete.md) |     Nenhum.   |   Remova um programControl de um programa.|
|[Lista programControls](../api/programcontrol-list.md) | coleção [programControl](programcontrol.md)| Controles de lista com todos os programas no inquilino.|

## <a name="permissions"></a>Permissions

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | ProgramControl.Read.All, ProgramControl.ReadWrite.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo                            | Sem suporte. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| `id`                     |`String`                | O identificador atribuído pelo recurso do vínculo entre o programa e controle                                      |
| `programId`              |`String`                | O programId do programa esse controle é parte do. Necessários na criação.                            |
| `controlId`              |`String`                | ControlId do controle, em especial o identificador de uma revisão de acesso. Necessários na criação.                                                |
| `controlTypeId`          |`String`                | O programControlType identifica o tipo de controle do programa - por exemplo, um controle de vinculação para o acesso de convidado analisa. Necessários na criação. |
| `displayName`            |`String`                | O nome do controle.                                                             |
| `status`                 |`String`                | O status do ciclo de vida do controle.                                                 |
| `createdDateTime`        |`DateTimeOffset`        | A data de criação e a hora do controle programa.                                        |
| `owner`                  |[userIdentity](useridentity.md)   | O usuário que criou o controle de programa.                                               |
| `resource`               |`programResource`       | O recurso, um grupo ou um aplicativo alvo de revisão de acesso do controle este programa.                   |

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
| `program`                |[programa](program.md)               | O programa esse controle faz parte do.                                                |

## <a name="see-also"></a>Confira também

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Lista programControls de um programa](../api/program-listcontrols.md) |      coleção [programControl](programcontrol.md)| Obter uma coleção dos controles de um programa.|
|[Lista programControlTypes](../api/programcontroltype-list.md) | coleção [programControlType](programcontroltype.md)| Lista os tipos de controle do programa. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.programControl"
}-->

```json
{
 "id": "string (identifier)",
 "programId": "string (identifier)",
 "controlId": "string (identifier)",
 "controlTypeId": "string (identifier)",
 "displayName": "string",
 "status": "string",
 "createdDateTime": "string (timestamp)",
 "owner": "microsoft.graph.userIdentity",
 "resource":"microsoft.graph.programResource"
}

```

## <a name="the-programresource-complex-type"></a>O tipo de programResource complexo

O recurso de programa, contido em um objeto de controle de programa, é uma representação de uma referência a um objeto que é o destino da revisão acesso.

Esse tipo de herda de `microsoft.graph.identity` e tem uma propriedade adicional:

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| `type`               |`String`  | Tipo de recurso, indicando se ele é um grupo ou um aplicativo. |     


<!-- {
  "type": "#page.annotation",
  "description": "programControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
