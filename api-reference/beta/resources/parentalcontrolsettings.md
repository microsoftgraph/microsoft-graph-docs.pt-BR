---
title: tipo de recurso parentalControlSettings
description: Especifica as configurações de controle parental de um aplicativo. Essas configurações controlam a experiência de consentimento.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 066182d0e591dc0a260313beafe75504b328a31b
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939001"
---
# <a name="parentalcontrolsettings-resource-type"></a><span data-ttu-id="e1d76-104">tipo de recurso parentalControlSettings</span><span class="sxs-lookup"><span data-stu-id="e1d76-104">parentalControlSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1d76-105">Especifica as configurações de controle parental de um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e1d76-105">Specifies parental control settings for an application.</span></span> <span data-ttu-id="e1d76-106">Essas configurações controlam a experiência de consentimento.</span><span class="sxs-lookup"><span data-stu-id="e1d76-106">These settings control the consent experience.</span></span>

## <a name="properties"></a><span data-ttu-id="e1d76-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e1d76-107">Properties</span></span>

| <span data-ttu-id="e1d76-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e1d76-108">Property</span></span> | <span data-ttu-id="e1d76-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1d76-109">Type</span></span> | <span data-ttu-id="e1d76-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1d76-110">Description</span></span> |
:---------------|:--------|:----------|
|<span data-ttu-id="e1d76-111">countriesBlockedForMinors</span><span class="sxs-lookup"><span data-stu-id="e1d76-111">countriesBlockedForMinors</span></span>|<span data-ttu-id="e1d76-112">String collection</span><span class="sxs-lookup"><span data-stu-id="e1d76-112">String collection</span></span>| <span data-ttu-id="e1d76-113">Especifica os [códigos de país ISO de duas letras](https://www.iso.org/iso-3166-country-codes.html).</span><span class="sxs-lookup"><span data-stu-id="e1d76-113">Specifies the [two-letter ISO country codes](https://www.iso.org/iso-3166-country-codes.html).</span></span> <span data-ttu-id="e1d76-114">O acesso ao aplicativo será bloqueado para menores dos países especificados nesta lista.</span><span class="sxs-lookup"><span data-stu-id="e1d76-114">Access to the application will be blocked for minors from the countries specified in this list.</span></span>|
|<span data-ttu-id="e1d76-115">legalAgeGroupRule</span><span class="sxs-lookup"><span data-stu-id="e1d76-115">legalAgeGroupRule</span></span>| <span data-ttu-id="e1d76-116">String</span><span class="sxs-lookup"><span data-stu-id="e1d76-116">String</span></span> | <span data-ttu-id="e1d76-117">Especifica a regra de grupo de idades legais que se aplica aos usuários do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e1d76-117">Specifies the legal age group rule that applies to users of the app.</span></span> <span data-ttu-id="e1d76-118">Pode ser definido como um dos seguintes valores:</span><span class="sxs-lookup"><span data-stu-id="e1d76-118">Can be set to one of the following values:</span></span> <table><tr><th><span data-ttu-id="e1d76-119">Valor</span><span class="sxs-lookup"><span data-stu-id="e1d76-119">Value</span></span></th><th><span data-ttu-id="e1d76-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1d76-120">Description</span></span></th></tr><tr><td><span data-ttu-id="e1d76-121">Permitir</span><span class="sxs-lookup"><span data-stu-id="e1d76-121">Allow</span></span></td><td><span data-ttu-id="e1d76-122">Padrão.</span><span class="sxs-lookup"><span data-stu-id="e1d76-122">Default.</span></span> <span data-ttu-id="e1d76-123">Impõe o mínimo legal.</span><span class="sxs-lookup"><span data-stu-id="e1d76-123">Enforces the legal minimum.</span></span> <span data-ttu-id="e1d76-124">Isso significa que o consentimento do responsável é obrigatório para menores na União Européia e na Coréia.</span><span class="sxs-lookup"><span data-stu-id="e1d76-124">This means parental consent is required for minors in the European Union and Korea.</span></span></td></tr><tr><td><span data-ttu-id="e1d76-125">RequireConsentForPrivacyServices</span><span class="sxs-lookup"><span data-stu-id="e1d76-125">RequireConsentForPrivacyServices</span></span></td><td><span data-ttu-id="e1d76-126">Impõe que o usuário especifique a data de nascimento para estar em conformidade com as regras do COOPA.</span><span class="sxs-lookup"><span data-stu-id="e1d76-126">Enforces the user to specify date of birth to comply with COPPA rules.</span></span> </td></tr><tr><td><span data-ttu-id="e1d76-127">RequireConsentForMinors</span><span class="sxs-lookup"><span data-stu-id="e1d76-127">RequireConsentForMinors</span></span></td><td><span data-ttu-id="e1d76-128">Requer o consentimento dos pais para crianças abaixo de 18, independentemente das regras secundárias do país.</span><span class="sxs-lookup"><span data-stu-id="e1d76-128">Requires parental consent for ages below 18, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="e1d76-129">RequireConsentForKids</span><span class="sxs-lookup"><span data-stu-id="e1d76-129">RequireConsentForKids</span></span></td><td><span data-ttu-id="e1d76-130">Requer o consentimento dos pais para crianças abaixo de 14, independentemente das regras secundárias do país.</span><span class="sxs-lookup"><span data-stu-id="e1d76-130">Requires parental consent for ages below 14, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="e1d76-131">BlockMinors</span><span class="sxs-lookup"><span data-stu-id="e1d76-131">BlockMinors</span></span></td><td><span data-ttu-id="e1d76-132">Bloqueia os menores de usar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e1d76-132">Blocks minors from using the app.</span></span></td></tr></table> |

## <a name="json-representation"></a><span data-ttu-id="e1d76-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e1d76-133">JSON representation</span></span>
<span data-ttu-id="e1d76-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e1d76-134">Here is a JSON representation of the resource.</span></span>

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
