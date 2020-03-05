---
title: tipo de recurso signInActivity
description: Fornece a última data de logon de um usuário específico.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8144a681f93df45827c8b304d507eea820adcca2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520594"
---
# <a name="signinactivity-resource-type"></a><span data-ttu-id="5523d-103">tipo de recurso signInActivity</span><span class="sxs-lookup"><span data-stu-id="5523d-103">signInActivity resource type</span></span>

<span data-ttu-id="5523d-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5523d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5523d-105">Fornece a última data de logon de um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="5523d-105">Provides the last signed-in date for a specific user.</span></span>

## <a name="properties"></a><span data-ttu-id="5523d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5523d-106">Properties</span></span>

| <span data-ttu-id="5523d-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5523d-107">Property</span></span>     | <span data-ttu-id="5523d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="5523d-108">Type</span></span>        | <span data-ttu-id="5523d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5523d-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5523d-110">lastSignInDateTime</span><span class="sxs-lookup"><span data-stu-id="5523d-110">lastSignInDateTime</span></span>|<span data-ttu-id="5523d-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5523d-111">DateTimeOffset</span></span>|<span data-ttu-id="5523d-112">A última data de entrada de um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="5523d-112">The last sign-in date for a specific user.</span></span> <span data-ttu-id="5523d-113">Você pode usar esse campo para calcular a última vez que um usuário entrou no diretório.</span><span class="sxs-lookup"><span data-stu-id="5523d-113">You can use this field to calculate the last time a user signed in to the directory.</span></span> <span data-ttu-id="5523d-114">Este campo pode ser usado para criar relatórios, como usuários inativos.</span><span class="sxs-lookup"><span data-stu-id="5523d-114">This field can be used to build reports, such as inactive users.</span></span> <span data-ttu-id="5523d-115">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="5523d-115">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5523d-116">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="5523d-116">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="5523d-117">lastSignInRequestId</span><span class="sxs-lookup"><span data-stu-id="5523d-117">lastSignInRequestId</span></span>|<span data-ttu-id="5523d-118">String</span><span class="sxs-lookup"><span data-stu-id="5523d-118">String</span></span>|<span data-ttu-id="5523d-119">ID da solicitação da última entrada realizada por esse usuário.</span><span class="sxs-lookup"><span data-stu-id="5523d-119">Request ID of the last sign-in performed by this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5523d-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5523d-120">JSON representation</span></span>

<span data-ttu-id="5523d-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5523d-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signInActivity",
  "baseType": null
}-->

```json
{
  "lastSignInDateTime": "String (timestamp)",
  "lastSignInRequestId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signInActivity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->