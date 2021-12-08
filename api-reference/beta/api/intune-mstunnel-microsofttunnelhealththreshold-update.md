---
title: Atualizar microsoftTunnelHealthThreshold
description: Atualize as propriedades de um objeto microsoftTunnelHealthThreshold.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 58f26bc2659341f57b6149418c841cf714d62810
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61339294"
---
# <a name="update-microsofttunnelhealththreshold"></a>Atualizar microsoftTunnelHealthThreshold

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de [um objeto microsoftTunnelHealthThreshold.](../resources/intune-mstunnel-microsofttunnelhealththreshold.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/microsoftTunnelHealthThresholds/{microsoftTunnelHealthThresholdId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o [objeto microsoftTunnelHealthThreshold.](../resources/intune-mstunnel-microsofttunnelhealththreshold.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [o microsoftTunnelHealthThreshold](../resources/intune-mstunnel-microsofttunnelhealththreshold.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O nome métrico|
|healthyThreshold|Int64|O limite para estar saudável|
|unhealthyThreshold|Int64|O limite para não estar 100%|
|defaultHealthyThreshold|Int64|O limite padrão para ser saudável|
|defaultUnhealthyThreshold|Int64|O limite padrão para não estar 100%|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto microsoftTunnelHealthThreshold](../resources/intune-mstunnel-microsofttunnelhealththreshold.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelHealthThresholds/{microsoftTunnelHealthThresholdId}
Content-type: application/json
Content-length: 194

{
  "@odata.type": "#microsoft.graph.microsoftTunnelHealthThreshold",
  "healthyThreshold": 0,
  "unhealthyThreshold": 2,
  "defaultHealthyThreshold": 7,
  "defaultUnhealthyThreshold": 9
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 243

{
  "@odata.type": "#microsoft.graph.microsoftTunnelHealthThreshold",
  "id": "419c526e-526e-419c-6e52-9c416e529c41",
  "healthyThreshold": 0,
  "unhealthyThreshold": 2,
  "defaultHealthyThreshold": 7,
  "defaultUnhealthyThreshold": 9
}
```




