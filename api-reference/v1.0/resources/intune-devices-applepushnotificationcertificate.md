---
title: Tipo de recurso applePushNotificationCertificate
description: Certificado de notificação por push da Apple.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2bbcca2707223f53b59d1b3d5d2ceb75ba08c57a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091317"
---
# <a name="applepushnotificationcertificate-resource-type"></a>Tipo de recurso applePushNotificationCertificate

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Certificado de notificação por push da Apple.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter applePushNotificationCertificate](../api/intune-devices-applepushnotificationcertificate-get.md)|[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md)|Ler propriedades e relações de objetos de [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).|
|[Atualizar applePushNotificationCertificate](../api/intune-devices-applepushnotificationcertificate-update.md)|[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md)|Atualizar as propriedades de um objeto de [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).|
|[Função downloadApplePushNotificationCertificateSigningRequest](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|Cadeia de caracteres|Baixa a solicitação de assinatura de certificado de notificação por push da Apple|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo do certificado.|
|appleIdentifier|Cadeia de caracteres|Id da Apple da conta usada para criar o certificado de push do MDM.|
|topicIdentifier|Cadeia de caracteres|ID do tópico.|
|lastModifiedDateTime|DateTimeOffset|Data e hora da última modificação de certificado de notificações por push da Apple.|
|expirationDateTime|DateTimeOffset|Data e hora do vencimento de certificado de notificações por push da Apple.|
|certificado|Cadeia de caracteres|Ainda não documentado|

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
  "certificate": "String"
}
```









