---
title: Atualizar cloudPcOrganizationSettings
description: Atualize as propriedades de um objeto cloudPcOrganizationSettings.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: c051f3dd21e2e6e8ad7071ee0a2980b66d1313fe
ms.sourcegitcommit: bfd1ab7e015ef04cb2ca3fb85d308ba2ce830a89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/19/2022
ms.locfileid: "62072772"
---
# <a name="update-cloudpcorganizationsettings"></a>Atualizar cloudPcOrganizationSettings
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades do [objeto cloudPcOrganizationSettings](../resources/cloudpcorganizationsettings.md) em um locatário.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|CloudPC.Read.All, CloudPC.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|CloudPC.Read.All, CloudPC.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/virtualEndpoint/cloudPcOrganizationSettings
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
|osVersion|cloudPcOperatingSystem|A versão do sistema operacional (OS) a ser provisionada em PCs na Nuvem. Os valores possíveis são: `windows10`, `windows11`, `unknownFutureValue`. Opcional.|
|userAccountType|cloudPcUserAccountType|O tipo de conta do usuário em PCs de Nuvem provisionados. Os valores possíveis são: `standardUser`, `administrator`, `unknownFutureValue`. Opcional.|


## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "update_cloudpcorganizationsettings"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/organizationSettings
Content-Type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.cloudPcOrganizationSettings",
  "userAccountType": "standardUser",
  "osVersion": "windows11"
}
```


### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
