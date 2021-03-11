---
title: Tipo de recurso accessPackageResourceEnvironment
description: Um ambiente de recurso do pacote de acesso é uma referência ao ambiente de localização geográfica no qual um recurso está localizado.
author: hanki-microsoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 09bd318036874bb52bfab0ed522a2948cbe83233
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722192"
---
# <a name="accesspackageresourceenvironment-resource-type"></a>Tipo de recurso accessPackageResourceEnvironment

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No [Azure AD Entitlement Management](entitlementmanagement-root.md), um ambiente de recurso do pacote de acesso é uma referência ao ambiente de localização geográfica no qual um recurso está localizado. Esse ambiente é fornecido automaticamente como parte do Gerenciamento de Direitos do Azure AD. A API só é aplicável a sites multi-geo do SharePoint Online.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar accessPackageResourceEnvironments](../api/accesspackageresourceenvironment-list.md)|[coleção accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md)|Recupere uma lista de [objetos accessPackageResourceEnvironment.](../resources/accesspackageresourceenvironment.md)|
|[Obter accessPackageResourceEnvironment](../api/accesspackageresourceenvironment-get.md)|[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md)|Leia as propriedades e as relações de um [objeto accessPackageResourceEnvironment.](../resources/accesspackageresourceenvironment.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|connectionInfo|[connectionInfo](../resources/connectioninfo.md)|Informações de conexão de um ambiente usado para se conectar a um recurso. |
|createdBy|Cadeia de caracteres|O nome de exibição do usuário que criou esse objeto.|
|createdDateTime|DateTimeOffset|A data e a hora em que esse objeto foi criado. <br>O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|description|Cadeia de caracteres|A descrição desse *objeto accessPackageResourceEnvironment.*|
|displayName|Cadeia de caracteres|O nome de exibição deste objeto.|
|id|Cadeia de caracteres|O identificador exclusivo atribuído pelo sistema do objeto.|
|isDefaultEnvironment|Booliano|Determina se esse é o ambiente padrão ou não. Ele é definido como `true` para todos os sistemas de origem estática, como grupos do Azure AD e Aplicativos do Azure AD.|
|modifiedBy|Cadeia de caracteres|O nome de exibição da entidade que modificou esse objeto pela última vez.|
|modifiedDateTime|DateTimeOffset|A data e a hora em que esse objeto foi modificado pela última vez. <br>O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. |
|originId|Cadeia de caracteres|O identificador exclusivo desse ambiente no sistema de origem.|
|originSystem|Cadeia de caracteres|O tipo do recurso no sistema de origem, como `SharePointOnline` . Oferece suporte para `$filter`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|accessPackageResources|[Coleção accessPackageResource](../resources/accesspackageresource.md)|Somente leitura. Obrigatório.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageResourceEnvironment",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageResourceEnvironment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "originSystem": "String",
  "originId": "String",
  "isDefaultEnvironment": "Boolean",
  "connectionInfo": {
    "@odata.type": "microsoft.graph.connectionInfo"
  },
  "createdBy": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedBy": "String",
  "modifiedDateTime": "String (timestamp)"
}
```
