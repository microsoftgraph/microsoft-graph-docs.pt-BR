---
title: tipo de recurso credentialUserRegistrationDetails
description: Representa os detalhes do uso da redefinição de senha de autoatendimento e da MFA (autenticação multifator) para todos os usuários registrados.
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 414cd6977f4e3c15ab7b82bd88329e9e3549f137
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35518661"
---
# <a name="credentialuserregistrationdetails-resource-type"></a><span data-ttu-id="fea10-103">tipo de recurso credentialUserRegistrationDetails</span><span class="sxs-lookup"><span data-stu-id="fea10-103">credentialUserRegistrationDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fea10-104">Representa os detalhes do uso da redefinição de senha de autoatendimento e da MFA (autenticação multifator) para todos os usuários registrados.</span><span class="sxs-lookup"><span data-stu-id="fea10-104">Represents the details of the usage of self-service password reset and multi-factor authentication (MFA) for all registered users.</span></span> <span data-ttu-id="fea10-105">Os detalhes incluem informações do usuário, status do registro e o método de autenticação usado.</span><span class="sxs-lookup"><span data-stu-id="fea10-105">Details include user information, status of registration, and the authentication method used.</span></span>

## <a name="methods"></a><span data-ttu-id="fea10-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="fea10-106">Methods</span></span>

| <span data-ttu-id="fea10-107">Método</span><span class="sxs-lookup"><span data-stu-id="fea10-107">Method</span></span>       | <span data-ttu-id="fea10-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fea10-108">Return Type</span></span> | <span data-ttu-id="fea10-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="fea10-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="fea10-110">Listar credentialUserRegistrationDetails</span><span class="sxs-lookup"><span data-stu-id="fea10-110">List credentialUserRegistrationDetails</span></span>](../api/reportroot-list-credentialuserregistrationdetails.md) | <span data-ttu-id="fea10-111">coleção credentialUserRegistrationDetails</span><span class="sxs-lookup"><span data-stu-id="fea10-111">credentialUserRegistrationDetails collection</span></span> | <span data-ttu-id="fea10-112">Obter uma lista de objetos [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) para um determinado locatário.</span><span class="sxs-lookup"><span data-stu-id="fea10-112">Get a list of [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) objects for a given tenant.</span></span>
 |

## <a name="properties"></a><span data-ttu-id="fea10-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fea10-113">Properties</span></span>

| <span data-ttu-id="fea10-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fea10-114">Property</span></span>     | <span data-ttu-id="fea10-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="fea10-115">Type</span></span>        | <span data-ttu-id="fea10-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="fea10-116">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="fea10-117">authMethods</span><span class="sxs-lookup"><span data-stu-id="fea10-117">authMethods</span></span> | <span data-ttu-id="fea10-118">coleção registrationAuthMethod</span><span class="sxs-lookup"><span data-stu-id="fea10-118">registrationAuthMethod collection</span></span> | <span data-ttu-id="fea10-119">Representa o método de autenticação usado pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="fea10-119">Represents the authentication method that the user used.</span></span> <span data-ttu-id="fea10-120">Os valores possíveis são `email`: `mobilePhone`, `officePhone`, `securityQuestion` , (usado somente para redefinição de senha de autoatendimento `appCode`), `alternateMobilePhone` `appNotification`, e (com suporte apenas no registro).</span><span class="sxs-lookup"><span data-stu-id="fea10-120">Possible values are: `email`, `mobilePhone`, `officePhone`, `securityQuestion` (only used for self-service password reset), `appNotification`, `appCode`, and `alternateMobilePhone` (supported only in registration).</span></span> |
| <span data-ttu-id="fea10-121">id</span><span class="sxs-lookup"><span data-stu-id="fea10-121">id</span></span> | <span data-ttu-id="fea10-122">String</span><span class="sxs-lookup"><span data-stu-id="fea10-122">String</span></span> | <span data-ttu-id="fea10-123">O identificador exclusivo da atividade.</span><span class="sxs-lookup"><span data-stu-id="fea10-123">The unique identifier for the activity.</span></span> <span data-ttu-id="fea10-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fea10-124">Read-only.</span></span>|
| <span data-ttu-id="fea10-125">iscapable</span><span class="sxs-lookup"><span data-stu-id="fea10-125">isCapable</span></span> | <span data-ttu-id="fea10-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="fea10-126">Boolean</span></span> | <span data-ttu-id="fea10-127">Indica se o usuário está pronto para executar a redefinição de senha de autoatendimento ou a MFA.</span><span class="sxs-lookup"><span data-stu-id="fea10-127">Indicates whether the user is ready to perform self-service password reset or MFA.</span></span> |
| <span data-ttu-id="fea10-128">isEnabled</span><span class="sxs-lookup"><span data-stu-id="fea10-128">isEnabled</span></span> | <span data-ttu-id="fea10-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="fea10-129">Boolean</span></span> | <span data-ttu-id="fea10-130">Indiciates se o usuário está habilitado para executar redefinição de senha de autoatendimento.</span><span class="sxs-lookup"><span data-stu-id="fea10-130">Indiciates whether the user enabled to perform self-service password reset.</span></span> |
| <span data-ttu-id="fea10-131">isMfaRegistered</span><span class="sxs-lookup"><span data-stu-id="fea10-131">isMfaRegistered</span></span> | <span data-ttu-id="fea10-132">Booliano</span><span class="sxs-lookup"><span data-stu-id="fea10-132">Boolean</span></span> | <span data-ttu-id="fea10-133">Indiciates se o usuário está registrado para MFA.</span><span class="sxs-lookup"><span data-stu-id="fea10-133">Indiciates whether the user is registered for MFA.</span></span> |
| <span data-ttu-id="fea10-134">IsRegistered</span><span class="sxs-lookup"><span data-stu-id="fea10-134">isRegistered</span></span> | <span data-ttu-id="fea10-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="fea10-135">Boolean</span></span> | <span data-ttu-id="fea10-136">Indica se o usuário registrou todos os métodos de autenticação para redefinição de senha de autoatendimento.</span><span class="sxs-lookup"><span data-stu-id="fea10-136">Indicates whether the user has registered any authentication methods for self-service password reset.</span></span> |
| <span data-ttu-id="fea10-137">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="fea10-137">userDisplayName</span></span> | <span data-ttu-id="fea10-138">String</span><span class="sxs-lookup"><span data-stu-id="fea10-138">String</span></span> | <span data-ttu-id="fea10-139">Fornece o nome de usuário do usuário correspondente.</span><span class="sxs-lookup"><span data-stu-id="fea10-139">Provides the user name of the corresponding user.</span></span> |
| <span data-ttu-id="fea10-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fea10-140">userPrincipalName</span></span> | <span data-ttu-id="fea10-141">String</span><span class="sxs-lookup"><span data-stu-id="fea10-141">String</span></span> | <span data-ttu-id="fea10-142">Fornece o nome principal de usuário do usuário correspondente.</span><span class="sxs-lookup"><span data-stu-id="fea10-142">Provides the user principal name of the corresponding user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="fea10-143">Relações</span><span class="sxs-lookup"><span data-stu-id="fea10-143">Relationships</span></span>

<span data-ttu-id="fea10-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fea10-144">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fea10-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fea10-145">JSON representation</span></span>

<span data-ttu-id="fea10-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fea10-146">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.credentialUserRegistrationDetails",
  "baseType": "",
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