---
title: tipo de recurso credentialUsageSummary
description: Representa o estado atual de quantos usuários da sua organização estão usando recursos de redefinição de senha de autoatendimento.
localization_priority: Normal
author: khotz
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 311f89b67549e6bc373029aef82c88ca0e592f3d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050091"
---
# <a name="credentialusagesummary-resource-type"></a><span data-ttu-id="c3088-103">tipo de recurso credentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="c3088-103">credentialUsageSummary resource type</span></span>

<span data-ttu-id="c3088-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3088-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3088-105">Representa o estado atual de quantos usuários da sua organização estão usando recursos de redefinição de senha de autoatendimento.</span><span class="sxs-lookup"><span data-stu-id="c3088-105">Represents the current state of how many users in your organization are using self-service password reset capabilities.</span></span>

## <a name="methods"></a><span data-ttu-id="c3088-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="c3088-106">Methods</span></span>

| <span data-ttu-id="c3088-107">Método</span><span class="sxs-lookup"><span data-stu-id="c3088-107">Method</span></span>       | <span data-ttu-id="c3088-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c3088-108">Return Type</span></span> | <span data-ttu-id="c3088-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3088-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="c3088-110">getCredentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="c3088-110">getCredentialUsageSummary</span></span>](../api/reportroot-getcredentialusagesummary.md) | <span data-ttu-id="c3088-111">credentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="c3088-111">credentialUsageSummary</span></span> | <span data-ttu-id="c3088-112">Ler propriedades e relações de um objeto credentialUsageSummary.</span><span class="sxs-lookup"><span data-stu-id="c3088-112">Read properties and relationships of a credentialUsageSummary object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c3088-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c3088-113">Properties</span></span>

| <span data-ttu-id="c3088-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c3088-114">Property</span></span>     | <span data-ttu-id="c3088-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3088-115">Type</span></span>        | <span data-ttu-id="c3088-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3088-116">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="c3088-117">authMethod</span><span class="sxs-lookup"><span data-stu-id="c3088-117">authMethod</span></span> | <span data-ttu-id="c3088-118">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c3088-118">string</span></span> | <span data-ttu-id="c3088-119">Representa o método de autenticação usado pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="c3088-119">Represents the authentication method that the user used.</span></span> <span data-ttu-id="c3088-120">Os valores possíveis são: `email` , `mobileSMS` ,, `mobileCall` `officePhone` , `securityQuestion` (usado somente para redefinição de senha de autoatendimento),, `appNotification` `appCode` e  `alternateMobileCall` (somente com suporte para registro).</span><span class="sxs-lookup"><span data-stu-id="c3088-120">Possible values are: `email`, `mobileSMS`, `mobileCall`, `officePhone`, `securityQuestion` (only used for self-service password reset), `appNotification`, `appCode`, and  `alternateMobileCall` (only supported for registration).</span></span> |
| <span data-ttu-id="c3088-121">failureActivityCount</span><span class="sxs-lookup"><span data-stu-id="c3088-121">failureActivityCount</span></span> | <span data-ttu-id="c3088-122">Int64</span><span class="sxs-lookup"><span data-stu-id="c3088-122">Int64</span></span> | <span data-ttu-id="c3088-123">Fornece a contagem de redefinições ou dados de registro com falha.</span><span class="sxs-lookup"><span data-stu-id="c3088-123">Provides the count of failed resets or registration data.</span></span> |
| <span data-ttu-id="c3088-124">apresentam</span><span class="sxs-lookup"><span data-stu-id="c3088-124">feature</span></span> | <span data-ttu-id="c3088-125">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c3088-125">string</span></span> | <span data-ttu-id="c3088-126">Define o recurso a ser relatado.</span><span class="sxs-lookup"><span data-stu-id="c3088-126">Defines the feature to report.</span></span> <span data-ttu-id="c3088-127">Os valores possíveis são: `registration` e `reset` .</span><span class="sxs-lookup"><span data-stu-id="c3088-127">Possible values are: `registration` and `reset`.</span></span> |
| <span data-ttu-id="c3088-128">id</span><span class="sxs-lookup"><span data-stu-id="c3088-128">id</span></span> | <span data-ttu-id="c3088-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c3088-129">String</span></span> | <span data-ttu-id="c3088-130">O identificador exclusivo da atividade.</span><span class="sxs-lookup"><span data-stu-id="c3088-130">The unique identifier for the activity.</span></span> <span data-ttu-id="c3088-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c3088-131">Read-only.</span></span> |
| <span data-ttu-id="c3088-132">successfulActivityCount</span><span class="sxs-lookup"><span data-stu-id="c3088-132">successfulActivityCount</span></span> | <span data-ttu-id="c3088-133">Int64</span><span class="sxs-lookup"><span data-stu-id="c3088-133">Int64</span></span> | <span data-ttu-id="c3088-134">Fornece a contagem de registros ou redefinições bem-sucedidas.</span><span class="sxs-lookup"><span data-stu-id="c3088-134">Provides the count of successful registrations or resets.</span></span> |

## <a name="relationships"></a><span data-ttu-id="c3088-135">Relações</span><span class="sxs-lookup"><span data-stu-id="c3088-135">Relationships</span></span>

<span data-ttu-id="c3088-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c3088-136">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3088-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c3088-137">JSON representation</span></span>

<span data-ttu-id="c3088-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c3088-138">The following is a JSON representation of the resource.</span></span>

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

