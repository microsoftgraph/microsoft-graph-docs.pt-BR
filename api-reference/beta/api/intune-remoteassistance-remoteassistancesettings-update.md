---
title: Atualizar remoteAssistanceSettings
description: Atualize as propriedades de um objeto remoteAssistanceSettings.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 056ba18203dad1ff0e59297959e18459a5b879d9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59096428"
---
# <a name="update-remoteassistancesettings"></a>Atualizar remoteAssistanceSettings

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de [um objeto remoteAssistanceSettings.](../resources/intune-remoteassistance-remoteassistancesettings.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementServiceConfig.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementServiceConfig.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/remoteAssistanceSettings
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o [objeto remoteAssistanceSettings.](../resources/intune-remoteassistance-remoteassistancesettings.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [remoteAssistanceSettings](../resources/intune-remoteassistance-remoteassistancesettings.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador de configurações de assistência remota|
|remoteAssistanceState|[remoteAssistanceState](../resources/intune-remoteassistance-remoteassistancestate.md)|O estado atual da assistência remota para a conta. Os valores possíveis são: notConfigured, disabled, enabled. Essa configuração é configurável pelo administrador. As configurações de assistência remota que ainda não foram configuradas pelo administrador têm um estado nãoConfigurado. Retornado por padrão. Os valores possíveis são: `notConfigured`, `disabled`, `enabled`.|
|allowSessionsToUnenrolledDevices|Boleano| Indica se as sessões para dispositivos não reemrollados são permitidas para a conta. Essa configuração é configurável pelo administrador. O valor padrão é false.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto remoteAssistanceSettings](../resources/intune-remoteassistance-remoteassistancesettings.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/remoteAssistanceSettings
Content-type: application/json
Content-length: 151

{
  "@odata.type": "#microsoft.graph.remoteAssistanceSettings",
  "remoteAssistanceState": "disabled",
  "allowSessionsToUnenrolledDevices": true
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 200

{
  "@odata.type": "#microsoft.graph.remoteAssistanceSettings",
  "id": "cfef360e-360e-cfef-0e36-efcf0e36efcf",
  "remoteAssistanceState": "disabled",
  "allowSessionsToUnenrolledDevices": true
}
```



