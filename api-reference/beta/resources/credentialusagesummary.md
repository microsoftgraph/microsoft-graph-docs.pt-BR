---
title: Tipo de recurso credentialUsageSummary
description: Representa o estado atual de quantos usuários em sua organização estão usando recursos de redefinição de senha de autoatendado.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 03ae7b4b03cf58301895e5246fa4cb86d1b79667
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157698"
---
# <a name="credentialusagesummary-resource-type"></a><span data-ttu-id="ed289-103">Tipo de recurso credentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="ed289-103">credentialUsageSummary resource type</span></span>

<span data-ttu-id="ed289-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed289-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed289-105">Representa o estado atual de quantos usuários em sua organização estão usando recursos de redefinição de senha de autoatendado.</span><span class="sxs-lookup"><span data-stu-id="ed289-105">Represents the current state of how many users in your organization are using self-service password reset capabilities.</span></span>

## <a name="methods"></a><span data-ttu-id="ed289-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="ed289-106">Methods</span></span>

| <span data-ttu-id="ed289-107">Método</span><span class="sxs-lookup"><span data-stu-id="ed289-107">Method</span></span>       | <span data-ttu-id="ed289-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ed289-108">Return Type</span></span> | <span data-ttu-id="ed289-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed289-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="ed289-110">getCredentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="ed289-110">getCredentialUsageSummary</span></span>](../api/reportroot-getcredentialusagesummary.md) | <span data-ttu-id="ed289-111">credentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="ed289-111">credentialUsageSummary</span></span> | <span data-ttu-id="ed289-112">Ler propriedades e relações de um objeto credentialUsageSummary.</span><span class="sxs-lookup"><span data-stu-id="ed289-112">Read properties and relationships of a credentialUsageSummary object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ed289-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ed289-113">Properties</span></span>

| <span data-ttu-id="ed289-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ed289-114">Property</span></span>     | <span data-ttu-id="ed289-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed289-115">Type</span></span>        | <span data-ttu-id="ed289-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed289-116">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="ed289-117">authMethod</span><span class="sxs-lookup"><span data-stu-id="ed289-117">authMethod</span></span> | <span data-ttu-id="ed289-118">string</span><span class="sxs-lookup"><span data-stu-id="ed289-118">string</span></span> | <span data-ttu-id="ed289-119">Representa o método de autenticação que o usuário usou.</span><span class="sxs-lookup"><span data-stu-id="ed289-119">Represents the authentication method that the user used.</span></span> <span data-ttu-id="ed289-120">Os valores possíveis são: , , , (usado somente para redefinição de senha de `email` `mobileSMS` `mobileCall` `officePhone` `securityQuestion` autoatendido) `appNotification` `appCode` e  `alternateMobileCall` (somente com suporte para registro).</span><span class="sxs-lookup"><span data-stu-id="ed289-120">Possible values are: `email`, `mobileSMS`, `mobileCall`, `officePhone`, `securityQuestion` (only used for self-service password reset), `appNotification`, `appCode`, and  `alternateMobileCall` (only supported for registration).</span></span> |
| <span data-ttu-id="ed289-121">failureActivityCount</span><span class="sxs-lookup"><span data-stu-id="ed289-121">failureActivityCount</span></span> | <span data-ttu-id="ed289-122">Int64</span><span class="sxs-lookup"><span data-stu-id="ed289-122">Int64</span></span> | <span data-ttu-id="ed289-123">Fornece a contagem de redefinições com falha ou dados de registro.</span><span class="sxs-lookup"><span data-stu-id="ed289-123">Provides the count of failed resets or registration data.</span></span> |
| <span data-ttu-id="ed289-124">recurso</span><span class="sxs-lookup"><span data-stu-id="ed289-124">feature</span></span> | <span data-ttu-id="ed289-125">string</span><span class="sxs-lookup"><span data-stu-id="ed289-125">string</span></span> | <span data-ttu-id="ed289-126">Define o recurso a ser reportdo.</span><span class="sxs-lookup"><span data-stu-id="ed289-126">Defines the feature to report.</span></span> <span data-ttu-id="ed289-127">Os valores possíveis são: `registration` e `reset` .</span><span class="sxs-lookup"><span data-stu-id="ed289-127">Possible values are: `registration` and `reset`.</span></span> |
| <span data-ttu-id="ed289-128">id</span><span class="sxs-lookup"><span data-stu-id="ed289-128">id</span></span> | <span data-ttu-id="ed289-129">String</span><span class="sxs-lookup"><span data-stu-id="ed289-129">String</span></span> | <span data-ttu-id="ed289-130">O identificador exclusivo da atividade.</span><span class="sxs-lookup"><span data-stu-id="ed289-130">The unique identifier for the activity.</span></span> <span data-ttu-id="ed289-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ed289-131">Read-only.</span></span> |
| <span data-ttu-id="ed289-132">successfulActivityCount</span><span class="sxs-lookup"><span data-stu-id="ed289-132">successfulActivityCount</span></span> | <span data-ttu-id="ed289-133">Int64</span><span class="sxs-lookup"><span data-stu-id="ed289-133">Int64</span></span> | <span data-ttu-id="ed289-134">Fornece a contagem de registros ou redefinições bem-sucedidos.</span><span class="sxs-lookup"><span data-stu-id="ed289-134">Provides the count of successful registrations or resets.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ed289-135">Relações</span><span class="sxs-lookup"><span data-stu-id="ed289-135">Relationships</span></span>

<span data-ttu-id="ed289-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ed289-136">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ed289-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ed289-137">JSON representation</span></span>

<span data-ttu-id="ed289-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ed289-138">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.credentialUsageSummary",
  "keyProperty": "id"
}-->

```json
{
  "id" : "String",
  "feature":"string",
  "successfulActivityCount":"Int64",
  "failureActivityCount": "Int64",
  "authMethod": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "credentialUsageSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

