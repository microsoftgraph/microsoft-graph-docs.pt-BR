---
title: Tipo de recurso accessPackageResourceEnvironment
description: Um ambiente de recurso do pacote de acesso é uma referência ao ambiente de localização geográfica no qual um recurso está localizado.
author: hanki-microsoft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 0a1d9362371b9a479d12ba6613e49854283bd610
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651193"
---
# <a name="accesspackageresourceenvironment-resource-type"></a>Tipo de recurso accessPackageResourceEnvironment

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No [Azure AD Entitlement Management](entitlementmanagement-overview.md), um ambiente de recurso do pacote de acesso é uma referência ao ambiente de localização geográfica no qual um recurso está localizado. Esse ambiente é fornecido automaticamente como parte do Gerenciamento de Direitos do Azure AD. A API só é aplicável a sites multi-SharePoint Online.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar accessPackageResourceEnvironments](../api/entitlementmanagement-list-accesspackageresourceenvironment.md)|[coleção accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md)|Recupere uma lista de [objetos accessPackageResourceEnvironment.](../resources/accesspackageresourceenvironment.md)|
|[Obter accessPackageResourceEnvironment](../api/accesspackageresourceenvironment-get.md)|[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md)|Leia as propriedades e as relações de um [objeto accessPackageResourceEnvironment.](../resources/accesspackageresourceenvironment.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|connectionInfo|[connectionInfo](../resources/connectioninfo.md)|Informações de conexão de um ambiente usado para se conectar a um recurso. |
|createdBy|Cadeia de caracteres|O nome de exibição do usuário que criou esse objeto.|
|createdDateTime|DateTimeOffset|A data e a hora em que esse objeto foi criado. <br>O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|descrição|String|A descrição desse objeto.|
|displayName|String|O nome de exibição deste objeto.|
|id|String|O identificador exclusivo atribuído pelo sistema do objeto.|
|isDefaultEnvironment|Booliano|Determina se esse é o ambiente padrão ou não. Ele é definido como `true` para todos os sistemas de origem estática, como grupos do Azure AD e Aplicativos do Azure AD.|
|modifiedBy|String|O nome de exibição da entidade que modificou esse objeto pela última vez.|
|modifiedDateTime|DateTimeOffset|A data e a hora em que esse objeto foi modificado pela última vez. <br>O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. |
|originId|String|O identificador exclusivo desse ambiente no sistema de origem.|
|originSystem|String|O tipo do recurso no sistema de origem, ou seja, `SharePointOnline` . Requer `$filter` ( `eq` ).|

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
