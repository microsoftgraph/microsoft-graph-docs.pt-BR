---
title: Atualizar dataSharingConsent
description: Atualize as propriedades de um objeto dataSharingConsent.
author: tfitzmac
ms.openlocfilehash: 1d7759def9c11165fca0b646f166ac792c14369e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317630"
---
# <a name="update-datasharingconsent"></a>Atualizar dataSharingConsent

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Atualize as propriedades de um objeto [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) .
## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

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
PATCH /deviceManagement/dataSharingConsents/{dataSharingConsentId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Accept|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o objeto [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) .

A tabela a seguir mostra as propriedades que são necessárias quando você cria o [dataSharingConsent](../resources/intune-devices-datasharingconsent.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O consentimento de compartilhamento de dados Id|
|Nome_para_exibição_do_serviço|String|O nome para exibição do fluxo de trabalho de serviço|
|termsUrl|String|O TermsUrl para os consentimento de compartilhamento de dados|
|concedido|Boolean|O estado foram concedido para os consentimento de compartilhamento de dados|
|grantDateTime|DateTimeOffset|O consentimento de tempo foi concedido para esta conta|
|grantedByUpn|String|O Upn do usuário que tenha concedido consentimento para esta conta|
|grantedByUserId|String|A identificação do usuário do usuário que tenha concedido consentimento para esta conta|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) no corpo da resposta.

## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/dataSharingConsents/{dataSharingConsentId}
Content-type: application/json
Content-length: 276

{
  "serviceDisplayName": "Service Display Name value",
  "termsUrl": "https://example.com/termsUrl/",
  "granted": true,
  "grantDateTime": "2016-12-31T23:59:55.7154191-08:00",
  "grantedByUpn": "Granted By Upn value",
  "grantedByUserId": "Granted By User Id value"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 382

{
  "@odata.type": "#microsoft.graph.dataSharingConsent",
  "id": "333387f7-87f7-3333-f787-3333f7873333",
  "serviceDisplayName": "Service Display Name value",
  "termsUrl": "https://example.com/termsUrl/",
  "granted": true,
  "grantDateTime": "2016-12-31T23:59:55.7154191-08:00",
  "grantedByUpn": "Granted By Upn value",
  "grantedByUserId": "Granted By User Id value"
}
```





