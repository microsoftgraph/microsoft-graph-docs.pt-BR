---
title: Tipo de recurso applePushNotificationCertificate
description: Certificado de notificação por push da Apple.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c4a90b85dc79ff5261037e2f556b844691eeab2a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465268"
---
# <a name="applepushnotificationcertificate-resource-type"></a>Tipo de recurso applePushNotificationCertificate

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Certificado de notificação por push da Apple.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter applePushNotificationCertificate](../api/intune-devices-applepushnotificationcertificate-get.md)|[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md)|Ler propriedades e relações de objetos de [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).|
|[Atualizar applePushNotificationCertificate](../api/intune-devices-applepushnotificationcertificate-update.md)|[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md)|Atualizar as propriedades de um objeto de [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).|
|[Função downloadApplePushNotificationCertificateSigningRequest](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|String|Baixa a solicitação de assinatura de certificado de notificação por push da Apple|
|[ação generateApplePushNotificationCertificateSigningRequest](../api/intune-devices-applepushnotificationcertificate-generateapplepushnotificationcertificatesigningrequest.md)|String|Baixa a solicitação de assinatura de certificado de notificação por push da Apple|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo do certificado.|
|appleIdentifier|String|Id da Apple da conta usada para criar o certificado de push do MDM.|
|topicIdentifier|Cadeia de caracteres|ID do tópico.|
|lastModifiedDateTime|DateTimeOffset|Data e hora da última modificação de certificado de notificações por push da Apple.|
|expirationDateTime|DateTimeOffset|Data e hora do vencimento de certificado de notificações por push da Apple.|
|certificateUploadStatus|String|O status do carregamento do certificado.|
|certificateUploadFailureReason|String|O motivo da falha no carregamento do certificado.|
|certificateSerialNumber|String|Número de série do certificado. Essa propriedade é somente leitura.|
|certificado|String|Ainda não documentado|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.applePushNotificationCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "id": "String (identifier)",
  "appleIdentifier": "String",
  "topicIdentifier": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "certificateUploadStatus": "String",
  "certificateUploadFailureReason": "String",
  "certificateSerialNumber": "String",
  "certificate": "String"
}
```



