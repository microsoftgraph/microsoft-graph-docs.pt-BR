---
title: tipo de recurso do programa
description: 'No Windows Azure AD access analisa o recurso, um programa é um contêiner, mantendo os controles de programa. Um locatário pode ter um ou mais programas.  Cada controle vincula uma revisão de acesso a um programa, para torná-la mais fáceis de localizar relacionados access analisa.  '
localization_priority: Normal
ms.openlocfilehash: a342fd159bba3f7e31c55ffab9a64a72353bc7ac
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863900"
---
# <a name="program-resource-type"></a>tipo de recurso do programa

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

No recurso de [acesso analisa](accessreviews-root.md) Azure AD, um programa é um contêiner, mantendo os controles de programa. Um locatário pode ter um ou mais programas.  Cada controle vincula uma revisão de acesso a um programa, para torná-la mais fáceis de localizar relacionados access analisa.  

Cada locatário que tem em-hospedados Azure AD avaliações de acesso tem um programa, `Default program`.  Um administrador global pode criar programas adicionais, por exemplo representar as iniciativas de conformidade. 


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Criação de programa](../api/program-create.md) |   [programa](program.md)   |   Crie um novo programa.|
|[Excluir programa](../api/program-delete.md) |   Nenhum.   |   Exclua um programa.|
|[Lista de programas](../api/program-list.md) |  coleção de [programa](program.md)|   Obtenha uma coleção de todos os programas.|
|[Lista programControls de um programa](../api/program-listcontrols.md) |      coleção [programControl](programcontrol.md)| Obter uma coleção dos controles de um programa.|
|[Programa de atualização](../api/program-update.md) |   [programa](program.md)|  Atualize um programa.|

## <a name="permissions"></a>Permissions

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | ProgramControl.Read.All, ProgramControl.ReadWrite.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo                            | Sem suporte. |


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| `id`                        |`String`                              |  O identificador atribuído pelo recurso do programa.                    |
| `displayName`               |`String`                              |  O nome do programa.  Necessários na criação.                  |
| `description`               |`String`                              |  A descrição do programa.           |

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
| `controls`                  |[programControl](programcontrol.md) | Controles associados com o programa. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.program"
}-->

```json
{
 "id": "string (identifier)",
 "displayName": "string",
 "description": "string"
}

```

<!-- {
  "type": "#page.annotation",
  "description": "program resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
