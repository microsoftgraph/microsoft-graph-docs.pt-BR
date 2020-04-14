---
title: tipo de recurso outOfBoxExperienceSettings
description: Configuração de experiência inicial da caixa
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 82bfd9a7126298958d35ad121b22115bb1f71241
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43460704"
---
# <a name="outofboxexperiencesettings-resource-type"></a><span data-ttu-id="46c43-103">tipo de recurso outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="46c43-103">outOfBoxExperienceSettings resource type</span></span>

<span data-ttu-id="46c43-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46c43-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="46c43-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="46c43-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46c43-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="46c43-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46c43-107">Configuração de experiência inicial da caixa</span><span class="sxs-lookup"><span data-stu-id="46c43-107">Out of box experience setting</span></span>

## <a name="properties"></a><span data-ttu-id="46c43-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="46c43-108">Properties</span></span>
|<span data-ttu-id="46c43-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="46c43-109">Property</span></span>|<span data-ttu-id="46c43-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="46c43-110">Type</span></span>|<span data-ttu-id="46c43-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="46c43-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46c43-112">hidePrivacySettings</span><span class="sxs-lookup"><span data-stu-id="46c43-112">hidePrivacySettings</span></span>|<span data-ttu-id="46c43-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="46c43-113">Boolean</span></span>|<span data-ttu-id="46c43-114">Mostrar ou ocultar as configurações de privacidade para o usuário</span><span class="sxs-lookup"><span data-stu-id="46c43-114">Show or hide privacy settings to user</span></span>|
|<span data-ttu-id="46c43-115">hideEULA</span><span class="sxs-lookup"><span data-stu-id="46c43-115">hideEULA</span></span>|<span data-ttu-id="46c43-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="46c43-116">Boolean</span></span>|<span data-ttu-id="46c43-117">Mostrar ou ocultar o EULA para o usuário</span><span class="sxs-lookup"><span data-stu-id="46c43-117">Show or hide EULA to user</span></span>|
|<span data-ttu-id="46c43-118">userType</span><span class="sxs-lookup"><span data-stu-id="46c43-118">userType</span></span>|[<span data-ttu-id="46c43-119">windowsUserType</span><span class="sxs-lookup"><span data-stu-id="46c43-119">windowsUserType</span></span>](../resources/intune-enrollment-windowsusertype.md)|<span data-ttu-id="46c43-120">Tipo de usuário.</span><span class="sxs-lookup"><span data-stu-id="46c43-120">Type of user.</span></span> <span data-ttu-id="46c43-121">Os valores possíveis são: `administrator` e `standard`.</span><span class="sxs-lookup"><span data-stu-id="46c43-121">Possible values are: `administrator`, `standard`.</span></span>|
|<span data-ttu-id="46c43-122">deviceUsageType</span><span class="sxs-lookup"><span data-stu-id="46c43-122">deviceUsageType</span></span>|[<span data-ttu-id="46c43-123">windowsDeviceUsageType</span><span class="sxs-lookup"><span data-stu-id="46c43-123">windowsDeviceUsageType</span></span>](../resources/intune-enrollment-windowsdeviceusagetype.md)|<span data-ttu-id="46c43-124">Tipo de autenticação do AAD join.</span><span class="sxs-lookup"><span data-stu-id="46c43-124">AAD join authentication type.</span></span> <span data-ttu-id="46c43-125">Os valores possíveis são: `singleUser` e `shared`.</span><span class="sxs-lookup"><span data-stu-id="46c43-125">Possible values are: `singleUser`, `shared`.</span></span>|
|<span data-ttu-id="46c43-126">skipKeyboardSelectionPage</span><span class="sxs-lookup"><span data-stu-id="46c43-126">skipKeyboardSelectionPage</span></span>|<span data-ttu-id="46c43-127">Booliano</span><span class="sxs-lookup"><span data-stu-id="46c43-127">Boolean</span></span>|<span data-ttu-id="46c43-128">Se definido, ignore a página de seleção de teclado se idioma e região estiverem definidos</span><span class="sxs-lookup"><span data-stu-id="46c43-128">If set, then skip the keyboard selection page if Language and Region are set</span></span>|
|<span data-ttu-id="46c43-129">hideEscapeLink</span><span class="sxs-lookup"><span data-stu-id="46c43-129">hideEscapeLink</span></span>|<span data-ttu-id="46c43-130">Booliano</span><span class="sxs-lookup"><span data-stu-id="46c43-130">Boolean</span></span>|<span data-ttu-id="46c43-131">Se for definido como true, o usuário não poderá iniciar novamente com uma conta diferente, na entrada da empresa</span><span class="sxs-lookup"><span data-stu-id="46c43-131">If set to true, then the user can't start over with different account, on company sign-in</span></span>|

## <a name="relationships"></a><span data-ttu-id="46c43-132">Relações</span><span class="sxs-lookup"><span data-stu-id="46c43-132">Relationships</span></span>
<span data-ttu-id="46c43-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="46c43-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="46c43-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="46c43-134">JSON Representation</span></span>
<span data-ttu-id="46c43-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="46c43-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.outOfBoxExperienceSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.outOfBoxExperienceSettings",
  "hidePrivacySettings": true,
  "hideEULA": true,
  "userType": "String",
  "deviceUsageType": "String",
  "skipKeyboardSelectionPage": true,
  "hideEscapeLink": true
}
```



