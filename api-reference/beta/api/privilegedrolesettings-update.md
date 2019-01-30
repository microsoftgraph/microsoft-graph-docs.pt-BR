---
title: Atualizar privilegedRoleSettings
description: Atualize as configurações de função para a configuração de determinada função. Um objeto privilegedRoleSettings será retornado.
localization_priority: Normal
ms.openlocfilehash: 09464c878c76ed557f30d0eac21e0572fae05062
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641117"
---
# <a name="update-privilegedrolesettings"></a>Atualizar privilegedRoleSettings

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as configurações de função para a configuração de determinada função. Um objeto [privilegedRoleSettings](../resources/privilegedrolesettings.md) será retornado.
## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

>**Observação:** O solicitante deve ter uma das seguintes funções: leitor de segurança, Administrador Global, administrador de segurança ou administrador com privilégios de função. 

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante) | PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All    |
|Delegada (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
PUT /privilegedRoles/{id}/settings
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome      |Descrição|
|:----------|:----------|
| Autorização  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON de um objeto [privilegedRoleSettings](../resources/privilegedrolesettings.md) .

A tabela a seguir lista as propriedades que você pode fornecer ao atualizar uma configuração de função.

|Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|elevationDuration|duration|A duração quando a função for ativada. Obrigatório.|
|id|string|O identificador exclusivo para as configurações de função. Somente leitura. Obrigatório.|
|isMfaOnElevationConfigurable|boolean|**true** se mfaOnElevation é configurável. **false** se mfaOnElevation não é configurável. Obrigatório.|
|lastGlobalAdmin|Booliano|Apenas para uso interno.|
|maxElavationDuration|duration|Duração máxima para a função ativada. Obrigatório.|
|mfaOnElevation|Booliano|**true** se MFA é necessária para ativar a função. **false** se MFA não é necessário para ativar a função. Obrigatório.|
|minElevationDuration|duration|Duração mínima para a função ativada. Obrigatório.|
|notificationToUserOnElevation|Booliano|**True** se enviar notificação ao usuário final quando a função é ativada. **False** se não enviar notificação quando a função é ativada. Obrigatório.|
|ticketingInfoOnElevation|Booliano|**true** se as informações de tickets são necessária quando ativar a função. **false** se as informações de tickets não são necessária quando ativar a função. Obrigatório.|
|approvalOnElevation|Booliano|**true** se a aprovação é necessária quando ativar a função. **false** se a aprovação não é necessária quando ativar a função. Obrigatório.|
|approverIds|array|Lista de IDs de aprovação, se a aprovação é necessária para a ativação.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

Observe que o inquilino deve ser registrado no PIM. Caso contrário, será retornado o código de status HTTP 403-Proibido.
## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
<!-- {
  "blockType": "request",
  "name": "put_privilegedrolesettings"
}-->
```http
PUT https://graph.microsoft.com/beta/privilegedRoles/{id}/settings
Content-type: application/json

{
    "id": "9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3",
    "elevationDuration": "PT8H",
    "notificationToUserOnElevation": false,
    "ticketingInfoOnElevation": true,
    "mfaOnElevation": false,
    "maxElavationDuration": "PT0S",
    "minElevationDuration": "PT0S",
    "lastGlobalAdmin": false,
    "isMfaOnElevationConfigurable": true,
    "approvalOnElevation": false,
    "approverIds": ["e2b2a2fb-13d7-495c-adc9-941fe966793f", "22770e3f-b9b4-418e-9dea-d0e3d2f275dd"]
}
```
##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta.

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update privilegedRoleSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedrolesettings-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
