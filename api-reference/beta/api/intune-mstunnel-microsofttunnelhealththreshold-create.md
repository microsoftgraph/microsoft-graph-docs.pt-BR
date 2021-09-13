---
title: Criar microsoftTunnelHealthThreshold
description: Crie um novo objeto microsoftTunnelHealthThreshold.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: eec3d33082e1accef4c9bb0f5ec7f980009a2c13
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59041805"
---
# <a name="create-microsofttunnelhealththreshold"></a>Criar microsoftTunnelHealthThreshold

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo [objeto microsoftTunnelHealthThreshold.](../resources/intune-mstunnel-microsofttunnelhealththreshold.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementConfiguration.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/microsoftTunnelHealthThresholds
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o objeto microsoftTunnelHealthThreshold.

A tabela a seguir mostra as propriedades que são necessárias ao criar o microsoftTunnelHealthThreshold.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O nome métrico|
|healthyThreshold|Int64|O limite para estar saudável|
|unhealthyThreshold|Int64|O limite para não estar 100%|
|defaultHealthyThreshold|Int64|O limite padrão para ser saudável|
|defaultUnhealthyThreshold|Int64|O limite padrão para não estar 100%|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto microsoftTunnelHealthThreshold](../resources/intune-mstunnel-microsofttunnelhealththreshold.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelHealthThresholds
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
HTTP/1.1 201 Created
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



