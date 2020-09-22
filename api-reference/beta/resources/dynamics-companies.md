---
title: tipo de recurso de empresas
description: Uma empresa no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 3fedbd9407a4124c38a6ff08a95dbf4cd22c9fe1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081759"
---
# <a name="companies-resource-type"></a>tipo de recurso de empresas

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um tipo de recurso de empresas no Dynamics 365 Business central. 

## <a name="methods"></a>Métodos

| Método         | Tipo de retorno  |Descrição|
|:---------------|:-------------|:----------|
|[Obter empresas](../api/dynamics-companies-get.md)|companhias|Obter uma empresa.|

## <a name="properties"></a>Propriedades
| Propriedade        | Tipo |Descrição                             |
|:----------------|:-----|:---------------------------------------|
|id               |GUID  |A identificação exclusiva da empresa. Somente Leitura.|
|name             |string|Especifica a empresa.                  |
|displayName      |cadeia de caracteres|Especifica o nome de exibição da empresa.     |
|systemVersion    |cadeia de caracteres|Especifica a versão interna da empresa.|
|businessProfileId|cadeia de caracteres|Especifica a ID do perfil de negócios vinculada à empresa.|


## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON da empresa.

```json
{
  "id": "GUID",
  "name": "string",
  "displayName": "string",
  "systemVersion": "string",
  "businessProfileId": "string"
}

```




