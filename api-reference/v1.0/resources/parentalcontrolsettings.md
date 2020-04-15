---
title: tipo de recurso parentalControlSettings
description: Especifica as configurações de controle parental de um aplicativo. Essas configurações controlam a experiência de consentimento.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 8e54b8b437eb7a287102e67234a4f9b692136b79
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43353686"
---
# <a name="parentalcontrolsettings-resource-type"></a><span data-ttu-id="ea102-104">tipo de recurso parentalControlSettings</span><span class="sxs-lookup"><span data-stu-id="ea102-104">parentalControlSettings resource type</span></span>

<span data-ttu-id="ea102-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea102-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ea102-106">Especifica as configurações de controle parental de um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ea102-106">Specifies parental control settings for an application.</span></span> <span data-ttu-id="ea102-107">Essas configurações controlam a experiência de consentimento.</span><span class="sxs-lookup"><span data-stu-id="ea102-107">These settings control the consent experience.</span></span>

## <a name="properties"></a><span data-ttu-id="ea102-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ea102-108">Properties</span></span>

| <span data-ttu-id="ea102-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ea102-109">Property</span></span> | <span data-ttu-id="ea102-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea102-110">Type</span></span> | <span data-ttu-id="ea102-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea102-111">Description</span></span> |
:---------------|:--------|:----------|
|<span data-ttu-id="ea102-112">countriesBlockedForMinors</span><span class="sxs-lookup"><span data-stu-id="ea102-112">countriesBlockedForMinors</span></span>|<span data-ttu-id="ea102-113">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ea102-113">String collection</span></span>| <span data-ttu-id="ea102-114">Especifica os [códigos de país ISO de duas letras](https://www.iso.org/iso-3166-country-codes.html).</span><span class="sxs-lookup"><span data-stu-id="ea102-114">Specifies the [two-letter ISO country codes](https://www.iso.org/iso-3166-country-codes.html).</span></span> <span data-ttu-id="ea102-115">O acesso ao aplicativo será bloqueado para menores dos países especificados nesta lista.</span><span class="sxs-lookup"><span data-stu-id="ea102-115">Access to the application will be blocked for minors from the countries specified in this list.</span></span>|
|<span data-ttu-id="ea102-116">legalAgeGroupRule</span><span class="sxs-lookup"><span data-stu-id="ea102-116">legalAgeGroupRule</span></span>| <span data-ttu-id="ea102-117">String</span><span class="sxs-lookup"><span data-stu-id="ea102-117">String</span></span> | <span data-ttu-id="ea102-118">Especifica a regra de grupo de idades legais que se aplica aos usuários do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ea102-118">Specifies the legal age group rule that applies to users of the app.</span></span> <span data-ttu-id="ea102-119">Pode ser definido como um dos seguintes valores:</span><span class="sxs-lookup"><span data-stu-id="ea102-119">Can be set to one of the following values:</span></span> <table><tr><th><span data-ttu-id="ea102-120">Valor</span><span class="sxs-lookup"><span data-stu-id="ea102-120">Value</span></span></th><th><span data-ttu-id="ea102-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea102-121">Description</span></span></th></tr><tr><td><span data-ttu-id="ea102-122">Permitir</span><span class="sxs-lookup"><span data-stu-id="ea102-122">Allow</span></span></td><td><span data-ttu-id="ea102-123">Padrão.</span><span class="sxs-lookup"><span data-stu-id="ea102-123">Default.</span></span> <span data-ttu-id="ea102-124">Impõe o mínimo legal.</span><span class="sxs-lookup"><span data-stu-id="ea102-124">Enforces the legal minimum.</span></span> <span data-ttu-id="ea102-125">Isso significa que o consentimento do responsável é obrigatório para menores na União Européia e na Coréia.</span><span class="sxs-lookup"><span data-stu-id="ea102-125">This means parental consent is required for minors in the European Union and Korea.</span></span></td></tr><tr><td><span data-ttu-id="ea102-126">RequireConsentForPrivacyServices</span><span class="sxs-lookup"><span data-stu-id="ea102-126">RequireConsentForPrivacyServices</span></span></td><td><span data-ttu-id="ea102-127">Impõe que o usuário especifique a data de nascimento para estar em conformidade com as regras do COOPA.</span><span class="sxs-lookup"><span data-stu-id="ea102-127">Enforces the user to specify date of birth to comply with COPPA rules.</span></span> </td></tr><tr><td><span data-ttu-id="ea102-128">RequireConsentForMinors</span><span class="sxs-lookup"><span data-stu-id="ea102-128">RequireConsentForMinors</span></span></td><td><span data-ttu-id="ea102-129">Requer o consentimento dos pais para crianças abaixo de 18, independentemente das regras secundárias do país.</span><span class="sxs-lookup"><span data-stu-id="ea102-129">Requires parental consent for ages below 18, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="ea102-130">RequireConsentForKids</span><span class="sxs-lookup"><span data-stu-id="ea102-130">RequireConsentForKids</span></span></td><td><span data-ttu-id="ea102-131">Requer o consentimento dos pais para crianças abaixo de 14, independentemente das regras secundárias do país.</span><span class="sxs-lookup"><span data-stu-id="ea102-131">Requires parental consent for ages below 14, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="ea102-132">BlockMinors</span><span class="sxs-lookup"><span data-stu-id="ea102-132">BlockMinors</span></span></td><td><span data-ttu-id="ea102-133">Bloqueia os menores de usar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ea102-133">Blocks minors from using the app.</span></span></td></tr></table> |

## <a name="json-representation"></a><span data-ttu-id="ea102-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ea102-134">JSON representation</span></span>
<span data-ttu-id="ea102-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ea102-135">Here is a JSON representation of the resource.</span></span>

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
