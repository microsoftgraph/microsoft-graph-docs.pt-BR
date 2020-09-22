---
title: tipo de recurso Employees
description: Um objeto Employee no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: d404a1ede257f3a31371dba31c37ff329452fccd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071336"
---
# <a name="employees-resource-type"></a>tipo de recurso Employees

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um funcionário no Dynamics 365 Business central.

## <a name="methods"></a>Métodos

| Método                                              | Tipo de retorno|Descrição               |
|:----------------------------------------------------|:-----------|:-------------------------|
|[Obter funcionários](../api/dynamics-employee-get.md)      |dos  |Obter um objeto Employee.   |
|[Postar funcionários](../api/dynamics-create-employee.md)  |dos  |Criar um objeto Employee.|
|[Patch funcionários](../api/dynamics-employee-update.md) |dos  |Atualizar um objeto Employee.|
|[Excluir funcionários](../api/dynamics-employee-delete.md)|Nenhuma       |Excluir um objeto Employee.|

## <a name="properties"></a>Propriedades
| Propriedade           | Tipo   |Descrição                                            |
|:-------------------|:-------|:------------------------------------------------------|
|id                  |GUID    |A ID do funcionário. Não editável.                         |
|number              |cadeia de caracteres  |O número do funcionário. Somente Leitura.                        |
|displayName         |cadeia de caracteres  |O funcionário de atribuído + sobrenome. Somente Leitura.           |
|givenName           |cadeia de caracteres  |O nome fornecido do funcionário.                        |
|middleName          |cadeia de caracteres  |O nome do meio do funcionário.                       |
|surname             |cadeia de caracteres  |O sobrenome do funcionário                            |
|jobTitle            |cadeia de caracteres  |O nome completo do funcionário                          |
|address             |[Extra. Address](../resources/dynamics-complextypes.md)|Especifica o endereço do funcionário. Esse endereço aparecerá em todos os documentos de recursos do funcionário.|
|phoneNumber         |cadeia de caracteres  |Especifica o número de telefone do funcionário.             |
|mobilePhone         |cadeia de caracteres  |Especifica o número de telefone celular do funcionário.      |
|email               |cadeia de caracteres  |Especifica o endereço de email do funcionário.                |
|personalEmail       |cadeia de caracteres  |Especifica o endereço de email pessoal do funcionário.       |
|employmentDate      |data    |Especifica a data em que o funcionário começou a trabalhar para a empresa.|
|terminationDate     |data    |Especifica a data de término do funcionário, devido à aposentadoria ou à descarta, por exemplo.|
|status              |cadeia de caracteres  |Especifica o status do funcionário. Os valores possíveis estão ativos, inativos ou terminados|
|birthDate           |data    |Especifica a data de nascimento do funcionário.                |
|Panorama             |stream  |A imagem do funcionário. Somente Leitura.                       |
|lastModifiedDateTime|datetime|O último DateTime que o funcionário foi modificado. Somente leitura.|  


## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.


```json
{
    "id": "GUID",
    "number": "string",
    "displayName": "string",
    "givenName": "string",
    "middleName": "string",
    "surname": "string",
    "jobTitle": "string",
    "address": "NAV.PostalAddress",
    "phoneNumber": "string",
    "mobilePhone": "string",
    "email": "string",
    "personalEmail": "string",
    "employmentDate": "date",
    "terminationDate": "date",
    "status": "string",
    "birthDate": "date",
    "picture": "stream",
    "lastModifiedDateTime": "datetime"
}

```



