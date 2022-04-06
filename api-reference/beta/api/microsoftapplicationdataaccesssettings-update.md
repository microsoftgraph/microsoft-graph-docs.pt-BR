---
title: Atualizar microsoftApplicationDataAccessSettings
description: Atualize as propriedades de um objeto microsoftApplicationDataAccessSettings.
author: ttomi
ms.localizationpriority: medium
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: d7031fefb9f90718dc0e0fb66714cb933fa9dfe9
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589541"
---
# <a name="update-microsoftapplicationdataaccesssettings"></a>Atualizar microsoftApplicationDataAccessSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as configurações em um [objeto microsoftApplicationDataAccessSettings](../resources/microsoftapplicationdataaccesssettings.md) que especificam o acesso de aplicativos Microsoft para Microsoft 365 dados do usuário em uma organização.

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|Organization.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}/settings/microsoftApplicationDataAccess
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|isEnabledForAllMicrosoftApplications|Boolean|Quando definido como `true`, todos os usuários da organização podem acessar em um aplicativo microsoft qualquer Microsoft 365 dados que o usuário tenha sido autorizado a acessar. O aplicativo microsoft pode ser um aplicativo Microsoft 365 (por exemplo, Excel, Outlook) ou um aplicativo não Microsoft 365 (por exemplo, Edge). O padrão é `true`. <br> É possível desabilitar esse acesso para um subconjunto de usuários em um grupo de segurança Azure Active Directory (Azure AD), especificando o grupo na propriedade **disabledForGroup**. <br> Quando definido como `false`, os usuários podem acessar Microsoft 365 dados autorizados somente em um Microsoft 365 aplicativo.|
|disabledForGroup|Cadeia de caracteres|A ID de um grupo de segurança do Azure AD cujos membros têm permissão para acessar Microsoft 365 dados usando apenas aplicativos Microsoft 365, mas não outros aplicativos da Microsoft, como o Edge. <br> Isso só será aplicável **se isEnabledForAllMicrosoftApplications** estiver definido como `true`.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [microsoftApplicationDataAccessSettings](../resources/microsoftapplicationdataaccesssettings.md) atualizado no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

A solicitação de exemplo a seguir mostra como um administrador atualiza a configuração de privacidade **disabledForGroup** para proibir que os usuários em um determinado grupo do Azure AD acessem dados Microsoft 365 usando aplicativos Microsoft que não fazem parte do Microsoft 365.

<!-- {
  "blockType": "request",
  "name": "update_microsoftapplicationdataaccesssettings"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/organization/{organizationId}/settings/microsoftApplicationDataAccess
Content-Type: application/json

{
  "disabledForGroup": "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
}
```

### <a name="response"></a>Resposta

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.microsoftApplicationDataAccessSettings",
  "name": "update_microsoftapplicationdataaccesssettings"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.microsoftApplicationDataAccessSettings",
  "isEnabledForAllMicrosoftApplications": true,
  "disabledForGroup": "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
}
```
