---
title: Tipo de recurso tenantCustomizedInformation
description: Representa informações personalizáveis para um locatário gerenciado.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 4b6ad664b8b3bf42cf9fef2410ed0f9eac58e464
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61860947"
---
# <a name="tenantcustomizedinformation-resource-type"></a>Tipo de recurso tenantCustomizedInformation

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações personalizáveis para um locatário gerenciado.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar tenantCustomizedInformations](../api/managedtenants-managedtenant-list-tenantscustomizedinformation.md)|[coleção microsoft.graph.managedTenants.tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md)|Obter uma lista dos [objetos tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) e suas propriedades.|
|[Obter tenantCustomizedInformation](../api/managedtenants-tenantcustomizedinformation-get.md)|[microsoft.graph.managedTenants.tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md)|Leia as propriedades e as relações de um [objeto tenantCustomizedInformation.](../resources/managedtenants-tenantcustomizedinformation.md)|
|[Atualizar tenantCustomizedInformation](../api/managedtenants-tenantcustomizedinformation-update.md)|[microsoft.graph.managedTenants.tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md)|Atualize as propriedades de [um objeto tenantCustomizedInformation.](../resources/managedtenants-tenantcustomizedinformation.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|contacts|[coleção microsoft.graph.managedTenants.tenantContactInformation](../resources/managedtenants-tenantcontactinformation.md)|A coleção de contatos do locatário gerenciado. Opcional.|
|displayName|String|O nome de exibição do locatário gerenciado. Obrigatório. Somente leitura.|
|id|String|O Azure Active Directory de locatário do locatário gerenciado. Obrigatório. Somente leitura.|
|tenantId|String|O Azure Active Directory do locatário para o [locatário gerenciado.](../resources/managedtenants-tenant.md) Opcional. Somente leitura.|
|site|String|O site do locatário gerenciado. Obrigatório.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.tenantCustomizedInformation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenantCustomizedInformation",
  "id": "String (identifier)",
  "displayName": "String",
  "tenantId": "String",
  "contacts": [
    {
      "@odata.type": "microsoft.graph.managedTenants.tenantContactInformation"
    }
  ],
  "website": "String"
}
```
