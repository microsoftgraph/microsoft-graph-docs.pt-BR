---
title: tipo de recurso resourceSpecificPermission
description: Representa permissões usadas para autorizar um aplicativo para acesso direto a dados para uma instância específica do recurso
author: psignoret
ms.localizationpriority: medium
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: bc1cd89ba26629b59c83fdd6b626cb280f69eaab
ms.sourcegitcommit: efa06c63cd3154bcc7ecc993011f314c2dea9a92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63376382"
---
# <a name="resourcespecificpermission-resource-type"></a>tipo de recurso resourceSpecificPermission

Namespace: microsoft.graph

Representa permissões usadas para autorizar um aplicativo para acesso direto a dados para uma instância específica do recurso, como um chat ou uma equipe. Por exemplo, a permissão específica do recurso ChannelMessage.Read.Group permite que um aplicativo Microsoft Teams leia as mensagens de canal de uma única equipe. 

Permissões específicas de recursos são suportadas apenas para aplicativos Teams acessando chats e equipes específicos usando a API do Microsoft Graph. Para obter detalhes, consulte [Consentimento específico de recursos para Teams aplicativos](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|description|String|Descreve o nível de acesso que a permissão específica do recurso representa.|
|displayName|String|O nome de exibição da permissão específica do recurso.|
|id|Guid|O identificador exclusivo para a permissão de aplicativo específico do recurso.|
|isEnabled|Booliano|Indica se a permissão está habilitada.|
|value|Cadeia de caracteres|O valor da permissão.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resourceSpecificPermission"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceSpecificPermission",
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isEnabled": "Boolean",
  "value": "String"
}
```
