---
title: Tipo de recurso credentialUserRegistrationDetails
description: Representa os detalhes do uso da redefinição de senha de autoatendado e da autenticação multifatória (MFA) para todos os usuários registrados.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: c7e45b186e1ef7a3a96115f408cb5a0992e538fe
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159903"
---
# <a name="credentialuserregistrationdetails-resource-type"></a><span data-ttu-id="faa88-103">Tipo de recurso credentialUserRegistrationDetails</span><span class="sxs-lookup"><span data-stu-id="faa88-103">credentialUserRegistrationDetails resource type</span></span>

<span data-ttu-id="faa88-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="faa88-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="faa88-105">Representa os detalhes do uso da redefinição de senha de autoatendado e da autenticação multifatória (MFA) para todos os usuários registrados.</span><span class="sxs-lookup"><span data-stu-id="faa88-105">Represents the details of the usage of self-service password reset and multi-factor authentication (MFA) for all registered users.</span></span> <span data-ttu-id="faa88-106">Os detalhes incluem informações do usuário, status do registro e o método de autenticação usado.</span><span class="sxs-lookup"><span data-stu-id="faa88-106">Details include user information, status of registration, and the authentication method used.</span></span>

## <a name="methods"></a><span data-ttu-id="faa88-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="faa88-107">Methods</span></span>

| <span data-ttu-id="faa88-108">Método</span><span class="sxs-lookup"><span data-stu-id="faa88-108">Method</span></span>       | <span data-ttu-id="faa88-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="faa88-109">Return Type</span></span> | <span data-ttu-id="faa88-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="faa88-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="faa88-111">Listar credentialUserRegistrationDetails</span><span class="sxs-lookup"><span data-stu-id="faa88-111">List credentialUserRegistrationDetails</span></span>](../api/reportroot-list-credentialuserregistrationdetails.md) | <span data-ttu-id="faa88-112">Coleção credentialUserRegistrationDetails</span><span class="sxs-lookup"><span data-stu-id="faa88-112">credentialUserRegistrationDetails collection</span></span> | <span data-ttu-id="faa88-113">Obter uma lista de [objetos credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) para um determinado locatário.</span><span class="sxs-lookup"><span data-stu-id="faa88-113">Get a list of [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) objects for a given tenant.</span></span>
 |

## <a name="properties"></a><span data-ttu-id="faa88-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="faa88-114">Properties</span></span>

| <span data-ttu-id="faa88-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="faa88-115">Property</span></span>     | <span data-ttu-id="faa88-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="faa88-116">Type</span></span>        | <span data-ttu-id="faa88-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="faa88-117">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="faa88-118">authMethods</span><span class="sxs-lookup"><span data-stu-id="faa88-118">authMethods</span></span> | <span data-ttu-id="faa88-119">Coleção registrationAuthMethod</span><span class="sxs-lookup"><span data-stu-id="faa88-119">registrationAuthMethod collection</span></span> | <span data-ttu-id="faa88-120">Representa o método de autenticação que o usuário registrou.</span><span class="sxs-lookup"><span data-stu-id="faa88-120">Represents the authentication method that the user has registered.</span></span> <span data-ttu-id="faa88-121">Os valores possíveis são: , , (usado somente para redefinição de senha de `email` `mobilePhone` `officePhone` `securityQuestion` autoatendido) e (com suporte `appNotification` apenas no `appCode` `alternateMobilePhone` registro).</span><span class="sxs-lookup"><span data-stu-id="faa88-121">Possible values are: `email`, `mobilePhone`, `officePhone`, `securityQuestion` (only used for self-service password reset), `appNotification`, `appCode`, and `alternateMobilePhone` (supported only in registration).</span></span> |
| <span data-ttu-id="faa88-122">id</span><span class="sxs-lookup"><span data-stu-id="faa88-122">id</span></span> | <span data-ttu-id="faa88-123">String</span><span class="sxs-lookup"><span data-stu-id="faa88-123">String</span></span> | <span data-ttu-id="faa88-124">O identificador exclusivo da atividade.</span><span class="sxs-lookup"><span data-stu-id="faa88-124">The unique identifier for the activity.</span></span> <span data-ttu-id="faa88-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="faa88-125">Read-only.</span></span>|
| <span data-ttu-id="faa88-126">isCapable</span><span class="sxs-lookup"><span data-stu-id="faa88-126">isCapable</span></span> | <span data-ttu-id="faa88-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="faa88-127">Boolean</span></span> | <span data-ttu-id="faa88-128">Indica se o usuário está pronto para executar a redefinição de senha de autoatendado ou a MFA.</span><span class="sxs-lookup"><span data-stu-id="faa88-128">Indicates whether the user is ready to perform self-service password reset or MFA.</span></span> |
| <span data-ttu-id="faa88-129">isEnabled</span><span class="sxs-lookup"><span data-stu-id="faa88-129">isEnabled</span></span> | <span data-ttu-id="faa88-130">Booliano</span><span class="sxs-lookup"><span data-stu-id="faa88-130">Boolean</span></span> | <span data-ttu-id="faa88-131">Indicia se o usuário está habilitado para executar a redefinição de senha de autoatendência.</span><span class="sxs-lookup"><span data-stu-id="faa88-131">Indiciates whether the user enabled to perform self-service password reset.</span></span> |
| <span data-ttu-id="faa88-132">isMfaRegistered</span><span class="sxs-lookup"><span data-stu-id="faa88-132">isMfaRegistered</span></span> | <span data-ttu-id="faa88-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="faa88-133">Boolean</span></span> | <span data-ttu-id="faa88-134">Indicia se o usuário está registrado para MFA.</span><span class="sxs-lookup"><span data-stu-id="faa88-134">Indiciates whether the user is registered for MFA.</span></span> |
| <span data-ttu-id="faa88-135">isRegistered</span><span class="sxs-lookup"><span data-stu-id="faa88-135">isRegistered</span></span> | <span data-ttu-id="faa88-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="faa88-136">Boolean</span></span> | <span data-ttu-id="faa88-137">Indica se o usuário registrou quaisquer métodos de autenticação para redefinição de senha de autoatendado.</span><span class="sxs-lookup"><span data-stu-id="faa88-137">Indicates whether the user has registered any authentication methods for self-service password reset.</span></span> |
| <span data-ttu-id="faa88-138">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="faa88-138">userDisplayName</span></span> | <span data-ttu-id="faa88-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="faa88-139">String</span></span> | <span data-ttu-id="faa88-140">Fornece o nome de usuário do usuário correspondente.</span><span class="sxs-lookup"><span data-stu-id="faa88-140">Provides the user name of the corresponding user.</span></span> |
| <span data-ttu-id="faa88-141">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="faa88-141">userPrincipalName</span></span> | <span data-ttu-id="faa88-142">String</span><span class="sxs-lookup"><span data-stu-id="faa88-142">String</span></span> | <span data-ttu-id="faa88-143">Fornece o nome principal do usuário do usuário correspondente.</span><span class="sxs-lookup"><span data-stu-id="faa88-143">Provides the user principal name of the corresponding user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="faa88-144">Relações</span><span class="sxs-lookup"><span data-stu-id="faa88-144">Relationships</span></span>

<span data-ttu-id="faa88-145">Nenhum</span><span class="sxs-lookup"><span data-stu-id="faa88-145">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="faa88-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="faa88-146">JSON representation</span></span>

<span data-ttu-id="faa88-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="faa88-147">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.credentialUserRegistrationDetails",
  "keyProperty": "id"
}-->

```json
{
  "id" : "String",
  "userPrincipalName":"String",
  "userDisplayName": "String",
  "authMethods": ["string"],
  "isRegistered" : false,
  "isEnabled" : true,
  "isCapable" : false,
  "isMfaRegistered" : true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "credentialUserRegistrationDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


