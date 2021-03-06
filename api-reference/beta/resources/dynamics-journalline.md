---
title: tipo de recurso journalLines
description: Uma linha de diário no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 99d06b5a49bd2881ea6f329e8b0d3692a25444b4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013794"
---
# <a name="journallines-resource-type"></a>tipo de recurso journalLines

Namespace: Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma linha em um diário no Dynamics 365 Business central.

## <a name="methods"></a>Methods

| Método                                                    | Tipo de retorno|Descrição         |
|:----------------------------------------------------------|:-----------|:-------------------|
|[Obter journalLines](../api/dynamics-journalline-get.md)      |journalLines|Obtém uma linha do diário.   |
|[Postar journalLines](../api/dynamics-create-journalline.md)  |journalLines|Cria uma linha de diário.|
|[Patch journalLines](../api/dynamics-journalline-update.md) |journalLines|Atualiza uma linha do diário.|
|[Excluir journalLines](../api/dynamics-journalline-delete.md)|Nenhuma        |Exclui uma linha do diário.|

## <a name="properties"></a>Propriedades
| Propriedade             | Tipo                   |Descrição                                                        |
|:---------------------|:-----------------------|:------------------------------------------------------------------|
|id                    |GUID                    |A identificação exclusiva da linha do diário. Não editável.                   |
|journalDisplayName    |Cadeia de caracteres, tamanho máximo 10 |O nome de exibição do diário ao qual esta linha pertence. Somente Leitura.|
|lineNumber            |inteiro                 |O número da linha do diário.                                    |
|accountId             |GUID                    |A identificação exclusiva da conta à qual a linha do diário está relacionada.  |
|accountNumber         |Cadeia de caracteres, tamanho máximo 20 |O número da conta à qual a linha do diário está relacionada.     |
|postingDate           |data                    |A data em que a linha do diário é lançada.                          |
|documentNumber        |Cadeia de caracteres, tamanho máximo 20 |Especifica um número de documento para a linha do diário.                  |
|externalDocumentNumber|Cadeia de caracteres, tamanho máximo 20 |Especifica um número de documento externo para a linha do diário.        |
|quantia                |dígitos                 |Especifica o valor total (incluindo o IVA) que a linha do diário consiste.|
|description           |Cadeia de caracteres, tamanho máximo 50 |A descrição da linha do diário, fornecida pelo usuário ou autocriada.|
|comment               |Cadeia de caracteres, tamanho máximo 250|Um comentário especificado pelo usuário na linha do diário.                      |
|lastModifiedDateTime  |datetime                |O último DateTime em que a linha do diário foi modificada. Somente leitura.        |

## <a name="relationships"></a>Relações
Uma linha de diário é uma subpágina de um diário. Ele não pode ser acessado diretamente.

Uma linha de diário pode ser uma "entidade pai" das linhas de dimensão.

Uma conta (AccountId) deve existir na tabela accounts.


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.


```json
{
    "id": "GUID",
    "journalDisplayName": "string",
    "lineNumber": "integer",
    "accountId": "GUID",
    "accountNumber": "string",
    "postingDate": "date",
    "documentNumber": "string",
    "externalDocumentNumber": "string",
    "amount": "decimal",
    "description": "string",
    "comment": "string",
    "lastModifiedDateTime": "datetime"
}
```


