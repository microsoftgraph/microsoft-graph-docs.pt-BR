---
title: Tipo de recurso tenantDetailedInformation
description: Representa informações detalhadas para um locatário gerenciado.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: d896492c05223fdf4711842340df5032589913d9
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61828842"
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
|city|String|A cidade onde o locatário gerenciado está localizado. Opcional. Somente leitura.|
|countryCode|String|O código do país onde o locatário gerenciado está localizado. Opcional. Somente leitura.|
|countryName|String|O nome do país onde o locatário gerenciado está localizado. Opcional. Somente leitura.|
|defaultDomainName|String|O nome de domínio padrão para o locatário gerenciado. Opcional. Somente leitura.|
|displayName|String|O nome de exibição do locatário gerenciado.|
|id|String|O identificador exclusivo dessa entidade. Obrigatório. Somente leitura.|
|industryName|String|O setor comercial associado ao locatário gerenciado. Opcional. Somente leitura.|
|region|String|A região onde o locatário gerenciado está localizado. Opcional. Somente leitura.|
|segmentName|String|O segmento de negócios associado ao locatário gerenciado. Opcional. Somente leitura.|
|tenantId|String|O Azure Active Directory do locatário para o [locatário gerenciado.](../resources/managedtenants-tenant.md)|
|verticalName|String|A vertical associada ao locatário gerenciado. Opcional. Somente leitura.|

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

