---
title: Excluir usuário
description: Exclui usuário.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ecf07bf080a76e6f1fce515d41090be214e7a514
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407148"
---
# <a name="delete-user"></a>Excluir usuário

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Exclui [usuário](../resources/intune-shared-user.md).
## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é necessário chamar essa API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).  A permissão específica necessária depende de contexto.

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)||
| &nbsp; &nbsp; **Gerenciamento de dispositivo** | DeviceManagementManagedDevices.ReadWrite.All|
| &nbsp;&nbsp; **MAM** | DeviceManagementApps.ReadWrite.All|
| &nbsp;&nbsp; **Onboarding** | DeviceManagementServiceConfig.ReadWrite.All|
| &nbsp; &nbsp; **Solução de problemas** | DeviceManagementManagedDevices.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

Este é um exemplo da solicitação.

``` http
DELETE https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.

``` http
HTTP/1.1 204 No Content
```



