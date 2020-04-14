---
title: tipo de recurso credentialUserRegistrationCount
description: Representa o estado atual de quantos usuários da sua organização estão registrados para recursos de redefinição de senha de autoatendimento e autenticação multifator.
localization_priority: Normal
author: khotz
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: b291d871686b514474f754500d490be3ad331441
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43458008"
---
# <a name="credentialuserregistrationcount-resource-type"></a><span data-ttu-id="e1ab9-103">tipo de recurso credentialUserRegistrationCount</span><span class="sxs-lookup"><span data-stu-id="e1ab9-103">credentialUserRegistrationCount resource type</span></span>

<span data-ttu-id="e1ab9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1ab9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1ab9-105">Representa o estado atual de quantos usuários da sua organização estão registrados para recursos de redefinição de senha de autoatendimento e autenticação multifator.</span><span class="sxs-lookup"><span data-stu-id="e1ab9-105">Represents the current state of how many users in your organization are registered for self-service password reset and multi-factor authentication capabilities.</span></span>

## <a name="methods"></a><span data-ttu-id="e1ab9-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="e1ab9-106">Methods</span></span>

| <span data-ttu-id="e1ab9-107">Método</span><span class="sxs-lookup"><span data-stu-id="e1ab9-107">Method</span></span>       | <span data-ttu-id="e1ab9-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e1ab9-108">Return Type</span></span> | <span data-ttu-id="e1ab9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1ab9-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e1ab9-110">getCredentialUserRegistrationCount</span><span class="sxs-lookup"><span data-stu-id="e1ab9-110">getCredentialUserRegistrationCount</span></span>](../api/reportroot-getcredentialuserregistrationcount.md) | <span data-ttu-id="e1ab9-111">coleção credentialUserRegistrationCount</span><span class="sxs-lookup"><span data-stu-id="e1ab9-111">credentialUserRegistrationCount collection</span></span> | <span data-ttu-id="e1ab9-112">Informe o estado atual de quantos usuários da sua organização estão registrados para recursos de redefinição de senha de autoatendimento e de autenticação multifator (MFA).</span><span class="sxs-lookup"><span data-stu-id="e1ab9-112">Report the current state of how many users in your organization are registered for self-service password reset and multi-factor authentication (MFA) capabilities.</span></span> |

## <a name="properties"></a><span data-ttu-id="e1ab9-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e1ab9-113">Properties</span></span>

| <span data-ttu-id="e1ab9-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e1ab9-114">Property</span></span>     | <span data-ttu-id="e1ab9-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1ab9-115">Type</span></span>        | <span data-ttu-id="e1ab9-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1ab9-116">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="e1ab9-117">id</span><span class="sxs-lookup"><span data-stu-id="e1ab9-117">id</span></span> | <span data-ttu-id="e1ab9-118">String</span><span class="sxs-lookup"><span data-stu-id="e1ab9-118">String</span></span> | <span data-ttu-id="e1ab9-119">O identificador exclusivo da atividade.</span><span class="sxs-lookup"><span data-stu-id="e1ab9-119">The unique identifier for the activity.</span></span> <span data-ttu-id="e1ab9-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e1ab9-120">Read-only.</span></span> |
| <span data-ttu-id="e1ab9-121">totalUserCount</span><span class="sxs-lookup"><span data-stu-id="e1ab9-121">totalUserCount</span></span> | <span data-ttu-id="e1ab9-122">Int64</span><span class="sxs-lookup"><span data-stu-id="e1ab9-122">Int64</span></span> | <span data-ttu-id="e1ab9-123">Fornece a contagem total de usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="e1ab9-123">Provides the total user count in the tenant.</span></span> |
| <span data-ttu-id="e1ab9-124">userRegistrationCounts</span><span class="sxs-lookup"><span data-stu-id="e1ab9-124">userRegistrationCounts</span></span> | <span data-ttu-id="e1ab9-125">coleção [userRegistrationCount](userregistrationcount.md)</span><span class="sxs-lookup"><span data-stu-id="e1ab9-125">[userRegistrationCount](userregistrationcount.md) collection</span></span> | <span data-ttu-id="e1ab9-126">Uma coleção de informações de status e contagem de registro para usuários em seu locatário.</span><span class="sxs-lookup"><span data-stu-id="e1ab9-126">A collection of registration count and status information for users in your tenant.</span></span> |

## <a name="relationships"></a><span data-ttu-id="e1ab9-127">Relações</span><span class="sxs-lookup"><span data-stu-id="e1ab9-127">Relationships</span></span>

<span data-ttu-id="e1ab9-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e1ab9-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e1ab9-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e1ab9-129">JSON representation</span></span>

<span data-ttu-id="e1ab9-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e1ab9-130">The following is a JSON representation of the resource.</span></span>

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