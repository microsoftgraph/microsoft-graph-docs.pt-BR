---
title: tipo de recurso de parentalControlSettings
description: Especifica as configurações de controle do responsável para um aplicativo. Essas configurações controlam a experiência de consentimento.
localization_priority: Normal
ms.openlocfilehash: 52a808cd4c3e6f29e4d43c7c4ea5c9e30a81447b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528400"
---
# <a name="parentalcontrolsettings-resource-type"></a><span data-ttu-id="195d7-104">tipo de recurso de parentalControlSettings</span><span class="sxs-lookup"><span data-stu-id="195d7-104">parentalControlSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="195d7-105">Especifica as configurações de controle do responsável para um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="195d7-105">Specifies parental control settings for an application.</span></span> <span data-ttu-id="195d7-106">Essas configurações controlam a experiência de consentimento.</span><span class="sxs-lookup"><span data-stu-id="195d7-106">These settings control the consent experience.</span></span>

## <a name="properties"></a><span data-ttu-id="195d7-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="195d7-107">Properties</span></span>

| <span data-ttu-id="195d7-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="195d7-108">Property</span></span> | <span data-ttu-id="195d7-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="195d7-109">Type</span></span> | <span data-ttu-id="195d7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="195d7-110">Description</span></span> |
:---------------|:--------|:----------|
|<span data-ttu-id="195d7-111">countriesBlockedForMinors</span><span class="sxs-lookup"><span data-stu-id="195d7-111">countriesBlockedForMinors</span></span>|<span data-ttu-id="195d7-112">String collection</span><span class="sxs-lookup"><span data-stu-id="195d7-112">String collection</span></span>| <span data-ttu-id="195d7-113">Especifica os [códigos de país ISO de duas letras](https://www.iso.org/iso-3166-country-codes.html).</span><span class="sxs-lookup"><span data-stu-id="195d7-113">Specifies the [two-letter ISO country codes](https://www.iso.org/iso-3166-country-codes.html).</span></span> <span data-ttu-id="195d7-114">Acesso ao aplicativo será bloqueado para menores dos países especificados na lista.</span><span class="sxs-lookup"><span data-stu-id="195d7-114">Access to the application will be blocked for minors from the countries specified in this list.</span></span>|
|<span data-ttu-id="195d7-115">legalAgeGroupRule</span><span class="sxs-lookup"><span data-stu-id="195d7-115">legalAgeGroupRule</span></span>| <span data-ttu-id="195d7-116">String</span><span class="sxs-lookup"><span data-stu-id="195d7-116">String</span></span> | <span data-ttu-id="195d7-117">Especifica a regra de grupo de idade legais que se aplica a usuários do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="195d7-117">Specifies the legal age group rule that applies to users of the app.</span></span> <span data-ttu-id="195d7-118">Pode ser definido como um dos seguintes valores:</span><span class="sxs-lookup"><span data-stu-id="195d7-118">Can be set to one of the following values:</span></span> <table><tr><th><span data-ttu-id="195d7-119">Valor</span><span class="sxs-lookup"><span data-stu-id="195d7-119">Value</span></span></th><th><span data-ttu-id="195d7-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="195d7-120">Description</span></span></th></tr><tr><td><span data-ttu-id="195d7-121">Permitir</span><span class="sxs-lookup"><span data-stu-id="195d7-121">Allow</span></span></td><td><span data-ttu-id="195d7-122">Padrão.</span><span class="sxs-lookup"><span data-stu-id="195d7-122">Default.</span></span> <span data-ttu-id="195d7-123">Impõe o mínimo legal.</span><span class="sxs-lookup"><span data-stu-id="195d7-123">Enforces the legal minimum.</span></span> <span data-ttu-id="195d7-124">Isso significa que o consentimento dos pais é necessário para menores na União Europeia e Coreia.</span><span class="sxs-lookup"><span data-stu-id="195d7-124">This means parental consent is required for minors in the European Union and Korea.</span></span></td></tr><tr><td><span data-ttu-id="195d7-125">RequireConsentForPrivacyServices</span><span class="sxs-lookup"><span data-stu-id="195d7-125">RequireConsentForPrivacyServices</span></span></td><td><span data-ttu-id="195d7-126">Impõe o usuário para especificar a data de nascimento esteja em conformidade com as regras de COPPA.</span><span class="sxs-lookup"><span data-stu-id="195d7-126">Enforces the user to specify date of birth to comply with COPPA rules.</span></span> </td></tr><tr><td><span data-ttu-id="195d7-127">RequireConsentForMinors</span><span class="sxs-lookup"><span data-stu-id="195d7-127">RequireConsentForMinors</span></span></td><td><span data-ttu-id="195d7-128">Requer o consentimento dos pais para anos abaixo 18, independentemente das regras de país secundárias.</span><span class="sxs-lookup"><span data-stu-id="195d7-128">Requires parental consent for ages below 18, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="195d7-129">RequireConsentForKids</span><span class="sxs-lookup"><span data-stu-id="195d7-129">RequireConsentForKids</span></span></td><td><span data-ttu-id="195d7-130">Requer o consentimento dos pais para anos abaixo 14, independentemente das regras de país secundárias.</span><span class="sxs-lookup"><span data-stu-id="195d7-130">Requires parental consent for ages below 14, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="195d7-131">BlockMinors</span><span class="sxs-lookup"><span data-stu-id="195d7-131">BlockMinors</span></span></td><td><span data-ttu-id="195d7-132">Menores de blocos de usar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="195d7-132">Blocks minors from using the app.</span></span></td></tr></table> |

## <a name="json-representation"></a><span data-ttu-id="195d7-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="195d7-133">JSON representation</span></span>
<span data-ttu-id="195d7-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="195d7-134">Here is a JSON representation of the resource.</span></span>

```json
{
  "countriesBlockedForMinors": [ "String" ],
  "legalAgeGroupRule": "String"
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/parentalcontrolsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
