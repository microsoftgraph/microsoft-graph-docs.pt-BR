---
title: Obter usuário
description: Leia as propriedades e as relações do objeto user.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 909152da2608af14dbcdc693632710e3c6f703dd
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732277"
---
# <a name="get-user"></a>Obter usuário

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Leia as propriedades e as relações do objeto [user](../resources/intune-shared-user.md).

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é necessária para chamar essa API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).  A permissão específica depende do contexto.

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)| _varia de acordo com o contexto_|
| &nbsp;&nbsp;Gerenciamento de dispositivos | DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All |
| &nbsp;&nbsp;MAM | DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All |
| &nbsp;&nbsp;Integração | DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All |
| &nbsp;&nbsp;Solução de problemas | DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All |
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.
## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [user](../resources/intune-shared-user.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.

``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 118

{
  "value": {
    "@odata.type": "#microsoft.graph.user",
    "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
  }
}
```