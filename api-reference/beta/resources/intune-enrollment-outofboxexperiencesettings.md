---
title: tipo de recurso outOfBoxExperienceSettings
description: Configuração de experiência inicial da caixa
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 32336a0bc73c7d36ee4763dccbdc8a24197833ca
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999056"
---
# <a name="outofboxexperiencesettings-resource-type"></a><span data-ttu-id="3c3de-103">tipo de recurso outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="3c3de-103">outOfBoxExperienceSettings resource type</span></span>

> <span data-ttu-id="3c3de-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3c3de-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c3de-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3c3de-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c3de-106">Configuração de experiência inicial da caixa</span><span class="sxs-lookup"><span data-stu-id="3c3de-106">Out of box experience setting</span></span>

## <a name="properties"></a><span data-ttu-id="3c3de-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3c3de-107">Properties</span></span>
|<span data-ttu-id="3c3de-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3c3de-108">Property</span></span>|<span data-ttu-id="3c3de-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c3de-109">Type</span></span>|<span data-ttu-id="3c3de-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c3de-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c3de-111">hidePrivacySettings</span><span class="sxs-lookup"><span data-stu-id="3c3de-111">hidePrivacySettings</span></span>|<span data-ttu-id="3c3de-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="3c3de-112">Boolean</span></span>|<span data-ttu-id="3c3de-113">Mostrar ou ocultar as configurações de privacidade para o usuário</span><span class="sxs-lookup"><span data-stu-id="3c3de-113">Show or hide privacy settings to user</span></span>|
|<span data-ttu-id="3c3de-114">hideEULA</span><span class="sxs-lookup"><span data-stu-id="3c3de-114">hideEULA</span></span>|<span data-ttu-id="3c3de-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="3c3de-115">Boolean</span></span>|<span data-ttu-id="3c3de-116">Mostrar ou ocultar o EULA para o usuário</span><span class="sxs-lookup"><span data-stu-id="3c3de-116">Show or hide EULA to user</span></span>|
|<span data-ttu-id="3c3de-117">userType</span><span class="sxs-lookup"><span data-stu-id="3c3de-117">userType</span></span>|[<span data-ttu-id="3c3de-118">windowsUserType</span><span class="sxs-lookup"><span data-stu-id="3c3de-118">windowsUserType</span></span>](../resources/intune-enrollment-windowsusertype.md)|<span data-ttu-id="3c3de-119">Tipo de usuário.</span><span class="sxs-lookup"><span data-stu-id="3c3de-119">Type of user.</span></span> <span data-ttu-id="3c3de-120">Os valores possíveis são: `administrator` e `standard`.</span><span class="sxs-lookup"><span data-stu-id="3c3de-120">Possible values are: `administrator`, `standard`.</span></span>|
|<span data-ttu-id="3c3de-121">deviceUsageType</span><span class="sxs-lookup"><span data-stu-id="3c3de-121">deviceUsageType</span></span>|[<span data-ttu-id="3c3de-122">windowsDeviceUsageType</span><span class="sxs-lookup"><span data-stu-id="3c3de-122">windowsDeviceUsageType</span></span>](../resources/intune-enrollment-windowsdeviceusagetype.md)|<span data-ttu-id="3c3de-123">Tipo de autenticação do AAD join.</span><span class="sxs-lookup"><span data-stu-id="3c3de-123">AAD join authentication type.</span></span> <span data-ttu-id="3c3de-124">Os valores possíveis são: `singleUser` e `shared`.</span><span class="sxs-lookup"><span data-stu-id="3c3de-124">Possible values are: `singleUser`, `shared`.</span></span>|
|<span data-ttu-id="3c3de-125">skipKeyboardSelectionPage</span><span class="sxs-lookup"><span data-stu-id="3c3de-125">skipKeyboardSelectionPage</span></span>|<span data-ttu-id="3c3de-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="3c3de-126">Boolean</span></span>|<span data-ttu-id="3c3de-127">Se definido, ignore a página de seleção de teclado se idioma e região estiverem definidos</span><span class="sxs-lookup"><span data-stu-id="3c3de-127">If set, then skip the keyboard selection page if Language and Region are set</span></span>|
|<span data-ttu-id="3c3de-128">hideEscapeLink</span><span class="sxs-lookup"><span data-stu-id="3c3de-128">hideEscapeLink</span></span>|<span data-ttu-id="3c3de-129">Booliano</span><span class="sxs-lookup"><span data-stu-id="3c3de-129">Boolean</span></span>|<span data-ttu-id="3c3de-130">Se for definido como true, o usuário não poderá iniciar novamente com uma conta diferente, na entrada da empresa</span><span class="sxs-lookup"><span data-stu-id="3c3de-130">If set to true, then the user can't start over with different account, on company sign-in</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c3de-131">Relações</span><span class="sxs-lookup"><span data-stu-id="3c3de-131">Relationships</span></span>
<span data-ttu-id="3c3de-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3c3de-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3c3de-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3c3de-133">JSON Representation</span></span>
<span data-ttu-id="3c3de-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3c3de-134">Here is a JSON representation of the resource.</span></span>
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





