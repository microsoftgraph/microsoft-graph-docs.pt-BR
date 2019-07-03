---
title: tipo de recurso credentialUserRegistrationCount
description: Representa o estado atual de quantos usuários da sua organização estão registrados para recursos de redefinição de senha de autoatendimento e autenticação multifator.
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 42c722b04493767d3dbcaf713157d931569d8c32
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35475897"
---
# <a name="credentialuserregistrationcount-resource-type"></a><span data-ttu-id="e547f-103">tipo de recurso credentialUserRegistrationCount</span><span class="sxs-lookup"><span data-stu-id="e547f-103">credentialUserRegistrationCount resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e547f-104">Representa o estado atual de quantos usuários da sua organização estão registrados para recursos de redefinição de senha de autoatendimento e autenticação multifator.</span><span class="sxs-lookup"><span data-stu-id="e547f-104">Represents the current state of how many users in your organization are registered for self-service password reset and multi-factor authentication capabilities.</span></span>

## <a name="methods"></a><span data-ttu-id="e547f-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="e547f-105">Methods</span></span>

| <span data-ttu-id="e547f-106">Método</span><span class="sxs-lookup"><span data-stu-id="e547f-106">Method</span></span>       | <span data-ttu-id="e547f-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e547f-107">Return Type</span></span> | <span data-ttu-id="e547f-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="e547f-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e547f-109">getCredentialUserRegistrationCount</span><span class="sxs-lookup"><span data-stu-id="e547f-109">getCredentialUserRegistrationCount</span></span>](../api/reportroot-getcredentialuserregistrationcount.md) | <span data-ttu-id="e547f-110">coleção credentialUserRegistrationCount</span><span class="sxs-lookup"><span data-stu-id="e547f-110">credentialUserRegistrationCount collection</span></span> | <span data-ttu-id="e547f-111">Informe o estado atual de quantos usuários da sua organização estão registrados para recursos de redefinição de senha de autoatendimento e de autenticação multifator (MFA).</span><span class="sxs-lookup"><span data-stu-id="e547f-111">Report the current state of how many users in your organization are registered for self-service password reset and multi-factor authentication (MFA) capabilities.</span></span> |

## <a name="properties"></a><span data-ttu-id="e547f-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e547f-112">Properties</span></span>

| <span data-ttu-id="e547f-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e547f-113">Property</span></span>     | <span data-ttu-id="e547f-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="e547f-114">Type</span></span>        | <span data-ttu-id="e547f-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="e547f-115">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="e547f-116">id</span><span class="sxs-lookup"><span data-stu-id="e547f-116">id</span></span> | <span data-ttu-id="e547f-117">String</span><span class="sxs-lookup"><span data-stu-id="e547f-117">String</span></span> | <span data-ttu-id="e547f-118">O identificador exclusivo da atividade.</span><span class="sxs-lookup"><span data-stu-id="e547f-118">The unique identifier for the activity.</span></span> <span data-ttu-id="e547f-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e547f-119">Read-only.</span></span> |
| <span data-ttu-id="e547f-120">totalUserCount</span><span class="sxs-lookup"><span data-stu-id="e547f-120">totalUserCount</span></span> | <span data-ttu-id="e547f-121">Int64</span><span class="sxs-lookup"><span data-stu-id="e547f-121">Int64</span></span> | <span data-ttu-id="e547f-122">Fornece a contagem total de usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="e547f-122">Provides the total user count in the tenant.</span></span> |
| <span data-ttu-id="e547f-123">userRegistrationCounts</span><span class="sxs-lookup"><span data-stu-id="e547f-123">userRegistrationCounts</span></span> | <span data-ttu-id="e547f-124">coleção [userRegistrationCount](userregistrationcount.md)</span><span class="sxs-lookup"><span data-stu-id="e547f-124">[userRegistrationCount](userregistrationcount.md) collection</span></span> | <span data-ttu-id="e547f-125">Uma coleção de informações de status e contagem de registro para usuários em seu locatário.</span><span class="sxs-lookup"><span data-stu-id="e547f-125">A collection of registration count and status information for users in your tenant.</span></span> |

## <a name="relationships"></a><span data-ttu-id="e547f-126">Relações</span><span class="sxs-lookup"><span data-stu-id="e547f-126">Relationships</span></span>

<span data-ttu-id="e547f-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e547f-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e547f-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e547f-128">JSON representation</span></span>

<span data-ttu-id="e547f-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e547f-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.credentialUserRegistrationCount",
  "baseType": "",
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