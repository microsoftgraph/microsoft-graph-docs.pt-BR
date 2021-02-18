---
title: tipo de recurso vendors
description: Um objeto de fornecedor no Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 0848b6fbb67964faa9565f2ed95120f563c71f53
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50293068"
---
# <a name="vendors-resource-type"></a>tipo de recurso vendors

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um fornecedor no Dynamics 365 Business Central.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter fornecedores](../api/dynamics-vendor-get.md)|vendors|Obtém um objeto de fornecedor.|
|[Post vendors](../api/dynamics-create-vendor.md)|vendors|Cria um objeto de fornecedor.|
|[Fornecedores de patch](../api/dynamics-vendor-update.md)|vendors|Atualiza um objeto de fornecedor.|
|[Excluir fornecedor](../api/dynamics-vendor-delete.md)|nenhum|Exclui um objeto de fornecedor.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|GUID|A ID exclusiva do fornecedor. Não editável.|
|number|cadeia de caracteres|O número do fornecedor.|
|displayName|cadeia de caracteres|O nome de exibição do fornecedor.|
|address|[NAV. PostalAddress](../resources/dynamics-complextypes.md)|O endereço do fornecedor.|
|phoneNumber|cadeia de caracteres|O número de telefone do fornecedor.|
|email|cadeia de caracteres|O endereço de email do fornecedor.|
|site|cadeia de caracteres|O endereço do site do fornecedor.|
|taxRegistrationNumber|cadeia de caracteres|O número de registro fiscal do fornecedor.|
|currencyId|GUID|A ID de código de moeda padrão para o fornecedor.|
|currencyCode|cadeia de caracteres|O código de moeda padrão para o fornecedor.|
|irs1099Code|cadeia de caracteres|Especifica um código 1099 para o fornecedor. Somente eua.|
|paymentTermsId|GUID|A ID de termos de pagamento padrão para o fornecedor.|
|paymentMethodId|GUID|A ID de método de pagamento padrão para o fornecedor.|
|taxLiable|booliano|Especifica se o fornecedor é responsável pelo imposto.|
|bloqueado|cadeia de caracteres|Especifica quais transações com o fornecedor não podem ser publicadas. Os valores aceitos estão em branco, Pagamento ou Tudo|
|balance|decimal|O saldo do fornecedor. Somente Leitura.|
|lastModifiedDateTime|datetime|A última data em que o fornecedor foi modificado. Somente leitura.|  


## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.vendor"
}-->

Aqui está uma representação JSON do fornecedor.

```json
{
  "id": "GUID",
  "number": "string",
  "displayName": "string",
  "address": "NAV.PostalAddress",
  "phoneNumber": "string",
  "email": "string",
  "website": "string",
  "taxRegistrationNumber": "string",
  "currencyId": "GUID",
  "currencyCode": "string",
  "irs1099Code": "string",
  "paymentTermsId": "GUID",
  "paymentMethodId": "GUID",
  "taxLiable": "boolean",
  "blocked": "string",
  "balance": "decimal",
  "lastModifiedDateTime": "datetime"
}
```



