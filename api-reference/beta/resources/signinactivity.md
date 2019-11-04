---
title: tipo de recurso signInActivity
description: Fornece a última data de logon de um usuário específico.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d93ff4f3b395d9b0820865c3293a419471ab6473
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939240"
---
# <a name="signinactivity-resource-type"></a><span data-ttu-id="d211d-103">tipo de recurso signInActivity</span><span class="sxs-lookup"><span data-stu-id="d211d-103">signInActivity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d211d-104">Fornece a última data de logon de um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="d211d-104">Provides the last signed-in date for a specific user.</span></span>

## <a name="properties"></a><span data-ttu-id="d211d-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d211d-105">Properties</span></span>

| <span data-ttu-id="d211d-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d211d-106">Property</span></span>     | <span data-ttu-id="d211d-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="d211d-107">Type</span></span>        | <span data-ttu-id="d211d-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="d211d-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d211d-109">lastSignInDateTime</span><span class="sxs-lookup"><span data-stu-id="d211d-109">lastSignInDateTime</span></span>|<span data-ttu-id="d211d-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d211d-110">DateTimeOffset</span></span>|<span data-ttu-id="d211d-111">A última data de entrada de um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="d211d-111">The last sign-in date for a specific user.</span></span> <span data-ttu-id="d211d-112">Você pode usar esse campo para calcular a última vez que um usuário entrou no diretório.</span><span class="sxs-lookup"><span data-stu-id="d211d-112">You can use this field to calculate the last time a user signed in to the directory.</span></span> <span data-ttu-id="d211d-113">Este campo pode ser usado para criar relatórios, como usuários inativos.</span><span class="sxs-lookup"><span data-stu-id="d211d-113">This field can be used to build reports, such as inactive users.</span></span> <span data-ttu-id="d211d-114">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="d211d-114">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d211d-115">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="d211d-115">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="d211d-116">lastSignInRequestId</span><span class="sxs-lookup"><span data-stu-id="d211d-116">lastSignInRequestId</span></span>|<span data-ttu-id="d211d-117">String</span><span class="sxs-lookup"><span data-stu-id="d211d-117">String</span></span>|<span data-ttu-id="d211d-118">ID da solicitação da última entrada realizada por esse usuário.</span><span class="sxs-lookup"><span data-stu-id="d211d-118">Request ID of the last sign-in performed by this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d211d-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d211d-119">JSON representation</span></span>

<span data-ttu-id="d211d-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d211d-120">The following is a JSON representation of the resource.</span></span>

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