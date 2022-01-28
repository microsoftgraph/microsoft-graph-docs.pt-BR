---
title: 'teamworkDevice: updateSoftware'
description: Atualize o software para um Microsoft Teams habilitado para uso.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: teamwork
doc_type: apiPageType
ms.openlocfilehash: 9e2435dc52b88e836874ceae1b3e62bd09fdaec5
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262304"
---
# <a name="teamworkdevice-updatesoftware"></a>teamworkDevice: updateSoftware
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize o software para um Microsoft Teams habilitado para [uso.](../resources/teamworkdevice.md) Essa API dispara uma operação de longa duração.

[!INCLUDE [teamworkdevice-api-disclaimer](../../includes/teamworkdevice-api-disclaimer.md)]

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|TeamworkDevice.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|TeamworkDevice.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /teamwork/devices/{teamworkDeviceId}/updateSoftware
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON dos parâmetros.

A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.

|Parâmetro|Tipo|Descrição|
|:---|:---|:---|
|softwareType|teamworkSoftwareType|O tipo de software a ser atualizado. Os tipos válidos são: , , , , , `companyPortal``partnerAgent`. `firmware``teamsClient``operatingSystem``adminAgent`|
|softwareVersion|Cadeia de caracteres|Especifica a versão do software disponível para atualização.|



## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. A resposta também conterá um `Location` header, que contém o local do recurso [teamworkDeviceOperation](../resources/teamworkdeviceoperation.md) . Você pode verificar o status da operação de atualização de software fazendo uma solicitação GET para esse local `queued`que retorna se a operação é , `succeeded`ou `failed`.

Esse método também retornará um `409 Conflict` código de resposta se a operação já estiver em fila.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "teamworkdevice_updatesoftware"
}
-->
``` http
POST https://graph.microsoft.com/beta/teamwork/devices/0f3ce432-e432-0f3c-32e4-3c0f32e43c0f/updateSoftware
Content-Type: application/json
Content-length: 64

{
  "softwareType": "teamsClient",
  "softwareVersion": "1.0.96.22"
}
```


### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
Location: /teamwork/devices/0f3ce432-e432-0f3c-32e4-3c0f32e43c0f/operations/119eb06d-0c4b-4fb3-a754-33dd0d6b618c
Content-Type: text/plain
Content-Length: 0
```

