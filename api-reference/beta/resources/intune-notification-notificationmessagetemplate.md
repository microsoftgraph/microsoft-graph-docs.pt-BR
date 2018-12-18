---
title: Tipo de recurso notificationMessageTemplate
description: " seção. Use o objeto notificationMessageTemplate para criar suas próprias notificações personalizadas para os administradores escolherem durante a configuração de ações de não conformidade."
author: tfitzmac
ms.openlocfilehash: eae9d0ada0dcaf160b0b7dc8802af3ccbcfaa8f4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316237"
---
# <a name="notificationmessagetemplate-resource-type"></a>Tipo de recurso notificationMessageTemplate

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

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
|displayName|Cadeia de caracteres|Nome de exibição do modelo de mensagem de notificação.|
|defaultLocale|Cadeia de caracteres|A localidade padrão para fallback quando a localidade solicitada não está disponível.|
|brandingOptions|[notificationTemplateBrandingOptions](../resources/intune-notification-notificationtemplatebrandingoptions.md)|As opções de identidade visual do modelo de mensagem. A identidade visual é definida no Console do administrador do Intune. Os valores possíveis são: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.|
|roleScopeTagIds|String collection|Lista de escopo marcas para essa instância da entidade.|

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
  "brandingOptions": "String",
  "roleScopeTagIds": [
    "String"
  ]
}
```





