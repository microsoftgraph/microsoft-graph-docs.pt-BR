---
title: tipo de recurso credentialUserRegistrationDetails
description: Representa os detalhes do uso da redefinição de senha de autoatendados e da autenticação multifatória (MFA) para todos os usuários registrados.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: ac5712bf3c0d396f7ddc84c4812b4e1ed7090355
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941810"
---
# <a name="credentialuserregistrationdetails-resource-type"></a><span data-ttu-id="8e28a-103">tipo de recurso credentialUserRegistrationDetails</span><span class="sxs-lookup"><span data-stu-id="8e28a-103">credentialUserRegistrationDetails resource type</span></span>

<span data-ttu-id="8e28a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e28a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e28a-105">Representa os detalhes do uso da redefinição de senha de autoatendados e da autenticação multifatória (MFA) para todos os usuários registrados.</span><span class="sxs-lookup"><span data-stu-id="8e28a-105">Represents the details of the usage of self-service password reset and multi-factor authentication (MFA) for all registered users.</span></span> <span data-ttu-id="8e28a-106">Os detalhes incluem informações do usuário, status do registro e o método de autenticação usado.</span><span class="sxs-lookup"><span data-stu-id="8e28a-106">Details include user information, status of registration, and the authentication method used.</span></span>

## <a name="methods"></a><span data-ttu-id="8e28a-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="8e28a-107">Methods</span></span>

| <span data-ttu-id="8e28a-108">Método</span><span class="sxs-lookup"><span data-stu-id="8e28a-108">Method</span></span>       | <span data-ttu-id="8e28a-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8e28a-109">Return Type</span></span> | <span data-ttu-id="8e28a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e28a-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="8e28a-111">Listar credentialUserRegistrationDetails</span><span class="sxs-lookup"><span data-stu-id="8e28a-111">List credentialUserRegistrationDetails</span></span>](../api/reportroot-list-credentialuserregistrationdetails.md) | <span data-ttu-id="8e28a-112">coleção credentialUserRegistrationDetails</span><span class="sxs-lookup"><span data-stu-id="8e28a-112">credentialUserRegistrationDetails collection</span></span> | <span data-ttu-id="8e28a-113">Obter uma lista de [objetos credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) para um determinado locatário.</span><span class="sxs-lookup"><span data-stu-id="8e28a-113">Get a list of [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) objects for a given tenant.</span></span>
 |

## <a name="properties"></a><span data-ttu-id="8e28a-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8e28a-114">Properties</span></span>

| <span data-ttu-id="8e28a-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8e28a-115">Property</span></span>     | <span data-ttu-id="8e28a-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e28a-116">Type</span></span>        | <span data-ttu-id="8e28a-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e28a-117">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="8e28a-118">authMethods</span><span class="sxs-lookup"><span data-stu-id="8e28a-118">authMethods</span></span> | <span data-ttu-id="8e28a-119">coleção registrationAuthMethod</span><span class="sxs-lookup"><span data-stu-id="8e28a-119">registrationAuthMethod collection</span></span> | <span data-ttu-id="8e28a-120">Representa o método de autenticação que o usuário registrou.</span><span class="sxs-lookup"><span data-stu-id="8e28a-120">Represents the authentication method that the user has registered.</span></span> <span data-ttu-id="8e28a-121">Os valores possíveis são: , , (usado apenas para redefinição de senha de `email` `mobilePhone` `officePhone`  `securityQuestion` autoatendido), , , (suportado somente `appNotification` no  `appCode` `alternateMobilePhone` registro), , ,  `fido`  `appPassword`  `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="8e28a-121">Possible values are: `email`, `mobilePhone`, `officePhone`,  `securityQuestion` (only used for self-service password reset), `appNotification`,  `appCode`, `alternateMobilePhone` (supported only in registration),  `fido`,  `appPassword`,  `unknownFutureValue`.</span></span> |
| <span data-ttu-id="8e28a-122">id</span><span class="sxs-lookup"><span data-stu-id="8e28a-122">id</span></span> | <span data-ttu-id="8e28a-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8e28a-123">String</span></span> | <span data-ttu-id="8e28a-124">O identificador exclusivo da atividade.</span><span class="sxs-lookup"><span data-stu-id="8e28a-124">The unique identifier for the activity.</span></span> <span data-ttu-id="8e28a-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e28a-125">Read-only.</span></span>|
| <span data-ttu-id="8e28a-126">isCapable</span><span class="sxs-lookup"><span data-stu-id="8e28a-126">isCapable</span></span> | <span data-ttu-id="8e28a-127">Booliano</span><span class="sxs-lookup"><span data-stu-id="8e28a-127">Boolean</span></span> | <span data-ttu-id="8e28a-128">Indica se o usuário está pronto para executar a redefinição de senha de autoatendados ou MFA.</span><span class="sxs-lookup"><span data-stu-id="8e28a-128">Indicates whether the user is ready to perform self-service password reset or MFA.</span></span> |
| <span data-ttu-id="8e28a-129">isEnabled</span><span class="sxs-lookup"><span data-stu-id="8e28a-129">isEnabled</span></span> | <span data-ttu-id="8e28a-130">Booliano</span><span class="sxs-lookup"><span data-stu-id="8e28a-130">Boolean</span></span> | <span data-ttu-id="8e28a-131">Indica se o usuário habilitado para executar a redefinição de senha de autoatendados.</span><span class="sxs-lookup"><span data-stu-id="8e28a-131">Indicates whether the user enabled to perform self-service password reset.</span></span> |
| <span data-ttu-id="8e28a-132">isMfaRegistered</span><span class="sxs-lookup"><span data-stu-id="8e28a-132">isMfaRegistered</span></span> | <span data-ttu-id="8e28a-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="8e28a-133">Boolean</span></span> | <span data-ttu-id="8e28a-134">Indica se o usuário está registrado para MFA.</span><span class="sxs-lookup"><span data-stu-id="8e28a-134">Indicates whether the user is registered for MFA.</span></span> |
| <span data-ttu-id="8e28a-135">isRegistered</span><span class="sxs-lookup"><span data-stu-id="8e28a-135">isRegistered</span></span> | <span data-ttu-id="8e28a-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="8e28a-136">Boolean</span></span> | <span data-ttu-id="8e28a-137">Indica se o usuário registrou quaisquer métodos de autenticação para redefinição de senha de autoatendados.</span><span class="sxs-lookup"><span data-stu-id="8e28a-137">Indicates whether the user has registered any authentication methods for self-service password reset.</span></span> |
| <span data-ttu-id="8e28a-138">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="8e28a-138">userDisplayName</span></span> | <span data-ttu-id="8e28a-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8e28a-139">String</span></span> | <span data-ttu-id="8e28a-140">Fornece o nome de usuário do usuário correspondente.</span><span class="sxs-lookup"><span data-stu-id="8e28a-140">Provides the user name of the corresponding user.</span></span> |
| <span data-ttu-id="8e28a-141">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8e28a-141">userPrincipalName</span></span> | <span data-ttu-id="8e28a-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8e28a-142">String</span></span> | <span data-ttu-id="8e28a-143">Fornece o nome principal do usuário do usuário correspondente.</span><span class="sxs-lookup"><span data-stu-id="8e28a-143">Provides the user principal name of the corresponding user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8e28a-144">Relações</span><span class="sxs-lookup"><span data-stu-id="8e28a-144">Relationships</span></span>

<span data-ttu-id="8e28a-145">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8e28a-145">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8e28a-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8e28a-146">JSON representation</span></span>

<span data-ttu-id="8e28a-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8e28a-147">The following is a JSON representation of the resource.</span></span>

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


