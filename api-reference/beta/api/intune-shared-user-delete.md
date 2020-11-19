---
title: Excluir usuário
description: Exclui usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 669b35665fa0cf4449a12cb8af2e1bbc753ec6de
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49232204"
---
# <a name="delete-user"></a>Excluir usuário

Namespace: microsoft.graph

> **Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Exclui [usuário](../resources/intune-shared-user.md).
## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é necessária para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).  A permissão específica necessária depende do contexto.

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)||
| &nbsp;&nbsp; **Gerenciamento de dispositivos** | DeviceManagementManagedDevices.ReadWrite.All|
| &nbsp;&nbsp; **Mam** | DeviceManagementApps.ReadWrite.All|
| &nbsp; &nbsp; **Integração** | DeviceManagementServiceConfig.ReadWrite.All|
| &nbsp; &nbsp; **Solução de problemas** | DeviceManagementManagedDevices.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Application||
| &nbsp;&nbsp; **Gerenciamento de dispositivos** | DeviceManagementManagedDevices.ReadWrite.All|
| &nbsp;&nbsp; **Mam** | DeviceManagementApps.ReadWrite.All|
| &nbsp; &nbsp; **Integração** | DeviceManagementServiceConfig.ReadWrite.All|
| &nbsp; &nbsp; **Solução de problemas** | DeviceManagementManagedDevices.ReadWrite.All|

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










