---
title: Tipo de recurso notificationMessageTemplate
description: Mensagens de notificação são mensagens enviadas para usuários finais considerados não compatíveis com as políticas de conformidade definidas pelo administrador. Os administradores escolhem as notificações e as configuram no Console do administrador do Intune usando a página de criação de política de conformidade, na seção "Ações de não conformidade". Use o objeto notificationMessageTemplate para criar suas próprias notificações personalizadas para os administradores escolherem durante a configuração de ações de não conformidade.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9fa82b29f0512dce75191b537dc65108175525f27b200d4be7a8e69a79e17316
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54135082"
---
# <a name="notificationmessagetemplate-resource-type"></a>Tipo de recurso notificationMessageTemplate

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

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
|id|Cadeia de caracteres|Chave da entidade.|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto.|
|displayName|Cadeia de caracteres|Nome de exibição do modelo de mensagem de notificação.|
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




