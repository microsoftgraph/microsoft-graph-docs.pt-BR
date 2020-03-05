---
title: tipo de recurso de empresas
description: Uma empresa no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 13bc765f873bc893925ffbddc82b2f0685376cf6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42505137"
---
# <a name="companies-resource-type"></a>tipo de recurso de empresas

Namespace: Microsoft. Graph

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
|nome             |string|Especifica a empresa.                  |
|displayName      |string|Especifica o nome de exibição da empresa.     |
|systemVersion    |string|Especifica a versão interna da empresa.|
|businessProfileId|string|Especifica a ID do perfil de negócios vinculada à empresa.|


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


