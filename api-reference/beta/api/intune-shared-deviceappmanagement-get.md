---
title: Get deviceAppManagement
description: Ler propriedades e relações do objeto deviceAppManagement.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 64da3a10fbf0f218dd38b32cb67103b894e037ea
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437342"
---
# <a name="get-deviceappmanagement"></a>Get deviceAppManagement

Namespace: microsoft.graph

> **Importante:** As APIs na versão /beta no Microsoft Graph estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ler propriedades e relações do objeto [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).

## <a name="prerequisites"></a>Pré-requisitos

Uma das permissões a seguir é necessária para chamar essa API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).  Observe que a permissão apropriada varia de acordo com o fluxo de trabalho.

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
| Delegada (conta corporativa ou de estudante) | |
| &nbsp;&nbsp; **Aplicativos**, **livros**, **integração**, **integração de parceiros** ou **conjunto de políticas** | DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All |
| &nbsp;&nbsp; **Gerenciamento de dispositivos** | DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All |
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo| |
| &nbsp;&nbsp; **Aplicativos**, **livros**, **integração**, **integração de parceiros** ou **conjunto de políticas** | DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All |
| &nbsp; &nbsp; **Gerenciamento de dispositivos** | DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

Este é um exemplo da solicitação.

``` http
GET https://graph.microsoft.com/beta/deviceAppManagement
```

### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 133

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceAppManagement",
    "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
  }
}
```









