---
title: tipo de recurso de outOfBoxExperienceSettings
description: Configuração inicial pelo usuário configuração
ms.openlocfilehash: 7d685c7e229828309e2ee759396215c3cd8dfac9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040530"
---
# <a name="outofboxexperiencesettings-resource-type"></a><span data-ttu-id="fd5c1-103">tipo de recurso de outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="fd5c1-103">outOfBoxExperienceSettings resource type</span></span>

> <span data-ttu-id="fd5c1-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fd5c1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fd5c1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fd5c1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fd5c1-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="fd5c1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fd5c1-107">Configuração inicial pelo usuário configuração</span><span class="sxs-lookup"><span data-stu-id="fd5c1-107">Out of box experience setting</span></span>
## <a name="properties"></a><span data-ttu-id="fd5c1-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fd5c1-108">Properties</span></span>
|<span data-ttu-id="fd5c1-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fd5c1-109">Property</span></span>|<span data-ttu-id="fd5c1-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="fd5c1-110">Type</span></span>|<span data-ttu-id="fd5c1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd5c1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd5c1-112">hidePrivacySettings</span><span class="sxs-lookup"><span data-stu-id="fd5c1-112">hidePrivacySettings</span></span>|<span data-ttu-id="fd5c1-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="fd5c1-113">Boolean</span></span>|<span data-ttu-id="fd5c1-114">Mostrar ou ocultar as configurações de privacidade para o usuário</span><span class="sxs-lookup"><span data-stu-id="fd5c1-114">Show or hide privacy settings to user</span></span>|
|<span data-ttu-id="fd5c1-115">hideEULA</span><span class="sxs-lookup"><span data-stu-id="fd5c1-115">hideEULA</span></span>|<span data-ttu-id="fd5c1-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="fd5c1-116">Boolean</span></span>|<span data-ttu-id="fd5c1-117">Mostrar ou ocultar o EULA ao usuário</span><span class="sxs-lookup"><span data-stu-id="fd5c1-117">Show or hide EULA to user</span></span>|
|<span data-ttu-id="fd5c1-118">userType</span><span class="sxs-lookup"><span data-stu-id="fd5c1-118">userType</span></span>|[<span data-ttu-id="fd5c1-119">windowsUserType</span><span class="sxs-lookup"><span data-stu-id="fd5c1-119">windowsUserType</span></span>](../resources/intune-enrollment-windowsusertype.md)|<span data-ttu-id="fd5c1-120">Tipo de usuário.</span><span class="sxs-lookup"><span data-stu-id="fd5c1-120">Type of user.</span></span> <span data-ttu-id="fd5c1-121">Os valores possíveis são: `administrator` e `standard`.</span><span class="sxs-lookup"><span data-stu-id="fd5c1-121">Possible values are: `administrator`, `standard`.</span></span>|
|<span data-ttu-id="fd5c1-122">deviceUsageType</span><span class="sxs-lookup"><span data-stu-id="fd5c1-122">deviceUsageType</span></span>|[<span data-ttu-id="fd5c1-123">windowsDeviceUsageType</span><span class="sxs-lookup"><span data-stu-id="fd5c1-123">windowsDeviceUsageType</span></span>](../resources/intune-enrollment-windowsdeviceusagetype.md)|<span data-ttu-id="fd5c1-124">Tipo de autenticação de ingresso AAD.</span><span class="sxs-lookup"><span data-stu-id="fd5c1-124">AAD join authentication type.</span></span> <span data-ttu-id="fd5c1-125">Os valores possíveis são: `singleUser` e `shared`.</span><span class="sxs-lookup"><span data-stu-id="fd5c1-125">Possible values are: `singleUser`, `shared`.</span></span>|
|<span data-ttu-id="fd5c1-126">skipKeyboardSelectionPage</span><span class="sxs-lookup"><span data-stu-id="fd5c1-126">skipKeyboardSelectionPage</span></span>|<span data-ttu-id="fd5c1-127">Booliano</span><span class="sxs-lookup"><span data-stu-id="fd5c1-127">Boolean</span></span>|<span data-ttu-id="fd5c1-128">Se definido, em seguida, ignore a seleção de teclado página se estiver definida região e idioma</span><span class="sxs-lookup"><span data-stu-id="fd5c1-128">If set, then skip the keyboard selection page if Language and Region are set</span></span>|
|<span data-ttu-id="fd5c1-129">hideEscapeLink</span><span class="sxs-lookup"><span data-stu-id="fd5c1-129">hideEscapeLink</span></span>|<span data-ttu-id="fd5c1-130">Booliano</span><span class="sxs-lookup"><span data-stu-id="fd5c1-130">Boolean</span></span>|<span data-ttu-id="fd5c1-131">Se definido como verdadeiro, em seguida, o usuário não pode começar novamente com uma conta diferente, na empresa entrar</span><span class="sxs-lookup"><span data-stu-id="fd5c1-131">If set to true, then the user can't start over with different account, on company sign-in</span></span>|

## <a name="relationships"></a><span data-ttu-id="fd5c1-132">Relações</span><span class="sxs-lookup"><span data-stu-id="fd5c1-132">Relationships</span></span>
<span data-ttu-id="fd5c1-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fd5c1-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fd5c1-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fd5c1-134">JSON Representation</span></span>
<span data-ttu-id="fd5c1-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fd5c1-135">Here is a JSON representation of the resource.</span></span>
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





