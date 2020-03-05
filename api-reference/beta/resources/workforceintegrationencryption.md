---
title: tipo de recurso workforceIntegrationEncryption
description: Uma entidade de criptografia que define o protocolo e o segredo para uma integração de força de funcionários.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c2d24371a0a999069d80a9ad86afd48ac9e68d38
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519075"
---
# <a name="workforceintegrationencryption-resource-type"></a><span data-ttu-id="7183c-103">tipo de recurso workforceIntegrationEncryption</span><span class="sxs-lookup"><span data-stu-id="7183c-103">workforceIntegrationEncryption resource type</span></span>

<span data-ttu-id="7183c-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7183c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7183c-105">Uma entidade de criptografia que define o protocolo e o segredo de um [workforceintegration](../resources/workforceintegration.md).</span><span class="sxs-lookup"><span data-stu-id="7183c-105">An encryption entity defining the protocol and secret for a [workforceintegration](../resources/workforceintegration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7183c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7183c-106">Properties</span></span>

| <span data-ttu-id="7183c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7183c-107">Property</span></span>     | <span data-ttu-id="7183c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="7183c-108">Type</span></span>        | <span data-ttu-id="7183c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7183c-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7183c-110">RDP</span><span class="sxs-lookup"><span data-stu-id="7183c-110">protocol</span></span>|<span data-ttu-id="7183c-111">String</span><span class="sxs-lookup"><span data-stu-id="7183c-111">String</span></span>| <span data-ttu-id="7183c-112">Os valores possíveis são: `sharedSecret` e `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="7183c-112">Possible values are: `sharedSecret`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="7183c-113">sigilo</span><span class="sxs-lookup"><span data-stu-id="7183c-113">secret</span></span>|<span data-ttu-id="7183c-114">String</span><span class="sxs-lookup"><span data-stu-id="7183c-114">String</span></span>|<span data-ttu-id="7183c-115">Segredo compartilhado de criptografia.</span><span class="sxs-lookup"><span data-stu-id="7183c-115">Encryption shared secret.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7183c-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7183c-116">JSON representation</span></span>

<span data-ttu-id="7183c-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7183c-117">The following is a JSON representation of the resource.</span></span>

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
