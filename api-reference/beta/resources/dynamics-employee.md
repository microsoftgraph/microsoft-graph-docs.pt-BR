---
title: tipo de recurso Employees
description: Um objeto Employee no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 865da0c1e1256e2ba2a25902e37a00da9081eedf
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366652"
---
# <a name="employees-resource-type"></a>tipo de recurso Employees
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
|number              |string  |O número do funcionário. Somente Leitura.                        |
|displayName         |string  |O funcionário de atribuído + sobrenome. Somente Leitura.           |
|givenName           |string  |O nome fornecido do funcionário.                        |
|middleName          |string  |O nome do meio do funcionário.                       |
|surname             |string  |O sobrenome do funcionário                            |
|jobTitle            |string  |O nome completo do funcionário                          |
|address             |[Extra. Address](../resources/dynamics-complextypes.md)|Especifica o endereço do funcionário. Esse endereço aparecerá em todos os documentos de recursos do funcionário.|
|phoneNumber         |string  |Especifica o número de telefone do funcionário.             |
|mobilePhone         |string  |Especifica o número de telefone celular do funcionário.      |
|email               |string  |Especifica o endereço de email do funcionário.                |
|personalEmail       |string  |Especifica o endereço de email pessoal do funcionário.       |
|employmentDate      |data    |Especifica a data em que o funcionário começou a trabalhar para a empresa.|
|terminationDate     |data    |Especifica a data de término do funcionário, devido à aposentadoria ou à descarta, por exemplo.|
|status              |cadeia de caracteres  |Especifica o status do funcionário. Os valores possíveis estão ativos, inativos ou terminados|
|birthDate           |data    |Especifica a data de nascimento do funcionário.                |
|Panorama             |stream  |A imagem do funcionário. Somente Leitura.                       |
|lastModifiedDateTime|DateTime|O último DateTime que o funcionário foi modificado. Somente Leitura.|  


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

