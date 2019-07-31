---
title: tipo de recurso securityVendorInformation
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: e6f543a85ac2974f9b3e99d4290fb9d93a8cc025
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965212"
---
# <a name="securityvendorinformation-resource-type"></a>tipo de recurso securityVendorInformation

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém detalhes sobre o fornecedor de produtos/serviços de segurança, o provedor e o subfornecedor (por exemplo, fornecedor = Microsoft; Provider = Windows Defender ATP; subfornecedor = AppLocker).

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|provedor |String|Provedor específico (produto/serviço – empresa de fornecedor); por exemplo, WindowsDefenderATP.|
|providerVersion|String|Versão do provedor ou do subfornecedor, se existir, que gerou o alerta. **Required**|
|subprovedor|String|Subfornecedor específico (em provedor de agregação); por exemplo, WindowsDefenderATP. SmartScreen.|
|fornecedor |String|Nome do fornecedor do alerta (por exemplo, Microsoft, Dell, FireEye). **Required**|

## <a name="json-representation"></a>Representação JSON

O folllowing é uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityVendorInformation"
}-->

```json
{
  "provider": "String",
  "providerVersion": "String",
  "subProvider": "String",
  "vendor": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "securityVendorInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
