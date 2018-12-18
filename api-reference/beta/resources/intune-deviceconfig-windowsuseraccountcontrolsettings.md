---
title: tipo de enum windowsUserAccountControlSettings
description: Valores possíveis para configurações de controle de conta de usuário do Windows.
author: tfitzmac
ms.openlocfilehash: dcec2ca6e5b6401b5277e513867c0646bff79c21
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320297"
---
# <a name="windowsuseraccountcontrolsettings-enum-type"></a><span data-ttu-id="54674-103">tipo de enum windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="54674-103">windowsUserAccountControlSettings enum type</span></span>

> <span data-ttu-id="54674-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="54674-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="54674-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="54674-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="54674-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="54674-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="54674-107">Valores possíveis para configurações de controle de conta de usuário do Windows.</span><span class="sxs-lookup"><span data-stu-id="54674-107">Possible values for Windows user account control settings.</span></span>
## <a name="members"></a><span data-ttu-id="54674-108">Membros</span><span class="sxs-lookup"><span data-stu-id="54674-108">Members</span></span>
|<span data-ttu-id="54674-109">Membro</span><span class="sxs-lookup"><span data-stu-id="54674-109">Member</span></span>|<span data-ttu-id="54674-110">Valor</span><span class="sxs-lookup"><span data-stu-id="54674-110">Value</span></span>|<span data-ttu-id="54674-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="54674-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54674-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="54674-112">userDefined</span></span>|<span data-ttu-id="54674-113">0</span><span class="sxs-lookup"><span data-stu-id="54674-113">0</span></span>|<span data-ttu-id="54674-114">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="54674-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="54674-115">alwaysNotify</span><span class="sxs-lookup"><span data-stu-id="54674-115">alwaysNotify</span></span>|<span data-ttu-id="54674-116">1</span><span class="sxs-lookup"><span data-stu-id="54674-116">1</span></span>|<span data-ttu-id="54674-117">Sempre notifica.</span><span class="sxs-lookup"><span data-stu-id="54674-117">Always notify.</span></span>|
|<span data-ttu-id="54674-118">notifyOnAppChanges</span><span class="sxs-lookup"><span data-stu-id="54674-118">notifyOnAppChanges</span></span>|<span data-ttu-id="54674-119">2</span><span class="sxs-lookup"><span data-stu-id="54674-119">2</span></span>|<span data-ttu-id="54674-120">Notifica sobre alterações de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="54674-120">Notify on app changes.</span></span>|
|<span data-ttu-id="54674-121">notifyOnAppChangesWithoutDimming</span><span class="sxs-lookup"><span data-stu-id="54674-121">notifyOnAppChangesWithoutDimming</span></span>|<span data-ttu-id="54674-122">3</span><span class="sxs-lookup"><span data-stu-id="54674-122">3</span></span>|<span data-ttu-id="54674-123">Notifica sobre mudanças de app sem escurecer a área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="54674-123">Notify on app changes without dimming desktop.</span></span>|
|<span data-ttu-id="54674-124">neverNotify</span><span class="sxs-lookup"><span data-stu-id="54674-124">neverNotify</span></span>|<span data-ttu-id="54674-125">4</span><span class="sxs-lookup"><span data-stu-id="54674-125">4</span></span>|<span data-ttu-id="54674-126">Nunca notifica.</span><span class="sxs-lookup"><span data-stu-id="54674-126">Never notify.</span></span>|





