---
title: tipo de recurso de outOfBoxExperienceSettings
description: Configuração inicial pelo usuário configuração
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: af276dd520df9ee3b257650e703813de355bed9a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882730"
---
# <a name="outofboxexperiencesettings-resource-type"></a><span data-ttu-id="fef7d-103">tipo de recurso de outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="fef7d-103">outOfBoxExperienceSettings resource type</span></span>

> <span data-ttu-id="fef7d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fef7d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fef7d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fef7d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fef7d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="fef7d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fef7d-107">Configuração inicial pelo usuário configuração</span><span class="sxs-lookup"><span data-stu-id="fef7d-107">Out of box experience setting</span></span>
## <a name="properties"></a><span data-ttu-id="fef7d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fef7d-108">Properties</span></span>
|<span data-ttu-id="fef7d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fef7d-109">Property</span></span>|<span data-ttu-id="fef7d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="fef7d-110">Type</span></span>|<span data-ttu-id="fef7d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="fef7d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fef7d-112">hidePrivacySettings</span><span class="sxs-lookup"><span data-stu-id="fef7d-112">hidePrivacySettings</span></span>|<span data-ttu-id="fef7d-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="fef7d-113">Boolean</span></span>|<span data-ttu-id="fef7d-114">Mostrar ou ocultar as configurações de privacidade para o usuário</span><span class="sxs-lookup"><span data-stu-id="fef7d-114">Show or hide privacy settings to user</span></span>|
|<span data-ttu-id="fef7d-115">hideEULA</span><span class="sxs-lookup"><span data-stu-id="fef7d-115">hideEULA</span></span>|<span data-ttu-id="fef7d-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="fef7d-116">Boolean</span></span>|<span data-ttu-id="fef7d-117">Mostrar ou ocultar o EULA ao usuário</span><span class="sxs-lookup"><span data-stu-id="fef7d-117">Show or hide EULA to user</span></span>|
|<span data-ttu-id="fef7d-118">userType</span><span class="sxs-lookup"><span data-stu-id="fef7d-118">userType</span></span>|[<span data-ttu-id="fef7d-119">windowsUserType</span><span class="sxs-lookup"><span data-stu-id="fef7d-119">windowsUserType</span></span>](../resources/intune-enrollment-windowsusertype.md)|<span data-ttu-id="fef7d-120">Tipo de usuário.</span><span class="sxs-lookup"><span data-stu-id="fef7d-120">Type of user.</span></span> <span data-ttu-id="fef7d-121">Os valores possíveis são: `administrator` e `standard`.</span><span class="sxs-lookup"><span data-stu-id="fef7d-121">Possible values are: `administrator`, `standard`.</span></span>|
|<span data-ttu-id="fef7d-122">deviceUsageType</span><span class="sxs-lookup"><span data-stu-id="fef7d-122">deviceUsageType</span></span>|[<span data-ttu-id="fef7d-123">windowsDeviceUsageType</span><span class="sxs-lookup"><span data-stu-id="fef7d-123">windowsDeviceUsageType</span></span>](../resources/intune-enrollment-windowsdeviceusagetype.md)|<span data-ttu-id="fef7d-124">Tipo de autenticação de ingresso AAD.</span><span class="sxs-lookup"><span data-stu-id="fef7d-124">AAD join authentication type.</span></span> <span data-ttu-id="fef7d-125">Os valores possíveis são: `singleUser` e `shared`.</span><span class="sxs-lookup"><span data-stu-id="fef7d-125">Possible values are: `singleUser`, `shared`.</span></span>|
|<span data-ttu-id="fef7d-126">skipKeyboardSelectionPage</span><span class="sxs-lookup"><span data-stu-id="fef7d-126">skipKeyboardSelectionPage</span></span>|<span data-ttu-id="fef7d-127">Booliano</span><span class="sxs-lookup"><span data-stu-id="fef7d-127">Boolean</span></span>|<span data-ttu-id="fef7d-128">Se definido, em seguida, ignore a seleção de teclado página se estiver definida região e idioma</span><span class="sxs-lookup"><span data-stu-id="fef7d-128">If set, then skip the keyboard selection page if Language and Region are set</span></span>|
|<span data-ttu-id="fef7d-129">hideEscapeLink</span><span class="sxs-lookup"><span data-stu-id="fef7d-129">hideEscapeLink</span></span>|<span data-ttu-id="fef7d-130">Booliano</span><span class="sxs-lookup"><span data-stu-id="fef7d-130">Boolean</span></span>|<span data-ttu-id="fef7d-131">Se definido como verdadeiro, em seguida, o usuário não pode começar novamente com uma conta diferente, na empresa entrar</span><span class="sxs-lookup"><span data-stu-id="fef7d-131">If set to true, then the user can't start over with different account, on company sign-in</span></span>|

## <a name="relationships"></a><span data-ttu-id="fef7d-132">Relações</span><span class="sxs-lookup"><span data-stu-id="fef7d-132">Relationships</span></span>
<span data-ttu-id="fef7d-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fef7d-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fef7d-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fef7d-134">JSON Representation</span></span>
<span data-ttu-id="fef7d-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fef7d-135">Here is a JSON representation of the resource.</span></span>
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





