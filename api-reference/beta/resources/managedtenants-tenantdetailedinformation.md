---
title: Tipo de recurso tenantDetailedInformation
description: Representa informações detalhadas para um locatário gerenciado.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 40aa157b12ccef64b6eb7ab6c92349a3e74745f8
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401994"
---
# <a name="tenantdetailedinformation-resource-type"></a>Tipo de recurso tenantDetailedInformation

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações detalhadas para um locatário gerenciado.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar tenantDetailedInformation](../api/managedtenants-managedtenant-list-tenantsdetailedinformation.md)|[coleção microsoft.graph.managedTenants.tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md)|Obter uma lista dos [objetos tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md) e suas propriedades.|
|[Obter tenantDetailedInformation](../api/managedtenants-tenantdetailedinformation-get.md)|[microsoft.graph.managedTenants.tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md)|Leia as propriedades e as relações de um [objeto tenantDetailedInformation.](../resources/managedtenants-tenantdetailedinformation.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|city|Cadeia de caracteres|A cidade onde o locatário gerenciado está localizado. Opcional. Somente leitura.|
|countryCode|Cadeia de caracteres|O código do país onde o locatário gerenciado está localizado. Opcional. Somente leitura.|
|countryName|Cadeia de caracteres|O nome do país onde o locatário gerenciado está localizado. Opcional. Somente leitura.|
|defaultDomainName|Cadeia de caracteres|O nome de domínio padrão para o locatário gerenciado. Opcional. Somente leitura.|
|displayName|Cadeia de caracteres|O nome de exibição do locatário gerenciado.|
|id|Cadeia de caracteres|O identificador exclusivo dessa entidade. Obrigatório. Somente leitura.|
|industryName|Cadeia de caracteres|O setor comercial associado ao locatário gerenciado. Opcional. Somente leitura.|
|region|Cadeia de caracteres|A região onde o locatário gerenciado está localizado. Opcional. Somente leitura.|
|segmentName|Cadeia de caracteres|O segmento de negócios associado ao locatário gerenciado. Opcional. Somente leitura.|
|tenantId|String|O Azure Active Directory do locatário para o [locatário gerenciado.](../resources/managedtenants-tenant.md)|
|verticalName|Cadeia de caracteres|A vertical associada ao locatário gerenciado. Opcional. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.tenantDetailedInformation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenantDetailedInformation",
  "id": "String (identifier)",
  "tenantId": "String",
  "displayName": "String",
  "defaultDomainName": "String",
  "countryName": "String",
  "countryCode": "String",
  "city": "String",
  "region": "String",
  "verticalName": "String",
  "industryName": "String",
  "segmentName": "String"
}
```

