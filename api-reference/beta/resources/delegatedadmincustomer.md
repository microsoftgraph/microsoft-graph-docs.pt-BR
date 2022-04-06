---
title: Tipo de recurso delegatedAdminCustomer
description: Representa um cliente que tem uma relação de administrador delegada com um parceiro da Microsoft.
author: adtangir
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: b7ac3c580ab566565d99f7c7c542e2bee0f0bcc3
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589587"
---
# <a name="delegatedadmincustomer-resource-type"></a>Tipo de recurso delegatedAdminCustomer

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma organização do Azure AD que é cliente de um parceiro da Microsoft e tem uma relação de administrador delegada com o parceiro da Microsoft. Esse objeto é criado automaticamente pelo sistema quando há pelo menos uma relação de administrador delegado entre o parceiro e o cliente e é excluído quando não há mais relações ativas.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar delegatedAdminCustomers](../api/tenantrelationship-list-delegatedadmincustomers.md)|[coleção delegatedAdminCustomer](delegatedadmincustomer.md)|Obter uma lista dos **objetos delegatedAdminCustomer** e suas propriedades.|
|[Obter delegatedAdminCustomer](../api/delegatedadmincustomer-get.md)|[delegatedAdminCustomer](delegatedadmincustomer.md)|Leia as propriedades e as relações de um **objeto delegatedAdminCustomer** .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|O nome de exibição do Azure AD do locatário do cliente. Somente leitura. Oferece suporte para `$orderBy`. |
|id|Cadeia de caracteres|O identificador exclusivo atribuído ao Azure AD do cliente. Somente leitura. Herdado da [entidade](../resources/entity.md).|
|tenantId|String|A ID de locatário atribuída ao Azure AD do cliente. Somente leitura.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|serviceManagementDetails|[coleção delegatedAdminServiceManagementDetail](delegatedadminservicemanagementdetail.md)|Contém os detalhes de gerenciamento de um serviço no locatário do cliente gerenciado pela administração delegada.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.delegatedAdminCustomer",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.delegatedAdminCustomer",
  "id": "String (identifier)",
  "tenantId": "String",
  "displayName": "String"
}
```
