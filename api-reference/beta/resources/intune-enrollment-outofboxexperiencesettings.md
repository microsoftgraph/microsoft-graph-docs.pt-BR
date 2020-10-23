---
title: tipo de recurso outOfBoxExperienceSettings
description: Configuração de experiência inicial da caixa
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: df7137bfa4405e32887b1aa738d3b816ac3edf4a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728936"
---
# <a name="outofboxexperiencesettings-resource-type"></a><span data-ttu-id="08bde-103">tipo de recurso outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="08bde-103">outOfBoxExperienceSettings resource type</span></span>

<span data-ttu-id="08bde-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08bde-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="08bde-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="08bde-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08bde-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="08bde-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08bde-107">Configuração de experiência inicial da caixa</span><span class="sxs-lookup"><span data-stu-id="08bde-107">Out of box experience setting</span></span>

## <a name="properties"></a><span data-ttu-id="08bde-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="08bde-108">Properties</span></span>
|<span data-ttu-id="08bde-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="08bde-109">Property</span></span>|<span data-ttu-id="08bde-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="08bde-110">Type</span></span>|<span data-ttu-id="08bde-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="08bde-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08bde-112">hidePrivacySettings</span><span class="sxs-lookup"><span data-stu-id="08bde-112">hidePrivacySettings</span></span>|<span data-ttu-id="08bde-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="08bde-113">Boolean</span></span>|<span data-ttu-id="08bde-114">Mostrar ou ocultar as configurações de privacidade para o usuário</span><span class="sxs-lookup"><span data-stu-id="08bde-114">Show or hide privacy settings to user</span></span>|
|<span data-ttu-id="08bde-115">hideEULA</span><span class="sxs-lookup"><span data-stu-id="08bde-115">hideEULA</span></span>|<span data-ttu-id="08bde-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="08bde-116">Boolean</span></span>|<span data-ttu-id="08bde-117">Mostrar ou ocultar o EULA para o usuário</span><span class="sxs-lookup"><span data-stu-id="08bde-117">Show or hide EULA to user</span></span>|
|<span data-ttu-id="08bde-118">userType</span><span class="sxs-lookup"><span data-stu-id="08bde-118">userType</span></span>|[<span data-ttu-id="08bde-119">windowsUserType</span><span class="sxs-lookup"><span data-stu-id="08bde-119">windowsUserType</span></span>](../resources/intune-enrollment-windowsusertype.md)|<span data-ttu-id="08bde-120">Tipo de usuário.</span><span class="sxs-lookup"><span data-stu-id="08bde-120">Type of user.</span></span> <span data-ttu-id="08bde-121">Os valores possíveis são: `administrator` e `standard`.</span><span class="sxs-lookup"><span data-stu-id="08bde-121">Possible values are: `administrator`, `standard`.</span></span>|
|<span data-ttu-id="08bde-122">deviceUsageType</span><span class="sxs-lookup"><span data-stu-id="08bde-122">deviceUsageType</span></span>|[<span data-ttu-id="08bde-123">windowsDeviceUsageType</span><span class="sxs-lookup"><span data-stu-id="08bde-123">windowsDeviceUsageType</span></span>](../resources/intune-enrollment-windowsdeviceusagetype.md)|<span data-ttu-id="08bde-124">Tipo de autenticação do AAD join.</span><span class="sxs-lookup"><span data-stu-id="08bde-124">AAD join authentication type.</span></span> <span data-ttu-id="08bde-125">Os valores possíveis são: `singleUser` e `shared`.</span><span class="sxs-lookup"><span data-stu-id="08bde-125">Possible values are: `singleUser`, `shared`.</span></span>|
|<span data-ttu-id="08bde-126">skipKeyboardSelectionPage</span><span class="sxs-lookup"><span data-stu-id="08bde-126">skipKeyboardSelectionPage</span></span>|<span data-ttu-id="08bde-127">Booliano</span><span class="sxs-lookup"><span data-stu-id="08bde-127">Boolean</span></span>|<span data-ttu-id="08bde-128">Se definido, ignore a página de seleção de teclado se idioma e região estiverem definidos</span><span class="sxs-lookup"><span data-stu-id="08bde-128">If set, then skip the keyboard selection page if Language and Region are set</span></span>|
|<span data-ttu-id="08bde-129">hideEscapeLink</span><span class="sxs-lookup"><span data-stu-id="08bde-129">hideEscapeLink</span></span>|<span data-ttu-id="08bde-130">Booliano</span><span class="sxs-lookup"><span data-stu-id="08bde-130">Boolean</span></span>|<span data-ttu-id="08bde-131">Se for definido como true, o usuário não poderá iniciar novamente com uma conta diferente, na entrada da empresa</span><span class="sxs-lookup"><span data-stu-id="08bde-131">If set to true, then the user can't start over with different account, on company sign-in</span></span>|

## <a name="relationships"></a><span data-ttu-id="08bde-132">Relações</span><span class="sxs-lookup"><span data-stu-id="08bde-132">Relationships</span></span>
<span data-ttu-id="08bde-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="08bde-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="08bde-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="08bde-134">JSON Representation</span></span>
<span data-ttu-id="08bde-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="08bde-135">Here is a JSON representation of the resource.</span></span>
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





