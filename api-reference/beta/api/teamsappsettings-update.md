---
title: Atualizar teamsAppSettings
description: Atualize as propriedades de um objeto teamsAppSettings.
author: subray2014
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5fdcc9fafe199e11881c59e65842c09d955eb74e
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645600"
---
# <a name="update-teamsappsettings"></a>Atualizar teamsAppSettings
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades de um [objeto teamsAppSettings](../resources/teamsappsettings.md) .

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

>**Nota:** Somente administradores globais e administradores do Teams podem chamar essa API.

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|TeamworkAppSettings.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte|
|Aplicativo|Sem suporte|

> [!NOTE]
> As permissões TeamworkAppSettings.* podem não estar visíveis no portal do Azure. Para obter detalhes e soluções alternativas, consulte [problemas conhecidos](/graph/known-issues#teamworkappsettings-permissions-are-not-visible-in-the-azure-portal).

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /teamwork/teamsAppSettings
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
|isChatResourceSpecificConsentEnabled|Booliano|Indica se o consentimento específico do recurso para chats/reuniões foi habilitado para o locatário. Se verdadeiro, os aplicativos do Teams permitidos no locatário e que exigem permissões específicas de recursos podem ser instalados dentro de chats e reuniões. Se for false, a instalação de qualquer aplicativo do Teams que exija permissões específicas de recursos em um chat ou reunião será bloqueada.|



## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="example-1-enable-installation-of-apps-that-require-resource-specific-consent-in-chatsmeetings"></a>Exemplo 1: habilitar a instalação de aplicativos que exigem consentimento específico de recursos em chats/reuniões.

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "update_teamsappsettings"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/teamwork/teamsAppSettings
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.teamsAppSettings",
  "isChatResourceSpecificConsentEnabled": "true"
}
```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a>Confira também

- [Consentimento específico do recurso](/microsoftteams/platform/graph-api/rsc/resource-specific-consent)