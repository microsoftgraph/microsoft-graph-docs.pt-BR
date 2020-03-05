---
title: tipo de recurso companyInformation
description: Informações da empresa no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: ce982e7d03e4b2e5947381173d57706f6cf8f41e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42505123"
---
# <a name="companyinformation-resource-type"></a>tipo de recurso companyInformation

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as informações especificadas para a empresa atual no Dynamics 365 Business central, como nome, endereço, endereço de email e endereço do site.

## <a name="methods"></a>Métodos

| Método         | Tipo de retorno  |Descrição|
|:---------------|:-------------|:----------|
|[Obter companyInformation](../api/dynamics-companyinformation-get.md)|companyInformation|Obtém informações da empresa.|
|[Patch companyInformation](../api/dynamics-companyinformation-update.md)|companyInformation|Atualiza as informações da empresa.|


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo      |Descrição                           |
|:-------------|:--------|:-------------------------------------|
|id            |GUID|A identificação exclusiva da empresa. Não editável.|
|displayName   |string   |O nome de exibição da empresa.           |
|address       |[Extra. Address](../resources/dynamics-complextypes.md)|O endereço da empresa. Exiba o tipo complexo para obter detalhes adicionais.|
|phoneNumber   |string   |O número de telefone da empresa.       |
|faxNumber     |string   |O número de fax da empresa.             |
|email         |cadeia de caracteres   |O endereço de email da empresa.          |
|site       |string   |O endereço do site da empresa.        |
|taxRegistrationNumber|string|O número de registro de imposto da empresa.|
|currencyCode  |string   |A moeda na qual a empresa faz negócios. Somente Leitura.|
|currentFiscalYearStartDate|data|A data de início do ano fiscal atual da empresa. Somente Leitura.|
|indústria      |string   |O setor do qual a empresa faz parte.  |
|Panorama       |stream   |O logotipo da empresa. Somente Leitura.          |
|businessProfileId|string|A ID do perfil de negócios vinculada à empresa financeira. Somente Leitura.|
|lastModifiedDateTime|datetime|O último DateTime que a empresa foi modificada. Somente leitura.|  


## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do companyInformation
```json
{
  "id": "GUID",
  "displayName": "string",
  "address": "NAV.PostalAddress",
  "phoneNumber": "string",
  "faxNumber": "string",
  "email": "string",
  "website": "string",
  "taxRegistrationNumber": "string",
  "currencyCode": "string",
  "currentFiscalYearStartDate": "date",
  "industry": "string",
  "picture": "stream",
  "businessProfileId": "string",
  "lastModifiedDateTime": "datetime"
}

```

