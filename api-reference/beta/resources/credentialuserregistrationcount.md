---
title: tipo de recurso credentialUserRegistrationCount
description: Representa o estado atual de quantos usuários da sua organização estão registrados para recursos de redefinição de senha de autoatendimento e autenticação multifator.
localization_priority: Normal
author: khotz
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: c5fb3588c7d06f726c71c81279c0994fd0de4019
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050084"
---
# <a name="credentialuserregistrationcount-resource-type"></a><span data-ttu-id="16476-103">tipo de recurso credentialUserRegistrationCount</span><span class="sxs-lookup"><span data-stu-id="16476-103">credentialUserRegistrationCount resource type</span></span>

<span data-ttu-id="16476-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16476-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16476-105">Representa o estado atual de quantos usuários da sua organização estão registrados para recursos de redefinição de senha de autoatendimento e autenticação multifator.</span><span class="sxs-lookup"><span data-stu-id="16476-105">Represents the current state of how many users in your organization are registered for self-service password reset and multi-factor authentication capabilities.</span></span>

## <a name="methods"></a><span data-ttu-id="16476-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="16476-106">Methods</span></span>

| <span data-ttu-id="16476-107">Método</span><span class="sxs-lookup"><span data-stu-id="16476-107">Method</span></span>       | <span data-ttu-id="16476-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="16476-108">Return Type</span></span> | <span data-ttu-id="16476-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="16476-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="16476-110">getCredentialUserRegistrationCount</span><span class="sxs-lookup"><span data-stu-id="16476-110">getCredentialUserRegistrationCount</span></span>](../api/reportroot-getcredentialuserregistrationcount.md) | <span data-ttu-id="16476-111">coleção credentialUserRegistrationCount</span><span class="sxs-lookup"><span data-stu-id="16476-111">credentialUserRegistrationCount collection</span></span> | <span data-ttu-id="16476-112">Informe o estado atual de quantos usuários da sua organização estão registrados para recursos de redefinição de senha de autoatendimento e de autenticação multifator (MFA).</span><span class="sxs-lookup"><span data-stu-id="16476-112">Report the current state of how many users in your organization are registered for self-service password reset and multi-factor authentication (MFA) capabilities.</span></span> |

## <a name="properties"></a><span data-ttu-id="16476-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="16476-113">Properties</span></span>

| <span data-ttu-id="16476-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="16476-114">Property</span></span>     | <span data-ttu-id="16476-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="16476-115">Type</span></span>        | <span data-ttu-id="16476-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="16476-116">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="16476-117">id</span><span class="sxs-lookup"><span data-stu-id="16476-117">id</span></span> | <span data-ttu-id="16476-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16476-118">String</span></span> | <span data-ttu-id="16476-119">O identificador exclusivo da atividade.</span><span class="sxs-lookup"><span data-stu-id="16476-119">The unique identifier for the activity.</span></span> <span data-ttu-id="16476-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="16476-120">Read-only.</span></span> |
| <span data-ttu-id="16476-121">totalUserCount</span><span class="sxs-lookup"><span data-stu-id="16476-121">totalUserCount</span></span> | <span data-ttu-id="16476-122">Int64</span><span class="sxs-lookup"><span data-stu-id="16476-122">Int64</span></span> | <span data-ttu-id="16476-123">Fornece a contagem total de usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="16476-123">Provides the total user count in the tenant.</span></span> |
| <span data-ttu-id="16476-124">userRegistrationCounts</span><span class="sxs-lookup"><span data-stu-id="16476-124">userRegistrationCounts</span></span> | <span data-ttu-id="16476-125">coleção [userRegistrationCount](userregistrationcount.md)</span><span class="sxs-lookup"><span data-stu-id="16476-125">[userRegistrationCount](userregistrationcount.md) collection</span></span> | <span data-ttu-id="16476-126">Uma coleção de informações de status e contagem de registro para usuários em seu locatário.</span><span class="sxs-lookup"><span data-stu-id="16476-126">A collection of registration count and status information for users in your tenant.</span></span> |

## <a name="relationships"></a><span data-ttu-id="16476-127">Relações</span><span class="sxs-lookup"><span data-stu-id="16476-127">Relationships</span></span>

<span data-ttu-id="16476-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="16476-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="16476-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="16476-129">JSON representation</span></span>

<span data-ttu-id="16476-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="16476-130">The following is a JSON representation of the resource.</span></span>

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

