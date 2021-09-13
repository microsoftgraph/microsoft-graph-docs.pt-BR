---
title: tipo de recurso localizedNotificationMessage
description: O conteúdo do texto de um Modelo de mensagem de notificação para a localidade especificada.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 76d93fc670ac4ab65646ace70c2bd19a6d7b4079
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59017300"
---
# <a name="localizednotificationmessage-resource-type"></a>tipo de recurso localizedNotificationMessage

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

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
|localidade|Cadeia de caracteres|A localidade para a qual esta mensagem se destina.|
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



