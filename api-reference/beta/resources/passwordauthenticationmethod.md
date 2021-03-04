---
title: tipo de recurso passwordAuthenticationMethod
description: Uma representação de uma senha registrada para um usuário.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 2982b79df70b65bf09dff8f9b906ed85a8854b52
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444081"
---
# <a name="passwordauthenticationmethod-resource-type"></a><span data-ttu-id="0b588-103">tipo de recurso passwordAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0b588-103">passwordAuthenticationMethod resource type</span></span>

<span data-ttu-id="0b588-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b588-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b588-105">Uma representação da senha de um usuário.</span><span class="sxs-lookup"><span data-stu-id="0b588-105">A representation of a user's password.</span></span> <span data-ttu-id="0b588-106">Por segurança, a senha em si nunca será retornada no objeto, mas pode ser tomada uma ação para redefinir uma senha.</span><span class="sxs-lookup"><span data-stu-id="0b588-106">For security, the password itself will never be returned in the object, but action can be taken to reset a password.</span></span>

## <a name="methods"></a><span data-ttu-id="0b588-107">Methods</span><span class="sxs-lookup"><span data-stu-id="0b588-107">Methods</span></span>

| <span data-ttu-id="0b588-108">Método</span><span class="sxs-lookup"><span data-stu-id="0b588-108">Method</span></span>       | <span data-ttu-id="0b588-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0b588-109">Return Type</span></span> | <span data-ttu-id="0b588-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b588-110">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="0b588-111">Listar passwordAuthenticationMethods</span><span class="sxs-lookup"><span data-stu-id="0b588-111">List passwordAuthenticationMethods</span></span>](../api/authentication-list-passwordmethods.md) | <span data-ttu-id="0b588-112">[coleção passwordAuthenticationMethod](passwordauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="0b588-112">[passwordAuthenticationMethod](passwordauthenticationmethod.md) collection</span></span> | <span data-ttu-id="0b588-113">Leia as propriedades e as relações de todos os objetos **passwordAuthenticationMethod** deste usuário.</span><span class="sxs-lookup"><span data-stu-id="0b588-113">Read the properties and relationships of all of this user's **passwordAuthenticationMethod** objects.</span></span> |
|[<span data-ttu-id="0b588-114">Obter passwordAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0b588-114">Get passwordAuthenticationMethod</span></span>](../api/passwordauthenticationmethod-get.md) | [<span data-ttu-id="0b588-115">passwordAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0b588-115">passwordAuthenticationMethod</span></span>](passwordauthenticationmethod.md) | <span data-ttu-id="0b588-116">Leia as propriedades e as relações de um **objeto PasswordAuthenticationMethod.**</span><span class="sxs-lookup"><span data-stu-id="0b588-116">Read the properties and relationships of a **passwordAuthenticationMethod** object.</span></span> |
|[<span data-ttu-id="0b588-117">Redefinir senha</span><span class="sxs-lookup"><span data-stu-id="0b588-117">Reset password</span></span>](../api/passwordauthenticationmethod-resetpassword.md)|<span data-ttu-id="0b588-118">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="0b588-118">None</span></span>|<span data-ttu-id="0b588-119">Redefinir a senha de um usuário na nuvem e, se sincronizado, no local.</span><span class="sxs-lookup"><span data-stu-id="0b588-119">Reset a user's password in the cloud and, if synced, on-premises.</span></span>|

## <a name="properties"></a><span data-ttu-id="0b588-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0b588-120">Properties</span></span>

| <span data-ttu-id="0b588-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0b588-121">Property</span></span>     | <span data-ttu-id="0b588-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b588-122">Type</span></span>        | <span data-ttu-id="0b588-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b588-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0b588-124">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="0b588-124">creationDateTime</span></span>|<span data-ttu-id="0b588-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b588-125">DateTimeOffset</span></span>|<span data-ttu-id="0b588-126">A data e a hora em que essa senha foi atualizada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="0b588-126">The date and time when this password was last updated.</span></span> <span data-ttu-id="0b588-127">No momento, essa propriedade não está preenchida.</span><span class="sxs-lookup"><span data-stu-id="0b588-127">This property is currently not populated.</span></span> <span data-ttu-id="0b588-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0b588-128">Read-only.</span></span> <span data-ttu-id="0b588-129">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="0b588-129">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0b588-130">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="0b588-130">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="0b588-131">id</span><span class="sxs-lookup"><span data-stu-id="0b588-131">id</span></span>|<span data-ttu-id="0b588-132">String</span><span class="sxs-lookup"><span data-stu-id="0b588-132">String</span></span>| <span data-ttu-id="0b588-133">O identificador dessa senha registrado para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="0b588-133">The identifier of this password registered to this user.</span></span> <span data-ttu-id="0b588-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0b588-134">Read-only.</span></span>|
|<span data-ttu-id="0b588-135">password</span><span class="sxs-lookup"><span data-stu-id="0b588-135">password</span></span>|<span data-ttu-id="0b588-136">String</span><span class="sxs-lookup"><span data-stu-id="0b588-136">String</span></span>|<span data-ttu-id="0b588-137">Para segurança, a senha sempre é retornada como nula de uma operação LIST ou GET.</span><span class="sxs-lookup"><span data-stu-id="0b588-137">For security, the password is always returned as null from a LIST or GET operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b588-138">Relações</span><span class="sxs-lookup"><span data-stu-id="0b588-138">Relationships</span></span>

<span data-ttu-id="0b588-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0b588-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0b588-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0b588-140">JSON representation</span></span>

<span data-ttu-id="0b588-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0b588-141">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordAuthenticationMethod",
  "keyProperty": "id"
}-->

```json
{
  "creationDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "password": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordAuthenticationMethod resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


