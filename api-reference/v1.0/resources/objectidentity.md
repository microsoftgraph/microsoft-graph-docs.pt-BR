---
title: tipo de recurso objectidentity
description: Representa uma identidade usada para entrar em uma conta de usuário.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: users
author: krbain
ms.openlocfilehash: 61d5e664d9a905f8d009aa2752ac2bcd54b0fd29
ms.sourcegitcommit: 195fa0d441a49662e144323d37518dbba0c76fc7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2020
ms.locfileid: "43806834"
---
# <a name="objectidentity-resource-type"></a><span data-ttu-id="60a4e-103">tipo de recurso objectidentity</span><span class="sxs-lookup"><span data-stu-id="60a4e-103">objectIdentity resource type</span></span>

<span data-ttu-id="60a4e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60a4e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="60a4e-105">Representa uma identidade usada para entrar em uma conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="60a4e-105">Represents an identity used to sign in to a user account.</span></span> <span data-ttu-id="60a4e-106">Uma identidade pode ser fornecida pela Microsoft, por organizações ou por provedores de identidade social, como Facebook, Google ou Microsoft, que estão vinculados a uma conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="60a4e-106">An identity can be provided by Microsoft, by organizations, or by social identity providers such as Facebook, Google, or Microsoft, that are tied to a user account.</span></span> <span data-ttu-id="60a4e-107">Isso permite que o usuário entre na conta de usuário com qualquer uma dessas identidades associadas.</span><span class="sxs-lookup"><span data-stu-id="60a4e-107">This enables the user to sign in to the user account with any of those associated identities.</span></span>

<span data-ttu-id="60a4e-108">A propriedade **Identities** do recurso [User](user.md) é um objeto **objectidentity** .</span><span class="sxs-lookup"><span data-stu-id="60a4e-108">The **identities** property of the [user](user.md) resource is an **objectIdentity** object.</span></span>

## <a name="properties"></a><span data-ttu-id="60a4e-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="60a4e-109">Properties</span></span>

| <span data-ttu-id="60a4e-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="60a4e-110">Property</span></span>   | <span data-ttu-id="60a4e-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="60a4e-111">Type</span></span> |<span data-ttu-id="60a4e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="60a4e-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="60a4e-113">signInType</span><span class="sxs-lookup"><span data-stu-id="60a4e-113">signInType</span></span>|<span data-ttu-id="60a4e-114">string</span><span class="sxs-lookup"><span data-stu-id="60a4e-114">string</span></span>| <span data-ttu-id="60a4e-115">Especifica os tipos de entrada do usuário no seu diretório, `emailAddress`como `userName` ou. `federated`</span><span class="sxs-lookup"><span data-stu-id="60a4e-115">Specifies the user sign-in types in your directory, such as `emailAddress`, `userName` or `federated`.</span></span> <span data-ttu-id="60a4e-116">Aqui, `federated` representa um identificador exclusivo para um usuário de um emissor, que pode estar em qualquer formato escolhido pelo emissor.</span><span class="sxs-lookup"><span data-stu-id="60a4e-116">Here, `federated` represents a unique identifier for a user from an issuer, that can be in any format chosen by the issuer.</span></span> <span data-ttu-id="60a4e-117">A validação adicional é imposta no **issuerAssignedId** quando o tipo de entrada é definido como `emailAddress` ou. `userName`</span><span class="sxs-lookup"><span data-stu-id="60a4e-117">Additional validation is enforced on **issuerAssignedId** when the sign-in type is set to `emailAddress` or `userName`.</span></span> <span data-ttu-id="60a4e-118">Essa propriedade também pode ser definida como qualquer cadeia de caracteres personalizada.</span><span class="sxs-lookup"><span data-stu-id="60a4e-118">This property can also be set to any custom string.</span></span>|
|<span data-ttu-id="60a4e-119">emissor</span><span class="sxs-lookup"><span data-stu-id="60a4e-119">issuer</span></span>|<span data-ttu-id="60a4e-120">string</span><span class="sxs-lookup"><span data-stu-id="60a4e-120">string</span></span>|<span data-ttu-id="60a4e-121">Especifica o emissor da identidade, por exemplo `facebook.com`.</span><span class="sxs-lookup"><span data-stu-id="60a4e-121">Specifies the issuer of the identity, for example `facebook.com`.</span></span><br><span data-ttu-id="60a4e-122">Para contas locais (onde **signInType** não `federated`é), essa propriedade é o nome de domínio padrão do locatário do B2C local `contoso.onmicrosoft.com`, por exemplo.</span><span class="sxs-lookup"><span data-stu-id="60a4e-122">For local accounts (where **signInType** is not `federated`), this property is the local B2C tenant default domain name, for example `contoso.onmicrosoft.com`.</span></span><br><span data-ttu-id="60a4e-123">Para usuários externos de outra organização do Azure AD, esse será o domínio da organização federada, por exemplo `contoso.com`.</span><span class="sxs-lookup"><span data-stu-id="60a4e-123">For external users from other Azure AD organization, this will be the domain of the federated organization, for example `contoso.com`.</span></span><br><br><span data-ttu-id="60a4e-124">Suporte `$filter`.</span><span class="sxs-lookup"><span data-stu-id="60a4e-124">Supports `$filter`.</span></span> <span data-ttu-id="60a4e-125">limite de caracteres de 512.</span><span class="sxs-lookup"><span data-stu-id="60a4e-125">512 character limit.</span></span>|
|<span data-ttu-id="60a4e-126">issuerAssignedId</span><span class="sxs-lookup"><span data-stu-id="60a4e-126">issuerAssignedId</span></span>|<span data-ttu-id="60a4e-127">string</span><span class="sxs-lookup"><span data-stu-id="60a4e-127">string</span></span>|<span data-ttu-id="60a4e-128">Especifica o identificador exclusivo atribuído ao usuário pelo emissor.</span><span class="sxs-lookup"><span data-stu-id="60a4e-128">Specifies the unique identifier assigned to the user by the issuer.</span></span> <span data-ttu-id="60a4e-129">A combinação de **Issuer** e **issuerAssignedId** deve ser exclusiva dentro da organização.</span><span class="sxs-lookup"><span data-stu-id="60a4e-129">The combination of **issuer** and **issuerAssignedId** must be unique within the organization.</span></span> <span data-ttu-id="60a4e-130">Representa o nome de entrada do usuário, quando **signInType** é definido como `emailAddress` ou `userName` (também conhecido como contas locais).</span><span class="sxs-lookup"><span data-stu-id="60a4e-130">Represents the sign-in name for the user, when **signInType** is set to `emailAddress` or `userName` (also known as local accounts).</span></span><br><span data-ttu-id="60a4e-131">Quando **signInType** é definido como:</span><span class="sxs-lookup"><span data-stu-id="60a4e-131">When **signInType** is set to:</span></span> <ul><li><span data-ttu-id="60a4e-132">`emailAddress`, (ou começa com `emailAddress` like `emailAddress1`) **issuerAssignedId** deve ser um endereço de email válido</span><span class="sxs-lookup"><span data-stu-id="60a4e-132">`emailAddress`, (or starts with `emailAddress` like `emailAddress1`) **issuerAssignedId** must be a valid email address</span></span></li><li><span data-ttu-id="60a4e-133">`userName`, **issuerAssignedId** deve ser uma [parte local válida de um endereço de email](https://tools.ietf.org/html/rfc3696#section-3)</span><span class="sxs-lookup"><span data-stu-id="60a4e-133">`userName`, **issuerAssignedId** must be a valid [local part of an email address](https://tools.ietf.org/html/rfc3696#section-3)</span></span></li></ul><span data-ttu-id="60a4e-134">Suporte `$filter`.</span><span class="sxs-lookup"><span data-stu-id="60a4e-134">Supports `$filter`.</span></span> <span data-ttu-id="60a4e-135">limite de caracteres de 512.</span><span class="sxs-lookup"><span data-stu-id="60a4e-135">512 character limit.</span></span>|

><span data-ttu-id="60a4e-136">**Observação:** Ao filtrar na propriedade **Identities** , você deve fornecer o **emissor** e o **issuerAssignedId**.</span><span class="sxs-lookup"><span data-stu-id="60a4e-136">**Note:** When filtering on the **identities** property, you must supply both **issuer** and **issuerAssignedId**.</span></span>

## <a name="json-representation"></a><span data-ttu-id="60a4e-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="60a4e-137">JSON representation</span></span>

<span data-ttu-id="60a4e-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="60a4e-138">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.objectIdentity"
}-->

```json
{
  "signInType": "string",
  "issuer": "string",
  "issuerAssignedId": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "objectIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
