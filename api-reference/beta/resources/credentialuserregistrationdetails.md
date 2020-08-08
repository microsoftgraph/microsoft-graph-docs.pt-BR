---
title: tipo de recurso credentialUserRegistrationDetails
description: Representa os detalhes do uso da redefinição de senha de autoatendimento e da MFA (autenticação multifator) para todos os usuários registrados.
localization_priority: Normal
author: khotz
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: fb852bb20fa8564f81e3dbcb027fced3d630f36b
ms.sourcegitcommit: bbff139eea483faaa2d1dd08af39314f35ef48ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/08/2020
ms.locfileid: "46598455"
---
# <a name="credentialuserregistrationdetails-resource-type"></a><span data-ttu-id="712c7-103">tipo de recurso credentialUserRegistrationDetails</span><span class="sxs-lookup"><span data-stu-id="712c7-103">credentialUserRegistrationDetails resource type</span></span>

<span data-ttu-id="712c7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="712c7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="712c7-105">Representa os detalhes do uso da redefinição de senha de autoatendimento e da MFA (autenticação multifator) para todos os usuários registrados.</span><span class="sxs-lookup"><span data-stu-id="712c7-105">Represents the details of the usage of self-service password reset and multi-factor authentication (MFA) for all registered users.</span></span> <span data-ttu-id="712c7-106">Os detalhes incluem informações do usuário, status do registro e o método de autenticação usado.</span><span class="sxs-lookup"><span data-stu-id="712c7-106">Details include user information, status of registration, and the authentication method used.</span></span>

## <a name="methods"></a><span data-ttu-id="712c7-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="712c7-107">Methods</span></span>

| <span data-ttu-id="712c7-108">Método</span><span class="sxs-lookup"><span data-stu-id="712c7-108">Method</span></span>       | <span data-ttu-id="712c7-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="712c7-109">Return Type</span></span> | <span data-ttu-id="712c7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="712c7-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="712c7-111">Listar credentialUserRegistrationDetails</span><span class="sxs-lookup"><span data-stu-id="712c7-111">List credentialUserRegistrationDetails</span></span>](../api/reportroot-list-credentialuserregistrationdetails.md) | <span data-ttu-id="712c7-112">coleção credentialUserRegistrationDetails</span><span class="sxs-lookup"><span data-stu-id="712c7-112">credentialUserRegistrationDetails collection</span></span> | <span data-ttu-id="712c7-113">Obter uma lista de objetos [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) para um determinado locatário.</span><span class="sxs-lookup"><span data-stu-id="712c7-113">Get a list of [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) objects for a given tenant.</span></span>
 |

## <a name="properties"></a><span data-ttu-id="712c7-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="712c7-114">Properties</span></span>

| <span data-ttu-id="712c7-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="712c7-115">Property</span></span>     | <span data-ttu-id="712c7-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="712c7-116">Type</span></span>        | <span data-ttu-id="712c7-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="712c7-117">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="712c7-118">authMethods</span><span class="sxs-lookup"><span data-stu-id="712c7-118">authMethods</span></span> | <span data-ttu-id="712c7-119">coleção registrationAuthMethod</span><span class="sxs-lookup"><span data-stu-id="712c7-119">registrationAuthMethod collection</span></span> | <span data-ttu-id="712c7-120">Representa o método de autenticação que o usuário registrou.</span><span class="sxs-lookup"><span data-stu-id="712c7-120">Represents the authentication method that the user has registered.</span></span> <span data-ttu-id="712c7-121">Os valores possíveis são: `email` , `mobilePhone` , `officePhone` , `securityQuestion` (usado somente para redefinição de senha de autoatendimento),, `appNotification` `appCode` e `alternateMobilePhone` (com suporte apenas no registro).</span><span class="sxs-lookup"><span data-stu-id="712c7-121">Possible values are: `email`, `mobilePhone`, `officePhone`, `securityQuestion` (only used for self-service password reset), `appNotification`, `appCode`, and `alternateMobilePhone` (supported only in registration).</span></span> |
| <span data-ttu-id="712c7-122">id</span><span class="sxs-lookup"><span data-stu-id="712c7-122">id</span></span> | <span data-ttu-id="712c7-123">String</span><span class="sxs-lookup"><span data-stu-id="712c7-123">String</span></span> | <span data-ttu-id="712c7-124">O identificador exclusivo da atividade.</span><span class="sxs-lookup"><span data-stu-id="712c7-124">The unique identifier for the activity.</span></span> <span data-ttu-id="712c7-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="712c7-125">Read-only.</span></span>|
| <span data-ttu-id="712c7-126">iscapable</span><span class="sxs-lookup"><span data-stu-id="712c7-126">isCapable</span></span> | <span data-ttu-id="712c7-127">Booliano</span><span class="sxs-lookup"><span data-stu-id="712c7-127">Boolean</span></span> | <span data-ttu-id="712c7-128">Indica se o usuário está pronto para executar a redefinição de senha de autoatendimento ou a MFA.</span><span class="sxs-lookup"><span data-stu-id="712c7-128">Indicates whether the user is ready to perform self-service password reset or MFA.</span></span> |
| <span data-ttu-id="712c7-129">isEnabled</span><span class="sxs-lookup"><span data-stu-id="712c7-129">isEnabled</span></span> | <span data-ttu-id="712c7-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="712c7-130">Boolean</span></span> | <span data-ttu-id="712c7-131">Indiciates se o usuário está habilitado para executar redefinição de senha de autoatendimento.</span><span class="sxs-lookup"><span data-stu-id="712c7-131">Indiciates whether the user enabled to perform self-service password reset.</span></span> |
| <span data-ttu-id="712c7-132">isMfaRegistered</span><span class="sxs-lookup"><span data-stu-id="712c7-132">isMfaRegistered</span></span> | <span data-ttu-id="712c7-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="712c7-133">Boolean</span></span> | <span data-ttu-id="712c7-134">Indiciates se o usuário está registrado para MFA.</span><span class="sxs-lookup"><span data-stu-id="712c7-134">Indiciates whether the user is registered for MFA.</span></span> |
| <span data-ttu-id="712c7-135">IsRegistered</span><span class="sxs-lookup"><span data-stu-id="712c7-135">isRegistered</span></span> | <span data-ttu-id="712c7-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="712c7-136">Boolean</span></span> | <span data-ttu-id="712c7-137">Indica se o usuário registrou todos os métodos de autenticação para redefinição de senha de autoatendimento.</span><span class="sxs-lookup"><span data-stu-id="712c7-137">Indicates whether the user has registered any authentication methods for self-service password reset.</span></span> |
| <span data-ttu-id="712c7-138">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="712c7-138">userDisplayName</span></span> | <span data-ttu-id="712c7-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="712c7-139">String</span></span> | <span data-ttu-id="712c7-140">Fornece o nome de usuário do usuário correspondente.</span><span class="sxs-lookup"><span data-stu-id="712c7-140">Provides the user name of the corresponding user.</span></span> |
| <span data-ttu-id="712c7-141">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="712c7-141">userPrincipalName</span></span> | <span data-ttu-id="712c7-142">String</span><span class="sxs-lookup"><span data-stu-id="712c7-142">String</span></span> | <span data-ttu-id="712c7-143">Fornece o nome principal de usuário do usuário correspondente.</span><span class="sxs-lookup"><span data-stu-id="712c7-143">Provides the user principal name of the corresponding user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="712c7-144">Relações</span><span class="sxs-lookup"><span data-stu-id="712c7-144">Relationships</span></span>

<span data-ttu-id="712c7-145">Nenhum</span><span class="sxs-lookup"><span data-stu-id="712c7-145">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="712c7-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="712c7-146">JSON representation</span></span>

<span data-ttu-id="712c7-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="712c7-147">The following is a JSON representation of the resource.</span></span>

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
