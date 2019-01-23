---
title: tipo de recurso de outOfBoxExperienceSettings
description: Configuração inicial pelo usuário configuração
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5d2b48fef00c9c3a291a0a2fdfe680b9f4e21030
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404600"
---
# <a name="outofboxexperiencesettings-resource-type"></a><span data-ttu-id="beff8-103">tipo de recurso de outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="beff8-103">outOfBoxExperienceSettings resource type</span></span>

> <span data-ttu-id="beff8-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="beff8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="beff8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="beff8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="beff8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="beff8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="beff8-107">Configuração inicial pelo usuário configuração</span><span class="sxs-lookup"><span data-stu-id="beff8-107">Out of box experience setting</span></span>

## <a name="properties"></a><span data-ttu-id="beff8-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="beff8-108">Properties</span></span>
|<span data-ttu-id="beff8-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="beff8-109">Property</span></span>|<span data-ttu-id="beff8-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="beff8-110">Type</span></span>|<span data-ttu-id="beff8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="beff8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="beff8-112">hidePrivacySettings</span><span class="sxs-lookup"><span data-stu-id="beff8-112">hidePrivacySettings</span></span>|<span data-ttu-id="beff8-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="beff8-113">Boolean</span></span>|<span data-ttu-id="beff8-114">Mostrar ou ocultar as configurações de privacidade para o usuário</span><span class="sxs-lookup"><span data-stu-id="beff8-114">Show or hide privacy settings to user</span></span>|
|<span data-ttu-id="beff8-115">hideEULA</span><span class="sxs-lookup"><span data-stu-id="beff8-115">hideEULA</span></span>|<span data-ttu-id="beff8-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="beff8-116">Boolean</span></span>|<span data-ttu-id="beff8-117">Mostrar ou ocultar o EULA ao usuário</span><span class="sxs-lookup"><span data-stu-id="beff8-117">Show or hide EULA to user</span></span>|
|<span data-ttu-id="beff8-118">userType</span><span class="sxs-lookup"><span data-stu-id="beff8-118">userType</span></span>|[<span data-ttu-id="beff8-119">windowsUserType</span><span class="sxs-lookup"><span data-stu-id="beff8-119">windowsUserType</span></span>](../resources/intune-enrollment-windowsusertype.md)|<span data-ttu-id="beff8-120">Tipo de usuário.</span><span class="sxs-lookup"><span data-stu-id="beff8-120">Type of user.</span></span> <span data-ttu-id="beff8-121">Os valores possíveis são: `administrator` e `standard`.</span><span class="sxs-lookup"><span data-stu-id="beff8-121">Possible values are: `administrator`, `standard`.</span></span>|
|<span data-ttu-id="beff8-122">deviceUsageType</span><span class="sxs-lookup"><span data-stu-id="beff8-122">deviceUsageType</span></span>|[<span data-ttu-id="beff8-123">windowsDeviceUsageType</span><span class="sxs-lookup"><span data-stu-id="beff8-123">windowsDeviceUsageType</span></span>](../resources/intune-enrollment-windowsdeviceusagetype.md)|<span data-ttu-id="beff8-124">Tipo de autenticação de ingresso AAD.</span><span class="sxs-lookup"><span data-stu-id="beff8-124">AAD join authentication type.</span></span> <span data-ttu-id="beff8-125">Os valores possíveis são: `singleUser` e `shared`.</span><span class="sxs-lookup"><span data-stu-id="beff8-125">Possible values are: `singleUser`, `shared`.</span></span>|
|<span data-ttu-id="beff8-126">skipKeyboardSelectionPage</span><span class="sxs-lookup"><span data-stu-id="beff8-126">skipKeyboardSelectionPage</span></span>|<span data-ttu-id="beff8-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="beff8-127">Boolean</span></span>|<span data-ttu-id="beff8-128">Se definido, em seguida, ignore a seleção de teclado página se estiver definida região e idioma</span><span class="sxs-lookup"><span data-stu-id="beff8-128">If set, then skip the keyboard selection page if Language and Region are set</span></span>|
|<span data-ttu-id="beff8-129">hideEscapeLink</span><span class="sxs-lookup"><span data-stu-id="beff8-129">hideEscapeLink</span></span>|<span data-ttu-id="beff8-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="beff8-130">Boolean</span></span>|<span data-ttu-id="beff8-131">Se definido como verdadeiro, em seguida, o usuário não pode começar novamente com uma conta diferente, na empresa entrar</span><span class="sxs-lookup"><span data-stu-id="beff8-131">If set to true, then the user can't start over with different account, on company sign-in</span></span>|

## <a name="relationships"></a><span data-ttu-id="beff8-132">Relações</span><span class="sxs-lookup"><span data-stu-id="beff8-132">Relationships</span></span>
<span data-ttu-id="beff8-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="beff8-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="beff8-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="beff8-134">JSON Representation</span></span>
<span data-ttu-id="beff8-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="beff8-135">Here is a JSON representation of the resource.</span></span>
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




