---
title: Tipo de recurso credentialUserRegistrationCount
description: Representa o estado atual de quantos usuários em sua organização estão registrados para redefinição de senha de autoatendado e recursos de autenticação multifa factor.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 521c8eca7c3233000bf04f2324e8990fd25c55f6
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159917"
---
# <a name="credentialuserregistrationcount-resource-type"></a><span data-ttu-id="ddb80-103">Tipo de recurso credentialUserRegistrationCount</span><span class="sxs-lookup"><span data-stu-id="ddb80-103">credentialUserRegistrationCount resource type</span></span>

<span data-ttu-id="ddb80-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ddb80-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ddb80-105">Representa o estado atual de quantos usuários em sua organização estão registrados para redefinição de senha de autoatendado e recursos de autenticação multifa factor.</span><span class="sxs-lookup"><span data-stu-id="ddb80-105">Represents the current state of how many users in your organization are registered for self-service password reset and multi-factor authentication capabilities.</span></span>

## <a name="methods"></a><span data-ttu-id="ddb80-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="ddb80-106">Methods</span></span>

| <span data-ttu-id="ddb80-107">Método</span><span class="sxs-lookup"><span data-stu-id="ddb80-107">Method</span></span>       | <span data-ttu-id="ddb80-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ddb80-108">Return Type</span></span> | <span data-ttu-id="ddb80-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddb80-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="ddb80-110">getCredentialUserRegistrationCount</span><span class="sxs-lookup"><span data-stu-id="ddb80-110">getCredentialUserRegistrationCount</span></span>](../api/reportroot-getcredentialuserregistrationcount.md) | <span data-ttu-id="ddb80-111">Coleção credentialUserRegistrationCount</span><span class="sxs-lookup"><span data-stu-id="ddb80-111">credentialUserRegistrationCount collection</span></span> | <span data-ttu-id="ddb80-112">Relatar o estado atual de quantos usuários em sua organização estão registrados para redefinição de senha de autoatendado e recursos de autenticação multifatória (MFA).</span><span class="sxs-lookup"><span data-stu-id="ddb80-112">Report the current state of how many users in your organization are registered for self-service password reset and multi-factor authentication (MFA) capabilities.</span></span> |

## <a name="properties"></a><span data-ttu-id="ddb80-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ddb80-113">Properties</span></span>

| <span data-ttu-id="ddb80-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ddb80-114">Property</span></span>     | <span data-ttu-id="ddb80-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="ddb80-115">Type</span></span>        | <span data-ttu-id="ddb80-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddb80-116">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="ddb80-117">id</span><span class="sxs-lookup"><span data-stu-id="ddb80-117">id</span></span> | <span data-ttu-id="ddb80-118">String</span><span class="sxs-lookup"><span data-stu-id="ddb80-118">String</span></span> | <span data-ttu-id="ddb80-119">O identificador exclusivo da atividade.</span><span class="sxs-lookup"><span data-stu-id="ddb80-119">The unique identifier for the activity.</span></span> <span data-ttu-id="ddb80-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ddb80-120">Read-only.</span></span> |
| <span data-ttu-id="ddb80-121">totalUserCount</span><span class="sxs-lookup"><span data-stu-id="ddb80-121">totalUserCount</span></span> | <span data-ttu-id="ddb80-122">Int64</span><span class="sxs-lookup"><span data-stu-id="ddb80-122">Int64</span></span> | <span data-ttu-id="ddb80-123">Fornece a contagem total de usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="ddb80-123">Provides the total user count in the tenant.</span></span> |
| <span data-ttu-id="ddb80-124">userRegistrationCounts</span><span class="sxs-lookup"><span data-stu-id="ddb80-124">userRegistrationCounts</span></span> | <span data-ttu-id="ddb80-125">[Coleção userRegistrationCount](userregistrationcount.md)</span><span class="sxs-lookup"><span data-stu-id="ddb80-125">[userRegistrationCount](userregistrationcount.md) collection</span></span> | <span data-ttu-id="ddb80-126">Uma coleção de informações de status e contagem de registro para usuários em seu locatário.</span><span class="sxs-lookup"><span data-stu-id="ddb80-126">A collection of registration count and status information for users in your tenant.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ddb80-127">Relações</span><span class="sxs-lookup"><span data-stu-id="ddb80-127">Relationships</span></span>

<span data-ttu-id="ddb80-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ddb80-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ddb80-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ddb80-129">JSON representation</span></span>

<span data-ttu-id="ddb80-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ddb80-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.credentialUserRegistrationCount",
  "keyProperty": "id"
}-->

```json
{
  "id" : "String",
  "totalUserCount" : 23123,
  "userRegistrationCounts" :
  [
    { "registrationStatus":"registered", "registrationCount": 23423 },
    { "registrationStatus":"enabled", "registrationCount": 4234 },
    { "registrationStatus":"capable", "registrationCount": 323 },
    { "registrationStatus":"mfaRegistered", "registrationCount": 33 }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "credentialUserRegistrationCount resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

