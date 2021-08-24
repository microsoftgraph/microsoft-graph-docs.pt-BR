---
title: Criar uma configuração de grupo
description: Crie uma nova configuração, com base nos modelos disponíveis em groupSettingTemplates.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 1b2aee406f5b579691876cb88b7f999cc3679548
ms.sourcegitcommit: c6f7a931a8d83ac54f577b7bec08237fd17ce51a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/24/2021
ms.locfileid: "58490522"
---
# <a name="create-a-group-setting"></a>Criar uma configuração de grupo

Namespace: microsoft.graph

Use essa API para criar uma nova configuração, com base nos modelos disponíveis em [groupSettingTemplates](../resources/groupsettingtemplate.md). Essas configurações podem estar no nível do locatário ou no nível do grupo. A solicitação de criação deve [fornecer settingValues](../resources/settingvalue.md) para todas as configurações definidas no modelo. Para configurações específicas de grupo, somente a configuração que rege se membros de um grupo podem convidar usuários convidados podem ser definidos. Isso regerá esse comportamento quando a capacidade de adicionar usuários convidados a um grupo geralmente está disponível. Para pontos de extremidade beta, use [directorySettingTemplates](/graph/api/resources/directorysettingtemplate?view=graph-rest-beta&preserve-view=true).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).


|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /groupSettings
POST /groups/{id}/settings
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome | Descrição |
|:---------------|:----------|
| Autorização | {token} de portador. Obrigatório. |
| Content-Type | application/json |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [groupSetting](../resources/groupsetting.md). No entanto, o nome de exibição para que a configuração será definida com base no nome do modelo configurações referenciado.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna o código de resposta `201 Created` e um objeto [groupSetting](../resources/groupsetting.md) no corpo da resposta.

## <a name="example-1-create-a-new-setting-for-all-microsoft-365-groups-in-the-tenant"></a>Exemplo 1: Criar uma nova configuração para todos os grupos Microsoft 365 no locatário

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "create_groupsetting_from_groupsettings"
}-->
```http
POST https://graph.microsoft.com/v1.0/groupSettings
Content-type: application/json

{
  "displayName": "Group.Unified",
  "templateId": "62375ab9-6b52-47ed-826b-58e47e0e304b",
  "values": [
    {
      "name": "GuestUsageGuidelinesUrl",
      "value": "https://privacy.contoso.com/privacystatement"
    },
    {
      "name": "EnableMSStandardBlockedWords",
      "value": "true"
    },
    {
      "name": "EnableMIPLabels",
      "value": "true"
    },
    {
      "name": "PrefixSuffixNamingRequirement",
      "value": "[Contoso-][GroupName]"
    }
  ]
}
```

No corpo da solicitação, forneça uma representação JSON do objeto [groupSetting](../resources/groupsetting.md).

### <a name="response"></a>Resposta

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groupSettings/$entity",
  "id": "b11b99c5-f0a3-4c32-a250-548cf11cae1c",
  "displayName": "Group.Unified",
  "templateId": "62375ab9-6b52-47ed-826b-58e47e0e304b",
  "values": [
    {
      "name": "GuestUsageGuidelinesUrl",
      "value": "https://privacy.contoso.com/privacystatement"
    },
    {
      "name": "EnableMSStandardBlockedWords",
      "value": "true"
    },
    {
      "name": "EnableMIPLabels",
      "value": "true"
    },
    {
      "name": "PrefixSuffixNamingRequirement",
      "value": "[Contoso-][GroupName]"
    }
  ]
}
```

## <a name="example-2-create-a-setting-to-block-guests-for-a-specific-microsoft-365-group"></a>Exemplo 2: Criar uma configuração para bloquear convidados para um grupo Microsoft 365 específico

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "create_groupsetting_from_groupsettings_for_guests"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/055a5d18-a3a9-4338-b9c5-de92559b7ebf/settings
Content-type: application/json

{
  "displayName": "Group.Unified.Guest",
  "templateId": "08d542b9-071f-4e16-94b0-74abb372e3d9",
  "values": [
    {
      "name": "AllowToAddGuests",
      "value": "false"
    }
  ]
}
```

No corpo da solicitação, forneça uma representação JSON do objeto [groupSetting](../resources/groupsetting.md).

### <a name="response"></a>Resposta

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groupSettings/$entity",
  "id": "2a0248a2-fde9-4a80-a53e-c0141f68e03d",
  "displayName": "Group.Unified.Guest",
  "templateId": "08d542b9-071f-4e16-94b0-74abb372e3d9",
  "values": [
    {
      "name": "AllowToAddGuests",
      "value": "false"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create groupsetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

