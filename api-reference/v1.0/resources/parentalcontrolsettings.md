---
title: Tipo de recurso parentalControlSettings
description: Especifica as configurações de controle parental de um aplicativo. Essas configurações controlam a experiência de consentimento.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 1f145ecabb4eccfe15eaedc856b1349fc6ce9f5a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128495"
---
# <a name="parentalcontrolsettings-resource-type"></a><span data-ttu-id="aadcd-104">Tipo de recurso parentalControlSettings</span><span class="sxs-lookup"><span data-stu-id="aadcd-104">parentalControlSettings resource type</span></span>

<span data-ttu-id="aadcd-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aadcd-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="aadcd-106">Especifica as configurações de controle parental de um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="aadcd-106">Specifies parental control settings for an application.</span></span> <span data-ttu-id="aadcd-107">Essas configurações controlam a experiência de consentimento.</span><span class="sxs-lookup"><span data-stu-id="aadcd-107">These settings control the consent experience.</span></span>

## <a name="properties"></a><span data-ttu-id="aadcd-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="aadcd-108">Properties</span></span>

| <span data-ttu-id="aadcd-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aadcd-109">Property</span></span> | <span data-ttu-id="aadcd-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="aadcd-110">Type</span></span> | <span data-ttu-id="aadcd-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="aadcd-111">Description</span></span> |
:---------------|:--------|:----------|
|<span data-ttu-id="aadcd-112">countriesBlockedForMinors</span><span class="sxs-lookup"><span data-stu-id="aadcd-112">countriesBlockedForMinors</span></span>|<span data-ttu-id="aadcd-113">String collection</span><span class="sxs-lookup"><span data-stu-id="aadcd-113">String collection</span></span>| <span data-ttu-id="aadcd-114">Especifica os códigos [de país ISO de](https://www.iso.org/iso-3166-country-codes.html)duas letras.</span><span class="sxs-lookup"><span data-stu-id="aadcd-114">Specifies the [two-letter ISO country codes](https://www.iso.org/iso-3166-country-codes.html).</span></span> <span data-ttu-id="aadcd-115">O acesso ao aplicativo será bloqueado para menores dos países especificados nesta lista.</span><span class="sxs-lookup"><span data-stu-id="aadcd-115">Access to the application will be blocked for minors from the countries specified in this list.</span></span>|
|<span data-ttu-id="aadcd-116">legalAgeGroupRule</span><span class="sxs-lookup"><span data-stu-id="aadcd-116">legalAgeGroupRule</span></span>| <span data-ttu-id="aadcd-117">String</span><span class="sxs-lookup"><span data-stu-id="aadcd-117">String</span></span> | <span data-ttu-id="aadcd-118">Especifica a regra de faixa etária legal que se aplica aos usuários do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="aadcd-118">Specifies the legal age group rule that applies to users of the app.</span></span> <span data-ttu-id="aadcd-119">Pode ser definido como um dos seguintes valores:</span><span class="sxs-lookup"><span data-stu-id="aadcd-119">Can be set to one of the following values:</span></span> <table><tr><th><span data-ttu-id="aadcd-120">Valor</span><span class="sxs-lookup"><span data-stu-id="aadcd-120">Value</span></span></th><th><span data-ttu-id="aadcd-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="aadcd-121">Description</span></span></th></tr><tr><td><span data-ttu-id="aadcd-122">Permitir</span><span class="sxs-lookup"><span data-stu-id="aadcd-122">Allow</span></span></td><td><span data-ttu-id="aadcd-123">Padrão.</span><span class="sxs-lookup"><span data-stu-id="aadcd-123">Default.</span></span> <span data-ttu-id="aadcd-124">Impõe o mínimo legal.</span><span class="sxs-lookup"><span data-stu-id="aadcd-124">Enforces the legal minimum.</span></span> <span data-ttu-id="aadcd-125">Isso significa que o consentimento dos pais é necessário para menores na União Europeia e na Coreia.</span><span class="sxs-lookup"><span data-stu-id="aadcd-125">This means parental consent is required for minors in the European Union and Korea.</span></span></td></tr><tr><td><span data-ttu-id="aadcd-126">RequireConsentForPrivacyServices</span><span class="sxs-lookup"><span data-stu-id="aadcd-126">RequireConsentForPrivacyServices</span></span></td><td><span data-ttu-id="aadcd-127">Impõe que o usuário especifique a data de nascimento para estar em conformidade com as regras do COPPA.</span><span class="sxs-lookup"><span data-stu-id="aadcd-127">Enforces the user to specify date of birth to comply with COPPA rules.</span></span> </td></tr><tr><td><span data-ttu-id="aadcd-128">RequireConsentForMinors</span><span class="sxs-lookup"><span data-stu-id="aadcd-128">RequireConsentForMinors</span></span></td><td><span data-ttu-id="aadcd-129">Requer o consentimento dos pais para menores de 18 anos, independentemente das regras secundárias do país.</span><span class="sxs-lookup"><span data-stu-id="aadcd-129">Requires parental consent for ages below 18, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="aadcd-130">RequireConsentForKids</span><span class="sxs-lookup"><span data-stu-id="aadcd-130">RequireConsentForKids</span></span></td><td><span data-ttu-id="aadcd-131">Requer o consentimento dos pais para menores de 14 anos, independentemente das regras secundárias do país.</span><span class="sxs-lookup"><span data-stu-id="aadcd-131">Requires parental consent for ages below 14, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="aadcd-132">BlockMinors</span><span class="sxs-lookup"><span data-stu-id="aadcd-132">BlockMinors</span></span></td><td><span data-ttu-id="aadcd-133">Impede que menores usem o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="aadcd-133">Blocks minors from using the app.</span></span></td></tr></table> |

## <a name="json-representation"></a><span data-ttu-id="aadcd-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="aadcd-134">JSON representation</span></span>
<span data-ttu-id="aadcd-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="aadcd-135">Here is a JSON representation of the resource.</span></span>

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

