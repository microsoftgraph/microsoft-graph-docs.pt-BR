---
title: Tipo de recurso delegatedAdminCustomer
description: Representa um cliente que tem uma relação de administrador delegado com um parceiro da Microsoft.
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: resourcePageType
ms.openlocfilehash: 4d86eb070a72102aee490321bc854ea319467fab
ms.sourcegitcommit: 5a43129dbf705f2d1a6afcff36af9f41ecee026d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2022
ms.locfileid: "64704186"
---
# <a name="delegatedadmincustomer-resource-type"></a>Tipo de recurso delegatedAdminCustomer

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma organização do Azure AD que é cliente de um parceiro da Microsoft e tem uma relação de administrador delegado com o parceiro da Microsoft. Esse objeto é criado automaticamente pelo sistema quando pelo menos uma relação de administrador delegado existe entre o parceiro e o cliente e é excluído quando não há mais relações ativas.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar delegatedAdminCustomers](../api/tenantrelationship-list-delegatedadmincustomers.md)|[coleção delegatedAdminCustomer](delegatedadmincustomer.md)|Obtenha uma lista dos **objetos delegatedAdminCustomer** e suas propriedades.|
|[Obter delegatedAdminCustomer](../api/delegatedadmincustomer-get.md)|[delegatedAdminCustomer](delegatedadmincustomer.md)|Leia as propriedades e as relações de um **objeto delegatedAdminCustomer** .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|O nome de exibição do locatário do cliente no Azure AD. Somente leitura. Oferece suporte para `$orderBy`. |
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
