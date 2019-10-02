---
title: função getManagedAppDiagnosticStatuses
description: Obtém diagnóstico do status de validação para um determinado usuário.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3ff023842e487997489ace66bad68b51c686cd91
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37361291"
---
# <a name="getmanagedappdiagnosticstatuses-function"></a>função getManagedAppDiagnosticStatuses

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Obtém diagnóstico do status de validação para um determinado usuário.

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)| _varia por contexto_|
| &nbsp;&nbsp; MAM | DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All |
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppDiagnosticStatuses
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se tiver êxito, essa função retornará um código de resposta `200 OK` e uma coleção [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.

``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}/getManagedAppDiagnosticStatuses
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 249

{
  "value": [
    {
      "@odata.type": "microsoft.graph.managedAppDiagnosticStatus",
      "validationName": "Validation Name value",
      "state": "State value",
      "mitigationInstruction": "Mitigation Instruction value"
    }
  ]
}
```




