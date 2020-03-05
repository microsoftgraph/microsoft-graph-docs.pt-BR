---
title: tipo de recurso localizedNotificationMessage
description: O conteúdo do texto de um Modelo de mensagem de notificação para a localidade especificada.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c8524263c2d0d3f3479ef83af8e90a41e700934f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448183"
---
# <a name="localizednotificationmessage-resource-type"></a>tipo de recurso localizedNotificationMessage

Namespace: Microsoft. Graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O conteúdo do texto de um Modelo de mensagem de notificação para a localidade especificada.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar localizedNotificationMessages](../api/intune-notification-localizednotificationmessage-list.md)|Conjunto [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)|Listar propriedades e relações de objetos de [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).|
|[Obter localizedNotificationMessage](../api/intune-notification-localizednotificationmessage-get.md)|[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)|Ler propriedades e relações de objetos de [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).|
|[Criar localizedNotificationMessage](../api/intune-notification-localizednotificationmessage-create.md)|[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)|Criar um novo objeto de [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).|
|[Excluir localizedNotificationMessage](../api/intune-notification-localizednotificationmessage-delete.md)|Nenhum|Excluir [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).|
|[Atualizar localizedNotificationMessage](../api/intune-notification-localizednotificationmessage-update.md)|[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)|Atualizar as propriedades de um objeto de [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto.|
|localidade|String|A localidade para a qual esta mensagem se destina.|
|assunto|Cadeia de caracteres|O assunto do modelo da mensagem.|
|messageTemplate|Cadeia de caracteres|O conteúdo do modelo da mensagem.|
|isDefault|Booliano|Sinaliza para indicar se esta é ou não a localidade padrão do fallback de idioma. Esse sinalizador só pode ser definido. Para remover a definição, defina esta propriedade como verdadeira na outra Mensagem de notificação localizada.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.localizedNotificationMessage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.localizedNotificationMessage",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "locale": "String",
  "subject": "String",
  "messageTemplate": "String",
  "isDefault": true
}
```




