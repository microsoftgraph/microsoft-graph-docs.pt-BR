---
title: Tipo de recurso externalMeetingRegistrant
description: Representa um registro de reunião externo que se registrou em uma reunião online.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 05c386137ea9e062e223eb7854afc4d13458fe30
ms.sourcegitcommit: ba46f9f77d1e0eb9c7f5b2f4366534bfcf99d9c0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2021
ms.locfileid: "61565153"
---
# <a name="externalmeetingregistrant-resource-type"></a>Tipo de recurso externalMeetingRegistrant

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um registro de reunião externo que se registrou em uma reunião online.

Herda de [meetingRegistrantBase](../resources/meetingregistrantbase.md).

## <a name="methods"></a>Methods

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar externalMeetingRegistrants](../api/externalmeetingregistrant-list.md)|[Coleção externalMeetingRegistrant](../resources/externalmeetingregistrant.md)|Obter uma lista dos [objetos externalMeetingRegistrant](../resources/externalmeetingregistrant.md) e suas propriedades.|
|[Criar externalMeetingRegistrant](../api/externalmeetingregistrant-post.md)|[externalMeetingRegistrant](../resources/externalmeetingregistrant.md)|Leia as propriedades e as relações de um [objeto externalMeetingRegistrant.](../resources/externalmeetingregistrant.md)|
|[Excluir externalMeetingRegistrant](../api/externalmeetingregistrant-delete.md)|Nenhum|[Exclua um objeto externalMeetingRegistrant.](../resources/externalmeetingregistrant.md)|

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo   | Descrição                                                                  |
|:-----------|:-------|:-----------------------------------------------------------------------------|
| id         | Cadeia de caracteres | O identificador exclusivo do registro no sistema de registro externo. Herdado [de meetingRegistrantBase](../resources/meetingregistrantbase.md). |
| joinWebUrl | Cadeia de caracteres | Uma URL da Web exclusiva para o registro ingressar na reunião. Herdado [de meetingRegistrantBase](../resources/meetingregistrantbase.md). Somente leitura.          |
| tenantId   | String | A ID do locatário desse registro se estiver Azure Active Directory.               |
| userId     | Cadeia de caracteres | A ID do usuário desse registro se estiver Azure Active Directory.                 |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalMeetingRegistrant",
  "baseType": "microsoft.graph.meetingRegistrantBase",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.externalMeetingRegistrant",
  "id": "String (identifier)",
  "joinWebUrl": "String",
  "userId": "String",
  "tenantId": "String"
}
```
