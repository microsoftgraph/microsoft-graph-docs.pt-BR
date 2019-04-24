---
title: tipo de recurso de contas
description: Um objeto Account no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 4252c20e9d11f67a6de40871b1649a165cbd787c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507571"
---
# <a name="accounts-resource-type"></a>tipo de recurso de contas
Representa um objeto Account no Dynamics 365 Business central.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter contas](../api/dynamics-account-get.md)|las|Obtém o objeto accounts.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|GUID|A identificação exclusiva da conta.|
|number|Cadeia de caracteres, tamanho máximo 20|Especifica o número da conta G/L.|
|displayName|Cadeia de caracteres, tamanho máximo 50|Especifica o nome da conta de G/L.|
|Ferramentas para desenvolvedores|Cadeia de caracteres, tamanho máximo 20|Especifica a categoria da conta de G/L.|
|Subcategoria|Cadeia de caracteres, tamanho máximo 80|Especifica a subcategoria da categoria de conta da conta G/L.|
|bloqueou|booliano|Especifica que não é possível postar entradas na conta G/L. **True** indica que a conta está bloqueada e o lançamento não é permitido.|
|lastModifiedDateTime|DateTime|O último DateTime que a conta foi modificada.|


## <a name="relationships"></a>Relações
Nenhuma

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.


```json
{
  "id": "GUID",
  "number": "string",
  "displayName": "string",
  "category": "string",
  "subCategory": "string",
  "blocked": "boolean",
  "lastModifiedDateTime": "datetime"
}

```
