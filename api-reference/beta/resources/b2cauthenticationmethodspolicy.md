---
title: Tipo de recurso b2cAuthenticationMethodsPolicy
description: Representa um método de autenticação de conta local registrado para um usuário configurado em um locatário Azure Active Directory (Azure AD) B2C.
localization_priority: Priority
author: namkedia
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 74b18a2a0bc6d0ace2062f07d44eb175f7ad39e9
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161758"
---
# <a name="b2cauthenticationmethodspolicy-resource-type"></a><span data-ttu-id="0eacb-103">Tipo de recurso b2cAuthenticationMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="0eacb-103">b2cAuthenticationMethodsPolicy resource type</span></span>

<span data-ttu-id="0eacb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0eacb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0eacb-105">O Azure Active Directory (Azure AD) B2C permite que os administradores de locatários escolham um mecanismo para permitir que os usuários finais se registrem por meio de contas locais.</span><span class="sxs-lookup"><span data-stu-id="0eacb-105">Azure Active Directory (Azure AD) B2C allows tenant admins to choose a mechanism for letting end users register via local accounts.</span></span> <span data-ttu-id="0eacb-106">Contas locais são as contas em que o Azure AD faz a asserção de identidade, em oposição a um provedor de identidade federada, como Google ou Facebook, etc.</span><span class="sxs-lookup"><span data-stu-id="0eacb-106">Local accounts are the accounts where Azure AD does the identity assertion, as opposed to a federated identity provider such as Google or Facebook etc.</span></span>

<span data-ttu-id="0eacb-107">As contas locais no Azure AD B2C não seguem as configurações ou paradigmas do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0eacb-107">The local accounts in Azure AD B2C do not follow the settings or paradigms from Azure AD.</span></span> <span data-ttu-id="0eacb-108">A política de métodos de autenticação do Azure AD não é usada ou aplicada pelo Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="0eacb-108">The Azure AD authentication methods policy is not used or enforced by Azure AD B2C.</span></span> <span data-ttu-id="0eacb-109">O Azure AD B2C armazena essas configurações em uma política diferente, que é consumida pelos fluxos do usuário.</span><span class="sxs-lookup"><span data-stu-id="0eacb-109">Azure AD B2C stores these settings in a different policy, which is consumed by user flows.</span></span>

## <a name="methods"></a><span data-ttu-id="0eacb-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="0eacb-110">Methods</span></span>

| <span data-ttu-id="0eacb-111">Método</span><span class="sxs-lookup"><span data-stu-id="0eacb-111">Method</span></span>       | <span data-ttu-id="0eacb-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0eacb-112">Return type</span></span> | <span data-ttu-id="0eacb-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="0eacb-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="0eacb-114">Obter b2cAuthenticationMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="0eacb-114">Get b2cAuthenticationMethodsPolicy</span></span>](../api/b2cauthenticationmethodspolicy-get.md) | [<span data-ttu-id="0eacb-115">b2cauthenticationmethodspolicy</span><span class="sxs-lookup"><span data-stu-id="0eacb-115">b2cauthenticationmethodspolicy</span></span>](b2cauthenticationmethodspolicy.md) | <span data-ttu-id="0eacb-116">Leia as propriedades de um objeto **b2cAuthenticationMethodsPolicy**.</span><span class="sxs-lookup"><span data-stu-id="0eacb-116">Read the properties of a **b2cauthenticationmethodspolicy** object.</span></span> |
| [<span data-ttu-id="0eacb-117">Atualizar b2cAuthenticationMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="0eacb-117">Update b2cAuthenticationMethodsPolicy</span></span>](../api/b2cauthenticationmethodspolicy-update.md) | <span data-ttu-id="0eacb-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0eacb-118">None</span></span> | <span data-ttu-id="0eacb-119">Atualize as propriedades de um objeto **b2cAuthenticationMethodsPolicy**.</span><span class="sxs-lookup"><span data-stu-id="0eacb-119">Update the properties of a **b2cauthenticationmethodspolicy** objects.</span></span> |

## <a name="properties"></a><span data-ttu-id="0eacb-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0eacb-120">Properties</span></span>

| <span data-ttu-id="0eacb-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0eacb-121">Property</span></span>     | <span data-ttu-id="0eacb-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="0eacb-122">Type</span></span>        | <span data-ttu-id="0eacb-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="0eacb-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0eacb-124">id</span><span class="sxs-lookup"><span data-stu-id="0eacb-124">id</span></span>|<span data-ttu-id="0eacb-125">String</span><span class="sxs-lookup"><span data-stu-id="0eacb-125">String</span></span>|<span data-ttu-id="0eacb-126">A id da política de métodos de autenticação do B2C.</span><span class="sxs-lookup"><span data-stu-id="0eacb-126">The id of the B2C authentication methods policy.</span></span> <span data-ttu-id="0eacb-127">Esta é a chave e uma propriedade somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0eacb-127">This is a read only property and the key.</span></span>|
|<span data-ttu-id="0eacb-128">isEmailPasswordAuthenticationEnabled</span><span class="sxs-lookup"><span data-stu-id="0eacb-128">isEmailPasswordAuthenticationEnabled</span></span>|<span data-ttu-id="0eacb-129">Booliano</span><span class="sxs-lookup"><span data-stu-id="0eacb-129">Boolean</span></span>|<span data-ttu-id="0eacb-130">O administrador de locatário pode configurar contas locais usando o email se o método de autenticação de email e senha estiver habilitado.</span><span class="sxs-lookup"><span data-stu-id="0eacb-130">The tenant admin can configure local accounts using email if the email and password authentication method is enabled.</span></span>|
|<span data-ttu-id="0eacb-131">isUserNameAuthenticationEnabled</span><span class="sxs-lookup"><span data-stu-id="0eacb-131">isUserNameAuthenticationEnabled</span></span>|<span data-ttu-id="0eacb-132">Booliano</span><span class="sxs-lookup"><span data-stu-id="0eacb-132">Boolean</span></span>|<span data-ttu-id="0eacb-133">O administrador de locatários pode configurar contas locais usando o nome de usuário se o método de autenticação do nome de usuário e senha estiver habilitado.</span><span class="sxs-lookup"><span data-stu-id="0eacb-133">The tenant admin can configure local accounts using username if the username and password authentication method is enabled.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0eacb-134">Relações</span><span class="sxs-lookup"><span data-stu-id="0eacb-134">Relationships</span></span>

<span data-ttu-id="0eacb-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0eacb-135">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0eacb-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0eacb-136">JSON representation</span></span>

<span data-ttu-id="0eacb-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0eacb-137">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.b2cAuthenticationMethodsPolicy",
  "keyProperty": "id"
}-->

```json
{
    "id": "b2CAuthenticationMethodsPolicy",
    "isEmailPasswordAuthenticationEnabled": true,
    "isUserNameAuthenticationEnabled": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "b2cAuthenticationMethodsPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
