---
title: tipo de recurso credentialUsageSummary
description: Representa o estado atual de quantos usuários da sua organização estão usando recursos de redefinição de senha de autoatendimento.
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 17fc4535e5132b6bf6c2f6eab4a94b5a58ef9bb1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507349"
---
# <a name="credentialusagesummary-resource-type"></a><span data-ttu-id="5e4c1-103">tipo de recurso credentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="5e4c1-103">credentialUsageSummary resource type</span></span>

<span data-ttu-id="5e4c1-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5e4c1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e4c1-105">Representa o estado atual de quantos usuários da sua organização estão usando recursos de redefinição de senha de autoatendimento.</span><span class="sxs-lookup"><span data-stu-id="5e4c1-105">Represents the current state of how many users in your organization are using self-service password reset capabilities.</span></span>

## <a name="methods"></a><span data-ttu-id="5e4c1-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="5e4c1-106">Methods</span></span>

| <span data-ttu-id="5e4c1-107">Método</span><span class="sxs-lookup"><span data-stu-id="5e4c1-107">Method</span></span>       | <span data-ttu-id="5e4c1-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5e4c1-108">Return Type</span></span> | <span data-ttu-id="5e4c1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e4c1-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="5e4c1-110">getCredentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="5e4c1-110">getCredentialUsageSummary</span></span>](../api/reportroot-getcredentialusagesummary.md) | <span data-ttu-id="5e4c1-111">credentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="5e4c1-111">credentialUsageSummary</span></span> | <span data-ttu-id="5e4c1-112">Ler propriedades e relações de um objeto credentialUsageSummary.</span><span class="sxs-lookup"><span data-stu-id="5e4c1-112">Read properties and relationships of a credentialUsageSummary object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5e4c1-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5e4c1-113">Properties</span></span>

| <span data-ttu-id="5e4c1-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5e4c1-114">Property</span></span>     | <span data-ttu-id="5e4c1-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e4c1-115">Type</span></span>        | <span data-ttu-id="5e4c1-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e4c1-116">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="5e4c1-117">authMethod</span><span class="sxs-lookup"><span data-stu-id="5e4c1-117">authMethod</span></span> | <span data-ttu-id="5e4c1-118">string</span><span class="sxs-lookup"><span data-stu-id="5e4c1-118">string</span></span> | <span data-ttu-id="5e4c1-119">Representa o método de autenticação usado pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="5e4c1-119">Represents the authentication method that the user used.</span></span> <span data-ttu-id="5e4c1-120">Os valores possíveis são `email`: `mobileSMS`, `mobileCall`, `officePhone`, `securityQuestion` , (usado somente para redefinição de senha de autoatendimento `appCode`), `alternateMobileCall` `appNotification`, e (somente com suporte para registro).</span><span class="sxs-lookup"><span data-stu-id="5e4c1-120">Possible values are: `email`, `mobileSMS`, `mobileCall`, `officePhone`, `securityQuestion` (only used for self-service password reset), `appNotification`, `appCode`, and  `alternateMobileCall` (only supported for registration).</span></span> |
| <span data-ttu-id="5e4c1-121">failureActivityCount</span><span class="sxs-lookup"><span data-stu-id="5e4c1-121">failureActivityCount</span></span> | <span data-ttu-id="5e4c1-122">Int64</span><span class="sxs-lookup"><span data-stu-id="5e4c1-122">Int64</span></span> | <span data-ttu-id="5e4c1-123">Fornece a contagem de redefinições ou dados de registro com falha.</span><span class="sxs-lookup"><span data-stu-id="5e4c1-123">Provides the count of failed resets or registration data.</span></span> |
| <span data-ttu-id="5e4c1-124">apresentam</span><span class="sxs-lookup"><span data-stu-id="5e4c1-124">feature</span></span> | <span data-ttu-id="5e4c1-125">string</span><span class="sxs-lookup"><span data-stu-id="5e4c1-125">string</span></span> | <span data-ttu-id="5e4c1-126">Define o recurso a ser relatado.</span><span class="sxs-lookup"><span data-stu-id="5e4c1-126">Defines the feature to report.</span></span> <span data-ttu-id="5e4c1-127">Os valores possíveis são `registration` : `reset`e.</span><span class="sxs-lookup"><span data-stu-id="5e4c1-127">Possible values are: `registration` and `reset`.</span></span> |
| <span data-ttu-id="5e4c1-128">id</span><span class="sxs-lookup"><span data-stu-id="5e4c1-128">id</span></span> | <span data-ttu-id="5e4c1-129">String</span><span class="sxs-lookup"><span data-stu-id="5e4c1-129">String</span></span> | <span data-ttu-id="5e4c1-130">O identificador exclusivo da atividade.</span><span class="sxs-lookup"><span data-stu-id="5e4c1-130">The unique identifier for the activity.</span></span> <span data-ttu-id="5e4c1-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5e4c1-131">Read-only.</span></span> |
| <span data-ttu-id="5e4c1-132">successfulActivityCount</span><span class="sxs-lookup"><span data-stu-id="5e4c1-132">successfulActivityCount</span></span> | <span data-ttu-id="5e4c1-133">Int64</span><span class="sxs-lookup"><span data-stu-id="5e4c1-133">Int64</span></span> | <span data-ttu-id="5e4c1-134">Fornece a contagem de registros ou redefinições bem-sucedidas.</span><span class="sxs-lookup"><span data-stu-id="5e4c1-134">Provides the count of successful registrations or resets.</span></span> |

## <a name="relationships"></a><span data-ttu-id="5e4c1-135">Relações</span><span class="sxs-lookup"><span data-stu-id="5e4c1-135">Relationships</span></span>

<span data-ttu-id="5e4c1-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5e4c1-136">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5e4c1-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5e4c1-137">JSON representation</span></span>

<span data-ttu-id="5e4c1-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5e4c1-138">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.credentialUsageSummary",
  "baseType": "",
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