---
title: Criar usuário
description: Criar um novo objeto user.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f46fbbc365e52ae9e46db9f6c05c3c8e8eeddc92
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572254"
---
# <a name="create-user"></a>Criar usuário

> **Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Criar um novo objeto [user](../resources/intune-shared-user.md).

## <a name="prerequisites"></a>Pré-requisitos

Uma das seguintes permissões é necessária para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).  A permissão específica necessária depende do contexto.

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)||
| &nbsp; &nbsp; **Gerenciamento de dispositivo** | DeviceManagementManagedDevices.ReadWrite.All|
| &nbsp;&nbsp; **Mam** | DeviceManagementApps.ReadWrite.All|
| &nbsp; &nbsp; **Integração** | DeviceManagementServiceConfig.ReadWrite.All|
| &nbsp; &nbsp; **Solução de problemas** | DeviceManagementManagedDevices.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça uma representação JSON do objeto user.

A tabela a seguir mostra as propriedades que são necessárias ao criar user.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo do usuário.|
|**Integração**||
|deviceEnrollmentLimit|Int32|O limite do número máximo de dispositivos que o usuário tem permissão para inscrever. Os valores permitidos vão de 5 a 1000.|

O suporte à propriedade do corpo da solicitação varia de acordo com o contexto.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [user](../resources/intune-shared-user.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

Este é um exemplo da solicitação.

``` http
POST https://graph.microsoft.com/beta/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. As propriedades retornadas de uma chamada real variam de acordo com o contexto.

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



