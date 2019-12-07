---
title: tipo de recurso workforceIntegrationEncryption
description: Uma entidade de criptografia que define o protocolo e o segredo para uma integração de força de funcionários.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 52fb72380ce74acad429aa3da6f9ad4e60102e06
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895560"
---
# <a name="workforceintegrationencryption-resource-type"></a><span data-ttu-id="f0885-103">tipo de recurso workforceIntegrationEncryption</span><span class="sxs-lookup"><span data-stu-id="f0885-103">workforceIntegrationEncryption resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0885-104">Uma entidade de criptografia que define o protocolo e o segredo de um [workforceintegration](../resources/workforceintegration.md).</span><span class="sxs-lookup"><span data-stu-id="f0885-104">An encryption entity defining the protocol and secret for a [workforceintegration](../resources/workforceintegration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f0885-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f0885-105">Properties</span></span>

| <span data-ttu-id="f0885-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f0885-106">Property</span></span>     | <span data-ttu-id="f0885-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0885-107">Type</span></span>        | <span data-ttu-id="f0885-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0885-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f0885-109">RDP</span><span class="sxs-lookup"><span data-stu-id="f0885-109">protocol</span></span>|<span data-ttu-id="f0885-110">String</span><span class="sxs-lookup"><span data-stu-id="f0885-110">String</span></span>| <span data-ttu-id="f0885-111">Os valores possíveis são: `sharedSecret` e `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="f0885-111">Possible values are: `sharedSecret`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="f0885-112">sigilo</span><span class="sxs-lookup"><span data-stu-id="f0885-112">secret</span></span>|<span data-ttu-id="f0885-113">String</span><span class="sxs-lookup"><span data-stu-id="f0885-113">String</span></span>|<span data-ttu-id="f0885-114">Segredo compartilhado de criptografia.</span><span class="sxs-lookup"><span data-stu-id="f0885-114">Encryption shared secret.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f0885-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f0885-115">JSON representation</span></span>

<span data-ttu-id="f0885-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f0885-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workforceIntegrationEncryption",
  "baseType": null
}-->

```json
{
  "protocol": "String",
  "secret": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workforceIntegrationEncryption resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
