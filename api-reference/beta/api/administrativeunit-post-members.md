---
title: Adicionar um membro
description: Use esta API para adicionar um membro (usuário ou grupo) a uma unidade administrativa.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a86fc2eaccb318164b91b8101577b4e3ffd64fbe
ms.sourcegitcommit: 27e8ddb53b699f70b676c9648db8f06bb8d831a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/27/2019
ms.locfileid: "35918010"
---
# <a name="add-a-member"></a>Adicionar um membro

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Use esta API para adicionar um membro (usuário ou grupo) a uma unidade administrativa.

`NOTE: Currently it's only possible to add one member at a time to an administrative unit.`

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).


|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | AdministrativeUnit. ReadWrite. All, Directory. AccessAsUser. All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | AdministrativeUnit. ReadWrite. All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome      |Descrição|
|:----------|:----------|
| Autorização  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON de um [usuário](../resources/user.md), [grupo](../resources/group.md) ou [directoryobject](../resources/directoryobject.md) a ser adicionado.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.

## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.

```http
POST https://graph.microsoft.com/beta/administrativeUnits/{id}/members/$ref
Content-type: application/json
Content-length: 109

{
  "@odata.id":"https://graph.microsoft.com/beta/groups/{id}"
}

```
No corpo da solicitação, forneça uma representação JSON do `id` objeto [User](../resources/user.md) ou [Group](../resources/group.md) que você deseja adicionar.

##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta.
 
```http
HTTP/1.1 204 No Content
```
