---
title: Criar mobileAppTroubleshootingEvent
description: Descreve o método Create mobileAppTroubleshootingEvent da API do Microsoft Graph para o Intune, que oferece suporte a vários fluxos de trabalho.
ms.localizationpriority: medium
author: rolyon
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 539cd4c502d4f053d74fdd8f9638ccb12676c733
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59033949"
---
# <a name="create-mobileapptroubleshootingevent"></a>Criar mobileAppTroubleshootingEvent

Namespace: microsoft.graph

> **Importante:** APIs na versão /beta no Microsoft Graph estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo [objeto mobileAppTroubleshootingEvent.](../resources/intune-shared-mobileapptroubleshootingevent.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)||
|&nbsp; &nbsp; **Gerenciamento de dispositivo**|DeviceManagementManagedDevices.ReadWrite.All|
|&nbsp; &nbsp; **Solução de problemas**|DeviceManagementManagedDevices.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo||
|&nbsp; &nbsp; **Gerenciamento de dispositivo**|DeviceManagementManagedDevices.ReadWrite.All|
|&nbsp; &nbsp; **Solução de problemas**|DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileAppTroubleshootingEvents
POST /users/{usersId}/mobileAppTroubleshootingEvents
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o objeto mobileAppTroubleshootingEvent.

A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppTroubleshootingEvent.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O GUID do objeto.|
|**Solução de Problemas**|
|additionalInformation|Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Um conjunto de pares de valores de chave de cadeia de caracteres e cadeia de caracteres que fornece informações adicionais sobre o evento Solução de problemas.|
|ApplicationId|Cadeia de caracteres|Identificador de aplicativo do Intune.|
|correlationId|Cadeia de caracteres|ID usada para rastrear a falha no serviço. |
|eventDateTime|DateTimeOffset|A hora em que o evento ocorreu. |
|eventName|Cadeia de caracteres|Nome do Evento correspondente ao Evento de Solução de Problemas. Opcional.|
|history|[coleção mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)|Item histórico de solução de problemas de aplicativo móvel do Intune|
|managedDeviceIdentifier|Cadeia de caracteres|Identificador de dispositivo criado ou coletado pelo Intune.|
|troubleshootingErrorDetails|[deviceManagementTroubleshootingErrorDetails](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|Objeto contendo informações detalhadas sobre o erro e sua correção. |
|userId|Cadeia de caracteres|Identificador do usuário que tentou registrar o dispositivo.|

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de `201 Created` resposta e um objeto [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents
Content-type: application/json
Content-length: 71

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 120

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "77943c10-3c10-7794-103c-9477103c9477"
}
```










