---
title: tipo de recurso de funcionários
description: Um objeto de funcionário no Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: eceea9e1811b61045c03fb8dc5d7710f33158ccc
ms.sourcegitcommit: a9a035e7cf7b500aebe5477c05361552e7c3a7ab
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/28/2021
ms.locfileid: "52695970"
---
# <a name="employees-resource-type"></a>tipo de recurso de funcionários

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um funcionário no Dynamics 365 Business Central.

## <a name="methods"></a>Métodos

| Método                                              | Tipo de retorno|Descrição               |
|:----------------------------------------------------|:-----------|:-------------------------|
|[Obter funcionários](../api/dynamics-employee-get.md)      |employees  |Obter um objeto de funcionário.   |
|[Funcionários de postagem](../api/dynamics-create-employee.md)  |employees  |Crie um objeto de funcionário.|
|[Corrigir funcionários](../api/dynamics-employee-update.md) |employees  |Atualizar um objeto de funcionário.|
|[Excluir funcionários](../api/dynamics-employee-delete.md)|nenhuma       |Excluir um objeto de funcionário.|

## <a name="properties"></a>Propriedades
| Propriedade           | Tipo   |Descrição                                            |
|:-------------------|:-------|:------------------------------------------------------|
|id                  |GUID    |A ID do funcionário. Não editável.                         |
|number              |cadeia de caracteres  |O número do funcionário. Somente Leitura.                        |
|displayName         |cadeia de caracteres  |O funcionário givenName + sobrenome. Somente Leitura.           |
|givenName           |cadeia de caracteres  |O nome dado do funcionário.                        |
|middleName          |cadeia de caracteres  |O nome do meio do funcionário.                       |
|surname             |cadeia de caracteres  |O sobrenome do funcionário                            |
|jobTitle            |cadeia de caracteres  |O cargo do funcionário                          |
|address             |[NAV. PostalAddress](../resources/dynamics-complextypes.md)|Especifica o endereço do funcionário. Esse endereço aparecerá em todos os documentos de recursos do funcionário.|
|phoneNumber         |cadeia de caracteres  |Especifica o número de telefone do funcionário.             |
|mobilePhone         |cadeia de caracteres  |Especifica o número de telefone celular do funcionário.      |
|email               |cadeia de caracteres  |Especifica o endereço de email do funcionário.                |
|personalEmail       |cadeia de caracteres  |Especifica o endereço de email pessoal do funcionário.       |
|employmentDate      |data    |Especifica a data em que o funcionário começou a trabalhar para a empresa.|
|terminationDate     |data    |Especifica a data em que o funcionário foi encerrado, devido à aposentadoria ou à demissão, por exemplo.|
|status              |cadeia de caracteres  |Especifica o status do funcionário. Os valores possíveis são Active, Inactive ou Terminated|
|birthDate           |data    |Especifica a data de nascimento do funcionário.                |
|picture             |stream  |A imagem do funcionário. Somente Leitura.                       |
|lastModifiedDateTime|datetime|A última data em que o funcionário foi modificado. Somente leitura.|  


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



