---
title: tipo de recurso credentialUsageSummary
description: Representa o estado atual de quantos usuários da sua organização estão usando recursos de redefinição de senha de autoatendimento.
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 46fc3f90b7a7f286d61a324e7b5f439d467a4978
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35518662"
---
# <a name="credentialusagesummary-resource-type"></a><span data-ttu-id="68081-103">tipo de recurso credentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="68081-103">credentialUsageSummary resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68081-104">Representa o estado atual de quantos usuários da sua organização estão usando recursos de redefinição de senha de autoatendimento.</span><span class="sxs-lookup"><span data-stu-id="68081-104">Represents the current state of how many users in your organization are using self-service password reset capabilities.</span></span>

## <a name="methods"></a><span data-ttu-id="68081-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="68081-105">Methods</span></span>

| <span data-ttu-id="68081-106">Método</span><span class="sxs-lookup"><span data-stu-id="68081-106">Method</span></span>       | <span data-ttu-id="68081-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="68081-107">Return Type</span></span> | <span data-ttu-id="68081-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="68081-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="68081-109">getCredentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="68081-109">getCredentialUsageSummary</span></span>](../api/reportroot-getcredentialusagesummary.md) | <span data-ttu-id="68081-110">credentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="68081-110">credentialUsageSummary</span></span> | <span data-ttu-id="68081-111">Ler propriedades e relações de um objeto credentialUsageSummary.</span><span class="sxs-lookup"><span data-stu-id="68081-111">Read properties and relationships of a credentialUsageSummary object.</span></span> |

## <a name="properties"></a><span data-ttu-id="68081-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="68081-112">Properties</span></span>

| <span data-ttu-id="68081-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="68081-113">Property</span></span>     | <span data-ttu-id="68081-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="68081-114">Type</span></span>        | <span data-ttu-id="68081-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="68081-115">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="68081-116">authMethod</span><span class="sxs-lookup"><span data-stu-id="68081-116">authMethod</span></span> | <span data-ttu-id="68081-117">string</span><span class="sxs-lookup"><span data-stu-id="68081-117">string</span></span> | <span data-ttu-id="68081-118">Representa o método de autenticação usado pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="68081-118">Represents the authentication method that the user used.</span></span> <span data-ttu-id="68081-119">Os valores possíveis são `email`: `mobileSMS`, `mobileCall`, `officePhone`, `securityQuestion` , (usado somente para redefinição de senha de autoatendimento `appCode`), `alternateMobileCall` `appNotification`, e (somente com suporte para registro).</span><span class="sxs-lookup"><span data-stu-id="68081-119">Possible values are: `email`, `mobileSMS`, `mobileCall`, `officePhone`, `securityQuestion` (only used for self-service password reset), `appNotification`, `appCode`, and  `alternateMobileCall` (only supported for registration).</span></span> |
| <span data-ttu-id="68081-120">failureActivityCount</span><span class="sxs-lookup"><span data-stu-id="68081-120">failureActivityCount</span></span> | <span data-ttu-id="68081-121">Int64</span><span class="sxs-lookup"><span data-stu-id="68081-121">Int64</span></span> | <span data-ttu-id="68081-122">Fornece a contagem de redefinições ou dados de registro com falha.</span><span class="sxs-lookup"><span data-stu-id="68081-122">Provides the count of failed resets or registration data.</span></span> |
| <span data-ttu-id="68081-123">apresentam</span><span class="sxs-lookup"><span data-stu-id="68081-123">feature</span></span> | <span data-ttu-id="68081-124">string</span><span class="sxs-lookup"><span data-stu-id="68081-124">string</span></span> | <span data-ttu-id="68081-125">Define o recurso a ser relatado.</span><span class="sxs-lookup"><span data-stu-id="68081-125">Defines the feature to report.</span></span> <span data-ttu-id="68081-126">Os valores possíveis são `registration` : `reset`e.</span><span class="sxs-lookup"><span data-stu-id="68081-126">Possible values are: `registration` and `reset`.</span></span> |
| <span data-ttu-id="68081-127">id</span><span class="sxs-lookup"><span data-stu-id="68081-127">id</span></span> | <span data-ttu-id="68081-128">String</span><span class="sxs-lookup"><span data-stu-id="68081-128">String</span></span> | <span data-ttu-id="68081-129">O identificador exclusivo da atividade.</span><span class="sxs-lookup"><span data-stu-id="68081-129">The unique identifier for the activity.</span></span> <span data-ttu-id="68081-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="68081-130">Read-only.</span></span> |
| <span data-ttu-id="68081-131">successfulActivityCount</span><span class="sxs-lookup"><span data-stu-id="68081-131">successfulActivityCount</span></span> | <span data-ttu-id="68081-132">Int64</span><span class="sxs-lookup"><span data-stu-id="68081-132">Int64</span></span> | <span data-ttu-id="68081-133">Fornece a contagem de registros ou redefinições bem-sucedidas.</span><span class="sxs-lookup"><span data-stu-id="68081-133">Provides the count of successful registrations or resets.</span></span> |

## <a name="relationships"></a><span data-ttu-id="68081-134">Relações</span><span class="sxs-lookup"><span data-stu-id="68081-134">Relationships</span></span>

<span data-ttu-id="68081-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="68081-135">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="68081-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="68081-136">JSON representation</span></span>

<span data-ttu-id="68081-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="68081-137">The following is a JSON representation of the resource.</span></span>

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