---
title: Criar remoteAssistancePartner
description: Criar um novo objeto remoteAssistancePartner.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8b1f8306c3ece3b5153a9352c38e41eb89e71d6b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410424"
---
# <a name="create-remoteassistancepartner"></a>Criar remoteAssistancePartner

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Criar um novo objeto [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementServiceConfig.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto remoteAssistancePartner.

A tabela a seguir mostra as propriedades que são necessárias ao criar remoteAssistancePartner.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo do parceiro.|
|displayName|Cadeia de caracteres|Nome de exibição do parceiro.|
|onboardingUrl|Cadeia de caracteres|URL do portal de integração do parceiro, no qual um administrador pode configurar o serviço de assistência remota.|
|onboardingStatus|[remoteAssistanceOnboardingStatus](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|TBD. Os valores possíveis são: `notOnboarded`, `onboarding`, `onboarded`.|
|lastConnectionDateTime|DateTimeOffset|Carimbo de data/hora da última solicitação enviada ao Intune pelo parceiro TEM.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/remoteAssistancePartners
Content-type: application/json
Content-length: 266

{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "displayName": "Display Name value",
  "onboardingUrl": "https://example.com/onboardingUrl/",
  "onboardingStatus": "onboarding",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 315

{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "id": "7443c8b9-c8b9-7443-b9c8-4374b9c84374",
  "displayName": "Display Name value",
  "onboardingUrl": "https://example.com/onboardingUrl/",
  "onboardingStatus": "onboarding",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```




