---
title: Tipo de recurso accessPackageResourceEnvironment
description: Um ambiente de recurso do pacote de acesso é uma referência ao ambiente de geolocalização no qual um recurso está localizado.
author: hanki-microsoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 814e77cb8122773bc425180c7e78a2794c9e0784
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137691"
---
# <a name="accesspackageresourceenvironment-resource-type"></a>Tipo de recurso accessPackageResourceEnvironment

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No Gerenciamento de Direitos do [Azure AD,](entitlementmanagement-root.md)um ambiente de recursos do pacote de acesso é uma referência ao ambiente de geolocalização no qual um recurso está localizado. Esse ambiente é fornecido automaticamente como parte do Gerenciamento de Entilement do Azure AD. A API só é aplicável a sites multi-geo do SharePoint Online.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar accessPackageResourceEnvironments](../api/accesspackageresourceenvironment-list.md)|[Coleção accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md)|Recupere uma lista de [objetos accessPackageResourceEnvironment.](../resources/accesspackageresourceenvironment.md)|
|[Acessar AccessPackageResourceEnvironment](../api/accesspackageresourceenvironment-get.md)|[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md)|Leia as propriedades e os relacionamentos de um [objeto accessPackageResourceEnvironment.](../resources/accesspackageresourceenvironment.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|connectionInfo|[connectionInfo](../resources/connectioninfo.md)|Informações de conexão de um ambiente usado para se conectar a um recurso. |
|createdBy|Cadeia de caracteres|O nome de exibição do usuário que criou esse objeto.|
|createdDateTime|DateTimeOffset|A data e a hora em que esse objeto foi criado. <br>O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 `'2014-01-01T00:00:00Z'` será.|
|description|String|A descrição deste *objeto accessPackageResourceEnvironment.*|
|displayName|String|O nome de exibição deste objeto.|
|id|String|O identificador exclusivo atribuído pelo sistema do objeto.|
|isDefaultEnvironment|Boolean|Determina se esse é o ambiente padrão ou não. Ele é definido para todos os sistemas de origem estáticos, como grupos do `true` Azure AD e aplicativos do Azure AD.|
|modifiedBy|String|O nome de exibição da entidade que modificou esse objeto pela última vez.|
|modifiedDateTime|DateTimeOffset|A data e a hora em que esse objeto foi modificado pela última vez. <br>O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 `'2014-01-01T00:00:00Z'` será. |
|originId|String|O identificador exclusivo deste ambiente no sistema de origem.|
|originSystem|String|O tipo do recurso no sistema de origem, como `SharePointOnline` . Oferece suporte para `$filter`.|

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
  "baseType": "",
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
