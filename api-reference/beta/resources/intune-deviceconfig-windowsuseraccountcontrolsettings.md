---
title: tipo de enum windowsUserAccountControlSettings
description: Valores possíveis para configurações de controle de conta de usuário do Windows.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cd16db4236096687ddcc9f169dd657c938fd6815
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911809"
---
# <a name="windowsuseraccountcontrolsettings-enum-type"></a><span data-ttu-id="8e449-103">tipo de enum windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="8e449-103">windowsUserAccountControlSettings enum type</span></span>

> <span data-ttu-id="8e449-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8e449-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8e449-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8e449-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8e449-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8e449-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8e449-107">Valores possíveis para configurações de controle de conta de usuário do Windows.</span><span class="sxs-lookup"><span data-stu-id="8e449-107">Possible values for Windows user account control settings.</span></span>
## <a name="members"></a><span data-ttu-id="8e449-108">Membros</span><span class="sxs-lookup"><span data-stu-id="8e449-108">Members</span></span>
|<span data-ttu-id="8e449-109">Membro</span><span class="sxs-lookup"><span data-stu-id="8e449-109">Member</span></span>|<span data-ttu-id="8e449-110">Valor</span><span class="sxs-lookup"><span data-stu-id="8e449-110">Value</span></span>|<span data-ttu-id="8e449-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e449-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e449-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="8e449-112">userDefined</span></span>|<span data-ttu-id="8e449-113">0</span><span class="sxs-lookup"><span data-stu-id="8e449-113">0</span></span>|<span data-ttu-id="8e449-114">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="8e449-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="8e449-115">alwaysNotify</span><span class="sxs-lookup"><span data-stu-id="8e449-115">alwaysNotify</span></span>|<span data-ttu-id="8e449-116">1</span><span class="sxs-lookup"><span data-stu-id="8e449-116">1</span></span>|<span data-ttu-id="8e449-117">Sempre notifica.</span><span class="sxs-lookup"><span data-stu-id="8e449-117">Always notify.</span></span>|
|<span data-ttu-id="8e449-118">notifyOnAppChanges</span><span class="sxs-lookup"><span data-stu-id="8e449-118">notifyOnAppChanges</span></span>|<span data-ttu-id="8e449-119">2</span><span class="sxs-lookup"><span data-stu-id="8e449-119">2</span></span>|<span data-ttu-id="8e449-120">Notifica sobre alterações de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8e449-120">Notify on app changes.</span></span>|
|<span data-ttu-id="8e449-121">notifyOnAppChangesWithoutDimming</span><span class="sxs-lookup"><span data-stu-id="8e449-121">notifyOnAppChangesWithoutDimming</span></span>|<span data-ttu-id="8e449-122">3</span><span class="sxs-lookup"><span data-stu-id="8e449-122">3</span></span>|<span data-ttu-id="8e449-123">Notifica sobre mudanças de app sem escurecer a área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="8e449-123">Notify on app changes without dimming desktop.</span></span>|
|<span data-ttu-id="8e449-124">neverNotify</span><span class="sxs-lookup"><span data-stu-id="8e449-124">neverNotify</span></span>|<span data-ttu-id="8e449-125">4</span><span class="sxs-lookup"><span data-stu-id="8e449-125">4</span></span>|<span data-ttu-id="8e449-126">Nunca notifica.</span><span class="sxs-lookup"><span data-stu-id="8e449-126">Never notify.</span></span>|





