---
title: tipo de recurso credentialUsageSummary
description: Representa o estado atual de quantos usuários em sua organização estão usando recursos de redefinição de senha de autoatendados.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 9db31a0d0397f1394a342fb52796a1bec37bae36
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941821"
---
# <a name="credentialusagesummary-resource-type"></a><span data-ttu-id="abf02-103">tipo de recurso credentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="abf02-103">credentialUsageSummary resource type</span></span>

<span data-ttu-id="abf02-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abf02-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="abf02-105">Representa o estado atual de quantos usuários em sua organização estão usando recursos de redefinição de senha de autoatendados.</span><span class="sxs-lookup"><span data-stu-id="abf02-105">Represents the current state of how many users in your organization are using self-service password reset capabilities.</span></span>

## <a name="methods"></a><span data-ttu-id="abf02-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="abf02-106">Methods</span></span>

| <span data-ttu-id="abf02-107">Método</span><span class="sxs-lookup"><span data-stu-id="abf02-107">Method</span></span>       | <span data-ttu-id="abf02-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="abf02-108">Return Type</span></span> | <span data-ttu-id="abf02-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="abf02-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="abf02-110">getCredentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="abf02-110">getCredentialUsageSummary</span></span>](../api/reportroot-getcredentialusagesummary.md) | <span data-ttu-id="abf02-111">credentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="abf02-111">credentialUsageSummary</span></span> | <span data-ttu-id="abf02-112">Ler propriedades e relações de um objeto credentialUsageSummary.</span><span class="sxs-lookup"><span data-stu-id="abf02-112">Read properties and relationships of a credentialUsageSummary object.</span></span> |

## <a name="properties"></a><span data-ttu-id="abf02-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="abf02-113">Properties</span></span>

| <span data-ttu-id="abf02-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="abf02-114">Property</span></span>     | <span data-ttu-id="abf02-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="abf02-115">Type</span></span>        | <span data-ttu-id="abf02-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="abf02-116">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="abf02-117">authMethod</span><span class="sxs-lookup"><span data-stu-id="abf02-117">authMethod</span></span> | <span data-ttu-id="abf02-118">usageAuthMethod</span><span class="sxs-lookup"><span data-stu-id="abf02-118">usageAuthMethod</span></span> | <span data-ttu-id="abf02-119">Representa o método de autenticação que o usuário usou.</span><span class="sxs-lookup"><span data-stu-id="abf02-119">Represents the authentication method that the user used.</span></span> <span data-ttu-id="abf02-120">Os valores possíveis são: , , , , , (usado apenas para redefinição de senha de `email` `mobileSMS` `mobileCall` `officePhone` `securityQuestion` autoatendido), , (suportado somente `appNotification` `appCode` no `alternateMobileCall` registro), , , `fido` `appPassword` `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="abf02-120">Possible values are:`email`, `mobileSMS`, `mobileCall`, `officePhone`, `securityQuestion` (only used for self-service password reset), `appNotification`, `appCode`, `alternateMobileCall` (supported only in registration), `fido`, `appPassword`, `unknownFutureValue`.</span></span> |
| <span data-ttu-id="abf02-121">failureActivityCount</span><span class="sxs-lookup"><span data-stu-id="abf02-121">failureActivityCount</span></span> | <span data-ttu-id="abf02-122">Int64</span><span class="sxs-lookup"><span data-stu-id="abf02-122">Int64</span></span> | <span data-ttu-id="abf02-123">Fornece a contagem de redefinições com falha ou dados de registro.</span><span class="sxs-lookup"><span data-stu-id="abf02-123">Provides the count of failed resets or registration data.</span></span> |
| <span data-ttu-id="abf02-124">feature</span><span class="sxs-lookup"><span data-stu-id="abf02-124">feature</span></span> | <span data-ttu-id="abf02-125">featureType</span><span class="sxs-lookup"><span data-stu-id="abf02-125">featureType</span></span> | <span data-ttu-id="abf02-126">Define o recurso a ser relatório.</span><span class="sxs-lookup"><span data-stu-id="abf02-126">Defines the feature to report.</span></span> <span data-ttu-id="abf02-127">Os valores possíveis são: `registration`, `reset`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="abf02-127">Possible values are: `registration`, `reset`, `unknownFutureValue`.</span></span> |
| <span data-ttu-id="abf02-128">id</span><span class="sxs-lookup"><span data-stu-id="abf02-128">id</span></span> | <span data-ttu-id="abf02-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="abf02-129">String</span></span> | <span data-ttu-id="abf02-130">O identificador exclusivo da atividade.</span><span class="sxs-lookup"><span data-stu-id="abf02-130">The unique identifier for the activity.</span></span> <span data-ttu-id="abf02-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="abf02-131">Read-only.</span></span> |
| <span data-ttu-id="abf02-132">successfulActivityCount</span><span class="sxs-lookup"><span data-stu-id="abf02-132">successfulActivityCount</span></span> | <span data-ttu-id="abf02-133">Int64</span><span class="sxs-lookup"><span data-stu-id="abf02-133">Int64</span></span> | <span data-ttu-id="abf02-134">Fornece a contagem de registros bem-sucedidos ou redefinições.</span><span class="sxs-lookup"><span data-stu-id="abf02-134">Provides the count of successful registrations or resets.</span></span> |

## <a name="relationships"></a><span data-ttu-id="abf02-135">Relações</span><span class="sxs-lookup"><span data-stu-id="abf02-135">Relationships</span></span>

<span data-ttu-id="abf02-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="abf02-136">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="abf02-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="abf02-137">JSON representation</span></span>

<span data-ttu-id="abf02-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="abf02-138">The following is a JSON representation of the resource.</span></span>

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

