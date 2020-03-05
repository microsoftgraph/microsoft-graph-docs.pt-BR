---
title: tipo de recurso fornecedores
description: Um objeto fornecedor no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: d05b30dbbb5ecb6aa8a1934a5fe2a1b35cbe890b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502855"
---
# <a name="vendors-resource-type"></a>tipo de recurso fornecedores

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um fornecedor no Dynamics 365 Business central.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter fornecedores](../api/dynamics-vendor-get.md)|fornecedor|Obtém um objeto fornecedor.|
|[Lançar fornecedores](../api/dynamics-create-vendor.md)|fornecedor|Cria um objeto fornecedor.|
|[Fornecedores de patch](../api/dynamics-vendor-update.md)|fornecedor|Atualiza um objeto fornecedor.|
|[Excluir fornecedor](../api/dynamics-vendor-delete.md)|nenhuma|Exclui um objeto fornecedor.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|GUID|A ID exclusiva do fornecedor. Não editável.|
|number|string|O número do fornecedor.|
|displayName|string|O nome de exibição do fornecedor.|
|address|[Extra. Address](../resources/dynamics-complextypes.md)|O endereço do fornecedor.|
|phoneNumber|string|O número de telefone do fornecedor.|
|email|cadeia de caracteres|O endereço de email do fornecedor.|
|site|string|O endereço do site do fornecedor.|
|taxRegistrationNumber|string|O número de registro de imposto do fornecedor.|
|CurrencyID|GUID|A ID do código de moeda padrão do fornecedor.|
|currencyCode|string|O código de moeda padrão do fornecedor.|
|irs1099Code|string|Especifica um código 1099 para o fornecedor. Somente EUA.|
|paymentTermsId|GUID|A ID padrão dos termos de pagamento do fornecedor.|
|paymentMethodId|GUID|A ID de método de pagamento padrão para o fornecedor.|
|taxLiable|booliano|Especifica se o fornecedor é responsável por impostos.|
|bloqueou|string|Especifica quais transações com o fornecedor que não podem ser lançados. Os valores aceitos estão em branco, pagamento ou todos|
|carga|dígitos|O saldo do fornecedor. Somente Leitura.|
|lastModifiedDateTime|datetime|O último DateTime que o fornecedor foi modificado. Somente leitura.|  


## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do fornecedor.

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

