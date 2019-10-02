---
title: Atualizar usuário
description: Atualize as propriedades de um objeto user.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 944930fcb5eb046908fe157713a486845322e2cc
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37361228"
---
# <a name="update-user"></a>Atualizar usuário

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualizar as propriedades de um objeto [user](../resources/intune-shared-user.md).

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)| _varia por contexto_|
| &nbsp;&nbsp; Gerenciamento de dispositivos | DeviceManagementManagedDevices.ReadWrite.All |
| &nbsp;&nbsp; MAM | DeviceManagementApps.ReadWrite.All |
| &nbsp;&nbsp; Integração | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; Solução de problemas | DeviceManagementManagedDevices.ReadWrite.All |
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/intune-shared-user.md).

A tabela a seguir mostra as propriedades que são necessárias ao criar [user](../resources/intune-shared-user.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo do usuário.|
|**Integração**|
|deviceEnrollmentLimit|Int32|O limite do número máximo de dispositivos que o usuário tem permissão para inscrever. Os valores permitidos vão de 5 a 1000.|

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [user](../resources/intune-shared-user.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.

``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```




