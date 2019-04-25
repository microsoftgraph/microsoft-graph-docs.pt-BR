---
title: Atualizar privilegedRoleSettings
description: Atualize as configurações de função para a configuração de função determinada. Um objeto privilegedRoleSettings será retornado.
localization_priority: Normal
ms.openlocfilehash: 779b0d4cd61672c90c103ebb2545cb75324273fd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32538658"
---
# <a name="update-privilegedrolesettings"></a>Atualizar privilegedRoleSettings

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as configurações de função para a configuração de função determinada. Um objeto [privilegedRoleSettings](../resources/privilegedrolesettings.md) será retornado.
## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

>**Observação:** O solicitante deve ter uma das seguintes funções: administrador de função privilegiada, administrador global, administrador de segurança ou leitor de segurança. 

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | PrivilegedAccess. ReadWrite. AzureAD, Directory. AccessAsUser. All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
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
No corpo da solicitação, forneça uma representação JSON de um objeto [privilegedRoleSettings](../resources/privilegedrolesettings.md) .

A tabela a seguir lista as propriedades que você pode fornecer ao atualizar uma configuração de função.

|Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|elevationDuration|duration|A duração quando a função é ativada. Obrigatório.|
|id|string|O identificador exclusivo das configurações de função. Somente leitura. Obrigatório.|
|isMfaOnElevationConfigurable|booliano|**true** se mfaOnElevation é configurável. **false** se mfaOnElevation não é configurável. Obrigatório.|
|lastGlobalAdmin|Booliano|Apenas para uso interno.|
|maxElavationDuration|duration|Duração máxima da função ativada. Obrigatório.|
|mfaOnElevation|Booliano|**true** se a MFA é necessária para ativar a função. **false** se a MFA não é necessária para ativar a função. Obrigatório.|
|minElevationDuration|duration|Duração mínima para a função ativada. Obrigatório.|
|notificationToUserOnElevation|Booliano|**true** se enviar notificação para o usuário final quando a função é ativada. **false** se não enviar notificações quando a função for ativada. Obrigatório.|
|ticketingInfoOnElevation|Booliano|**true** se as informações de tíquete são necessárias ao ativar a função. **false** se as informações de tíquete não são necessárias ao ativar a função. Obrigatório.|
|approvalOnElevation|Booliano|**true** se a aprovação é necessária ao ativar a função. **false** se a aprovação não é necessária ao ativar a função. Obrigatório.|
|approverIds|Coleção de cadeias de caracteres|Lista de IDs de aprovação, se a aprovação for necessária para ativação.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

Observe que o locatário precisa ser registrado no PIM. Caso contrário, o código de status HTTP 403 proibido será retornado.
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
<!-- {
  "blockType": "response",
  "truncated": true
}-->
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
