---
title: Tipo de recurso joinMeetingIdSettings
description: Especifica o joinMeetingId, a senha da reunião e o requisito para a senha.
author: yuyaolian-msft
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: fc954abe7c265c864587fdc5c2c6150c78374970
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645584"
---
# <a name="joinmeetingidsettings-resource-type"></a>Tipo de recurso joinMeetingIdSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Especifica o **joinMeetingId**, a senha da reunião e o requisito para a senha de uma reunião online.

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo      | Descrição                                   |
|:--------------------|:----------|:----------------------------------------------|
| isPasscodeRequired  | Booleano   | Indica se uma senha é necessária para ingressar em uma reunião ao usar **joinMeetingId**. Opcional. |
| joinMeetingId       | Cadeia de Caracteres    | A ID da reunião a ser usada para ingressar em uma reunião. Opcional. Somente leitura. |
| senha            | Cadeia de caracteres    | A senha para ingressar em uma reunião.  Opcional. Somente leitura. |
## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.joinMeetingIdSettings"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.joinMeetingIdSettings",
  "isPasscodeRequired": "Boolean",
  "joinMeetingId": "String",
  "passcode": "String"
}
```
