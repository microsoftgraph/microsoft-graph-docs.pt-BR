---
title: Tipo de recurso notificationMessageTemplate
description: Mensagens de notificação são mensagens enviadas para usuários finais considerados não compatíveis com as políticas de conformidade definidas pelo administrador. Os administradores escolhem as notificações e as configuram no Console do administrador do Intune usando a página de criação de política de conformidade, na seção "Ações de não conformidade". Use o objeto notificationMessageTemplate para criar suas próprias notificações personalizadas para os administradores escolherem durante a configuração de ações de não conformidade.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4dc7cb92cfbe87cd98b24614cd9fa31f4f81bb38
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32574472"
---
# <a name="notificationmessagetemplate-resource-type"></a>Tipo de recurso notificationMessageTemplate

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Mensagens de notificação são mensagens enviadas para usuários finais considerados não compatíveis com as políticas de conformidade definidas pelo administrador. Os administradores escolhem as notificações e as configuram no Console do administrador do Intune usando a página de criação de política de conformidade, na seção "Ações de não conformidade". Use o objeto notificationMessageTemplate para criar suas próprias notificações personalizadas para os administradores escolherem durante a configuração de ações de não conformidade.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar notificationMessageTemplates](../api/intune-notification-notificationmessagetemplate-list.md)|Conjunto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)|Listar propriedades e relações dos objetos [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).|
|[Obter notificationMessageTemplate](../api/intune-notification-notificationmessagetemplate-get.md)|[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)|Ler propriedades e relações do objeto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).|
|[Criar notificationMessageTemplate](../api/intune-notification-notificationmessagetemplate-create.md)|[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)|Criar um novo objeto de [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).|
|[Excluir notificationMessageTemplate](../api/intune-notification-notificationmessagetemplate-delete.md)|Nenhum|Excluir um [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).|
|[Atualizar notificationMessageTemplate](../api/intune-notification-notificationmessagetemplate-update.md)|[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)|Atualizar as propriedades de um objeto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).|
|[Ação sendTestMessage](../api/intune-notification-notificationmessagetemplate-sendtestmessage.md)|Nenhum|Envia mensagens de teste usando o notificationMessageTemplate especificado no local padrão|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto.|
|displayName|String|Nome de exibição do modelo de mensagem de notificação.|
|defaultLocale|Cadeia de caracteres|A localidade padrão para fallback quando a localidade solicitada não está disponível.|
|brandingOptions|[notificationTemplateBrandingOptions](../resources/intune-notification-notificationtemplatebrandingoptions.md)|As opções de identidade visual do modelo de mensagem. A identidade visual é definida no Console do administrador do Intune. Os valores possíveis são: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|localizedNotificationMessages|Coleção [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)|A lista de mensagens localizadas para esse modelo de mensagem de notificação.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.notificationMessageTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "defaultLocale": "String",
  "brandingOptions": "String"
}
```



