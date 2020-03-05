---
title: tipo de recurso credentialUserRegistrationDetails
description: Representa os detalhes do uso da redefinição de senha de autoatendimento e da MFA (autenticação multifator) para todos os usuários registrados.
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: c86a486223bd32857c17084244befe103a0942d4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507335"
---
# <a name="credentialuserregistrationdetails-resource-type"></a><span data-ttu-id="bf8ca-103">tipo de recurso credentialUserRegistrationDetails</span><span class="sxs-lookup"><span data-stu-id="bf8ca-103">credentialUserRegistrationDetails resource type</span></span>

<span data-ttu-id="bf8ca-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bf8ca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf8ca-105">Representa os detalhes do uso da redefinição de senha de autoatendimento e da MFA (autenticação multifator) para todos os usuários registrados.</span><span class="sxs-lookup"><span data-stu-id="bf8ca-105">Represents the details of the usage of self-service password reset and multi-factor authentication (MFA) for all registered users.</span></span> <span data-ttu-id="bf8ca-106">Os detalhes incluem informações do usuário, status do registro e o método de autenticação usado.</span><span class="sxs-lookup"><span data-stu-id="bf8ca-106">Details include user information, status of registration, and the authentication method used.</span></span>

## <a name="methods"></a><span data-ttu-id="bf8ca-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="bf8ca-107">Methods</span></span>

| <span data-ttu-id="bf8ca-108">Método</span><span class="sxs-lookup"><span data-stu-id="bf8ca-108">Method</span></span>       | <span data-ttu-id="bf8ca-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bf8ca-109">Return Type</span></span> | <span data-ttu-id="bf8ca-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf8ca-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="bf8ca-111">Listar credentialUserRegistrationDetails</span><span class="sxs-lookup"><span data-stu-id="bf8ca-111">List credentialUserRegistrationDetails</span></span>](../api/reportroot-list-credentialuserregistrationdetails.md) | <span data-ttu-id="bf8ca-112">coleção credentialUserRegistrationDetails</span><span class="sxs-lookup"><span data-stu-id="bf8ca-112">credentialUserRegistrationDetails collection</span></span> | <span data-ttu-id="bf8ca-113">Obter uma lista de objetos [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) para um determinado locatário.</span><span class="sxs-lookup"><span data-stu-id="bf8ca-113">Get a list of [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) objects for a given tenant.</span></span>
 |

## <a name="properties"></a><span data-ttu-id="bf8ca-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bf8ca-114">Properties</span></span>

| <span data-ttu-id="bf8ca-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bf8ca-115">Property</span></span>     | <span data-ttu-id="bf8ca-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="bf8ca-116">Type</span></span>        | <span data-ttu-id="bf8ca-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf8ca-117">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="bf8ca-118">authMethods</span><span class="sxs-lookup"><span data-stu-id="bf8ca-118">authMethods</span></span> | <span data-ttu-id="bf8ca-119">coleção registrationAuthMethod</span><span class="sxs-lookup"><span data-stu-id="bf8ca-119">registrationAuthMethod collection</span></span> | <span data-ttu-id="bf8ca-120">Representa o método de autenticação usado pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="bf8ca-120">Represents the authentication method that the user used.</span></span> <span data-ttu-id="bf8ca-121">Os valores possíveis são `email`: `mobilePhone`, `officePhone`, `securityQuestion` , (usado somente para redefinição de senha de autoatendimento `appCode`), `alternateMobilePhone` `appNotification`, e (com suporte apenas no registro).</span><span class="sxs-lookup"><span data-stu-id="bf8ca-121">Possible values are: `email`, `mobilePhone`, `officePhone`, `securityQuestion` (only used for self-service password reset), `appNotification`, `appCode`, and `alternateMobilePhone` (supported only in registration).</span></span> |
| <span data-ttu-id="bf8ca-122">id</span><span class="sxs-lookup"><span data-stu-id="bf8ca-122">id</span></span> | <span data-ttu-id="bf8ca-123">String</span><span class="sxs-lookup"><span data-stu-id="bf8ca-123">String</span></span> | <span data-ttu-id="bf8ca-124">O identificador exclusivo da atividade.</span><span class="sxs-lookup"><span data-stu-id="bf8ca-124">The unique identifier for the activity.</span></span> <span data-ttu-id="bf8ca-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bf8ca-125">Read-only.</span></span>|
| <span data-ttu-id="bf8ca-126">iscapable</span><span class="sxs-lookup"><span data-stu-id="bf8ca-126">isCapable</span></span> | <span data-ttu-id="bf8ca-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf8ca-127">Boolean</span></span> | <span data-ttu-id="bf8ca-128">Indica se o usuário está pronto para executar a redefinição de senha de autoatendimento ou a MFA.</span><span class="sxs-lookup"><span data-stu-id="bf8ca-128">Indicates whether the user is ready to perform self-service password reset or MFA.</span></span> |
| <span data-ttu-id="bf8ca-129">isEnabled</span><span class="sxs-lookup"><span data-stu-id="bf8ca-129">isEnabled</span></span> | <span data-ttu-id="bf8ca-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf8ca-130">Boolean</span></span> | <span data-ttu-id="bf8ca-131">Indiciates se o usuário está habilitado para executar redefinição de senha de autoatendimento.</span><span class="sxs-lookup"><span data-stu-id="bf8ca-131">Indiciates whether the user enabled to perform self-service password reset.</span></span> |
| <span data-ttu-id="bf8ca-132">isMfaRegistered</span><span class="sxs-lookup"><span data-stu-id="bf8ca-132">isMfaRegistered</span></span> | <span data-ttu-id="bf8ca-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf8ca-133">Boolean</span></span> | <span data-ttu-id="bf8ca-134">Indiciates se o usuário está registrado para MFA.</span><span class="sxs-lookup"><span data-stu-id="bf8ca-134">Indiciates whether the user is registered for MFA.</span></span> |
| <span data-ttu-id="bf8ca-135">IsRegistered</span><span class="sxs-lookup"><span data-stu-id="bf8ca-135">isRegistered</span></span> | <span data-ttu-id="bf8ca-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf8ca-136">Boolean</span></span> | <span data-ttu-id="bf8ca-137">Indica se o usuário registrou todos os métodos de autenticação para redefinição de senha de autoatendimento.</span><span class="sxs-lookup"><span data-stu-id="bf8ca-137">Indicates whether the user has registered any authentication methods for self-service password reset.</span></span> |
| <span data-ttu-id="bf8ca-138">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="bf8ca-138">userDisplayName</span></span> | <span data-ttu-id="bf8ca-139">String</span><span class="sxs-lookup"><span data-stu-id="bf8ca-139">String</span></span> | <span data-ttu-id="bf8ca-140">Fornece o nome de usuário do usuário correspondente.</span><span class="sxs-lookup"><span data-stu-id="bf8ca-140">Provides the user name of the corresponding user.</span></span> |
| <span data-ttu-id="bf8ca-141">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bf8ca-141">userPrincipalName</span></span> | <span data-ttu-id="bf8ca-142">String</span><span class="sxs-lookup"><span data-stu-id="bf8ca-142">String</span></span> | <span data-ttu-id="bf8ca-143">Fornece o nome principal de usuário do usuário correspondente.</span><span class="sxs-lookup"><span data-stu-id="bf8ca-143">Provides the user principal name of the corresponding user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="bf8ca-144">Relações</span><span class="sxs-lookup"><span data-stu-id="bf8ca-144">Relationships</span></span>

<span data-ttu-id="bf8ca-145">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bf8ca-145">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bf8ca-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bf8ca-146">JSON representation</span></span>

<span data-ttu-id="bf8ca-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bf8ca-147">The following is a JSON representation of the resource.</span></span>

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