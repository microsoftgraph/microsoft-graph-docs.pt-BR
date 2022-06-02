---
title: Ação getZebraFotaDeploymentReport
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d90a796c90a1f78c6df7559d479be6a523c3fa20
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2022
ms.locfileid: "65858574"
---
# <a name="getzebrafotadeploymentreport-action"></a>Ação getZebraFotaDeploymentReport

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Application|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getZebraFotaDeploymentReport
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON dos parâmetros.

A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|nome|String|Ainda não documentado|
|select|String collection|Ainda não documentado|
|search|String|Ainda não documentado|
|Groupby|String collection|Ainda não documentado|
|Orderby|String collection|Ainda não documentado|
|skip|Int32|Ainda não documentado|
|top|Int32|Ainda não documentado|
|Sessionid|Int32|Ainda não documentado|
|filter|String|Ainda não documentado|



## <a name="response"></a>Resposta
Se for bem-sucedida, essa ação retornará um `200 OK` código de resposta e um Fluxo no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/getZebraFotaDeploymentReport

Content-type: application/json
Content-length: 261

{
  "name": "Name value",
  "select": [
    "Select value"
  ],
  "search": "Search value",
  "groupBy": [
    "Group By value"
  ],
  "orderBy": [
    "Order By value"
  ],
  "skip": 4,
  "top": 3,
  "sessionId": 9,
  "filter": "Filter value"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "value": "Z2V0WmVicmFGb3RhRGVwbG95bWVudFJlcG9ydCBJbnR1bmUgRG9jIFNhbXBsZSAyMDcxMDQ2MzM5"
}
```




