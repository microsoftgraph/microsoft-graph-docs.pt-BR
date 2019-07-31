---
title: tipo de recurso fornecedores
description: Um objeto fornecedor no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 7c0609d96f6d97503faf5c5251d3641979a4f6e8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972849"
---
# <a name="vendors-resource-type"></a>tipo de recurso fornecedores
Representa um fornecedor no Dynamics 365 Business central.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter fornecedores](../api/dynamics-vendor-get.md)|fornecedor|Obtém um objeto fornecedor.|
|[Lançar fornecedores](../api/dynamics-create-vendor.md)|fornecedor|Cria um objeto fornecedor.|
|[Fornecedores de patch](../api/dynamics-vendor-update.md)|fornecedor|Atualiza um objeto fornecedor.|
|[Excluir fornecedor](../api/dynamics-vendor-delete.md)|none|Exclui um objeto fornecedor.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|GUID|A ID exclusiva do fornecedor. Não editável.|
|number|string|O número do fornecedor.|
|displayName|string|O nome de exibição do fornecedor.|
|address|[Extra. Address](../resources/dynamics-complextypes.md)|O endereço do fornecedor.|
|phoneNumber|string|O número de telefone do fornecedor.|
|email|string|O endereço de email do fornecedor.|
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
|lastModifiedDateTime|DateTime|O último DateTime que o fornecedor foi modificado. Somente leitura.|  


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

