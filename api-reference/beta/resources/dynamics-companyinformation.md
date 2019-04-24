---
title: tipo de recurso companyInformation
description: Informações da empresa no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 0f8671cbade11cc9db6bf797c39eb17acf286ef7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507270"
---
# <a name="companyinformation-resource-type"></a>tipo de recurso companyInformation
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
|FaxNumber     |string   |O número de fax da empresa.             |
|email         |string   |O endereço de email da empresa.          |
|site       |string   |O endereço do site da empresa.        |
|taxRegistrationNumber|string|O número de registro de imposto da empresa.|
|currencyCode  |string   |A moeda na qual a empresa faz negócios. Somente Leitura.|
|currentFiscalYearStartDate|data|A data de início do ano fiscal atual da empresa. Somente Leitura.|
|indústria      |string   |O setor do qual a empresa faz parte.  |
|Panorama       |stream   |O logotipo da empresa. Somente Leitura.          |
|businessProfileId|string|A ID do perfil de negócios vinculada à empresa financeira. Somente Leitura.|
|lastModifiedDateTime|DateTime|O último DateTime que a empresa foi modificada. Somente leitura.|  


## <a name="relationships"></a>Relações
Nenhuma

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

