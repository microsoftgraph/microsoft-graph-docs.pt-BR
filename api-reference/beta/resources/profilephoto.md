---
title: Tipo de recurso de profilePhoto
description: Exibe uma foto de perfil de um usuário, grupo, equipe ou contato do Outlook acessado do Exchange Online ou do Azure Active Directory (Azure AD).
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: people
author: kevinbellinger
ms.openlocfilehash: da5690ed1d0d82694c3de41ef9409eb2403a7b4b
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856397"
---
# <a name="profilephoto-resource-type"></a>Tipo de recurso de profilePhoto

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Exibe uma foto de perfil de um usuário, grupo, equipe ou contato do Outlook acessado do Exchange Online ou do Azure Active Directory (Azure AD). Os dados são binários e não são codificados em base 64.

Os tamanhos com suporte de fotos HD em Exchange Online são os seguintes: `48x48`, , , `96x96`, `120x120`, `240x240`, `360x360`, ,`432x432``504x504` e `648x648`. `64x64` Em Azure AD, as fotos podem ser de qualquer dimensão.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Get profilePhoto](../api/profilephoto-get.md) | [profilePhoto](profilephoto.md) |Obtenha a **profilePhoto** específica ou seus metadados (propriedades **profilePhoto**). |
|[Atualizar profilePhoto](../api/profilephoto-update.md) | [profilePhoto](profilephoto.md)  |Atribua uma foto ao usuário, grupo, equipe ou contato especificado. A foto deve estar em formato binário. Ela substitui a foto existente, se houver. |

> [!NOTE]
> Atualmente, não há suporte para o gerenciamento de fotos dos usuários usando o Microsoft API do Graph em locatários Azure AD B2C.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|cadeia de caracteres|Somente leitura.|
|height|int32|A altura da foto. Somente leitura.|
|width|int32|A largura da foto. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.profilePhoto"
}-->

```json
{
  "id": "String",
  "height": 240,
  "width": 240
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "profilePhoto resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


