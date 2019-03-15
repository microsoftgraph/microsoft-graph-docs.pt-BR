---
title: Ação removeAllDevicesFromManagement
description: Desativa todos os dispositivos de gerenciamento deste usuário
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 72a4ebafd857abef85231b90327f9f6d94e5f99b
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571078"
---
# <a name="removealldevicesfrommanagement-action"></a>Ação removeAllDevicesFromManagement

> **Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Desativa todos os dispositivos de gerenciamento deste usuário
## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)||
| &nbsp; &nbsp; **Gerenciamento de dispositivo** | DeviceManagementManagedDevices.PriviligedOperation.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/removeAllDevicesFromManagement
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.

## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/removeAllDevicesFromManagement
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 204 No Content
```





