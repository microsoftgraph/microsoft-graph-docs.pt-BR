---
title: Obter teamsAppSettings
description: Leia as propriedades e as relações de um objeto teamsAppSettings.
author: subray2014
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: bd04f3dcdb72775ec372763cb12e94ccbead9a0d
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645586"
---
# <a name="get-teamsappsettings"></a>Obter teamsAppSettings
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Leia as propriedades e as relações de um [objeto teamsAppSettings](../resources/teamsappsettings.md) .

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|TeamworkAppSettings.Read.All, TeamworkAppSettings.ReadWrite.All|
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
GET /teamwork/teamsAppSettings
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código `200 OK` de resposta e um [objeto teamsAppSettings](../resources/teamsappsettings.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-get-the-tenant-wide-settings-for-all-teams-apps-in-the-tenant"></a>Exemplo 1: obtenha as configurações de todo o locatário para todos os aplicativos do Teams no locatário.

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "get_teamsappsettings"
}
-->
``` http
GET https://graph.microsoft.com/beta/teamwork/teamsAppSettings
```


#### <a name="response"></a>Resposta

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppSettings"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.teamsAppSettings",
    "id": "65bdf003-0c4c-4bca-b102-0821ab0d1364",
    "isChatResourceSpecificConsentEnabled": "true"
  }
}
```

## <a name="see-also"></a>Confira também

- [Consentimento específico do recurso](/microsoftteams/platform/graph-api/rsc/resource-specific-consent)