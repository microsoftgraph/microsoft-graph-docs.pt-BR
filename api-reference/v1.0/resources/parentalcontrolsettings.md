---
title: tipo de recurso parentalControlSettings
description: Especifica as configurações de controle parental de um aplicativo. Essas configurações controlam a experiência de consentimento.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: bec744a555cd7aa71d9dbf577f6006980501ac61
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447231"
---
# <a name="parentalcontrolsettings-resource-type"></a><span data-ttu-id="f9b5c-104">tipo de recurso parentalControlSettings</span><span class="sxs-lookup"><span data-stu-id="f9b5c-104">parentalControlSettings resource type</span></span>

<span data-ttu-id="f9b5c-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f9b5c-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f9b5c-106">Especifica as configurações de controle parental de um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f9b5c-106">Specifies parental control settings for an application.</span></span> <span data-ttu-id="f9b5c-107">Essas configurações controlam a experiência de consentimento.</span><span class="sxs-lookup"><span data-stu-id="f9b5c-107">These settings control the consent experience.</span></span>

## <a name="properties"></a><span data-ttu-id="f9b5c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f9b5c-108">Properties</span></span>

| <span data-ttu-id="f9b5c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f9b5c-109">Property</span></span> | <span data-ttu-id="f9b5c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9b5c-110">Type</span></span> | <span data-ttu-id="f9b5c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9b5c-111">Description</span></span> |
:---------------|:--------|:----------|
|<span data-ttu-id="f9b5c-112">countriesBlockedForMinors</span><span class="sxs-lookup"><span data-stu-id="f9b5c-112">countriesBlockedForMinors</span></span>|<span data-ttu-id="f9b5c-113">String collection</span><span class="sxs-lookup"><span data-stu-id="f9b5c-113">String collection</span></span>| <span data-ttu-id="f9b5c-114">Especifica os [códigos de país ISO de duas letras](https://www.iso.org/iso-3166-country-codes.html).</span><span class="sxs-lookup"><span data-stu-id="f9b5c-114">Specifies the [two-letter ISO country codes](https://www.iso.org/iso-3166-country-codes.html).</span></span> <span data-ttu-id="f9b5c-115">O acesso ao aplicativo será bloqueado para menores dos países especificados nesta lista.</span><span class="sxs-lookup"><span data-stu-id="f9b5c-115">Access to the application will be blocked for minors from the countries specified in this list.</span></span>|
|<span data-ttu-id="f9b5c-116">legalAgeGroupRule</span><span class="sxs-lookup"><span data-stu-id="f9b5c-116">legalAgeGroupRule</span></span>| <span data-ttu-id="f9b5c-117">String</span><span class="sxs-lookup"><span data-stu-id="f9b5c-117">String</span></span> | <span data-ttu-id="f9b5c-118">Especifica a regra de grupo de idades legais que se aplica aos usuários do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f9b5c-118">Specifies the legal age group rule that applies to users of the app.</span></span> <span data-ttu-id="f9b5c-119">Pode ser definido como um dos seguintes valores:</span><span class="sxs-lookup"><span data-stu-id="f9b5c-119">Can be set to one of the following values:</span></span> <table><tr><th><span data-ttu-id="f9b5c-120">Valor</span><span class="sxs-lookup"><span data-stu-id="f9b5c-120">Value</span></span></th><th><span data-ttu-id="f9b5c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9b5c-121">Description</span></span></th></tr><tr><td><span data-ttu-id="f9b5c-122">Permitir</span><span class="sxs-lookup"><span data-stu-id="f9b5c-122">Allow</span></span></td><td><span data-ttu-id="f9b5c-123">Padrão.</span><span class="sxs-lookup"><span data-stu-id="f9b5c-123">Default.</span></span> <span data-ttu-id="f9b5c-124">Impõe o mínimo legal.</span><span class="sxs-lookup"><span data-stu-id="f9b5c-124">Enforces the legal minimum.</span></span> <span data-ttu-id="f9b5c-125">Isso significa que o consentimento do responsável é obrigatório para menores na União Européia e na Coréia.</span><span class="sxs-lookup"><span data-stu-id="f9b5c-125">This means parental consent is required for minors in the European Union and Korea.</span></span></td></tr><tr><td><span data-ttu-id="f9b5c-126">RequireConsentForPrivacyServices</span><span class="sxs-lookup"><span data-stu-id="f9b5c-126">RequireConsentForPrivacyServices</span></span></td><td><span data-ttu-id="f9b5c-127">Impõe que o usuário especifique a data de nascimento para estar em conformidade com as regras do COOPA.</span><span class="sxs-lookup"><span data-stu-id="f9b5c-127">Enforces the user to specify date of birth to comply with COPPA rules.</span></span> </td></tr><tr><td><span data-ttu-id="f9b5c-128">RequireConsentForMinors</span><span class="sxs-lookup"><span data-stu-id="f9b5c-128">RequireConsentForMinors</span></span></td><td><span data-ttu-id="f9b5c-129">Requer o consentimento dos pais para crianças abaixo de 18, independentemente das regras secundárias do país.</span><span class="sxs-lookup"><span data-stu-id="f9b5c-129">Requires parental consent for ages below 18, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="f9b5c-130">RequireConsentForKids</span><span class="sxs-lookup"><span data-stu-id="f9b5c-130">RequireConsentForKids</span></span></td><td><span data-ttu-id="f9b5c-131">Requer o consentimento dos pais para crianças abaixo de 14, independentemente das regras secundárias do país.</span><span class="sxs-lookup"><span data-stu-id="f9b5c-131">Requires parental consent for ages below 14, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="f9b5c-132">BlockMinors</span><span class="sxs-lookup"><span data-stu-id="f9b5c-132">BlockMinors</span></span></td><td><span data-ttu-id="f9b5c-133">Bloqueia os menores de usar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f9b5c-133">Blocks minors from using the app.</span></span></td></tr></table> |

## <a name="json-representation"></a><span data-ttu-id="f9b5c-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f9b5c-134">JSON representation</span></span>
<span data-ttu-id="f9b5c-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f9b5c-135">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.parentalControlSettings"
}-->
```json
{
  "countriesBlockedForMinors": [ "String" ],
  "legalAgeGroupRule": "String"
}

```
