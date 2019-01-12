---
title: tipo de enum windowsUserAccountControlSettings
description: Valores possíveis para configurações de controle de conta de usuário do Windows.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0475d8fb013cbb07f8d69a659f8ecde2eb580e43
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972471"
---
# <a name="windowsuseraccountcontrolsettings-enum-type"></a><span data-ttu-id="c943b-103">tipo de enum windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="c943b-103">windowsUserAccountControlSettings enum type</span></span>

> <span data-ttu-id="c943b-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c943b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c943b-105">Valores possíveis para configurações de controle de conta de usuário do Windows.</span><span class="sxs-lookup"><span data-stu-id="c943b-105">Possible values for Windows user account control settings.</span></span>
## <a name="members"></a><span data-ttu-id="c943b-106">Membros</span><span class="sxs-lookup"><span data-stu-id="c943b-106">Members</span></span>
|<span data-ttu-id="c943b-107">Membro</span><span class="sxs-lookup"><span data-stu-id="c943b-107">Member</span></span>|<span data-ttu-id="c943b-108">Valor</span><span class="sxs-lookup"><span data-stu-id="c943b-108">Value</span></span>|<span data-ttu-id="c943b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c943b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c943b-110">userDefined</span><span class="sxs-lookup"><span data-stu-id="c943b-110">userDefined</span></span>|<span data-ttu-id="c943b-111">0</span><span class="sxs-lookup"><span data-stu-id="c943b-111">0</span></span>|<span data-ttu-id="c943b-112">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="c943b-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="c943b-113">alwaysNotify</span><span class="sxs-lookup"><span data-stu-id="c943b-113">alwaysNotify</span></span>|<span data-ttu-id="c943b-114">1</span><span class="sxs-lookup"><span data-stu-id="c943b-114">1</span></span>|<span data-ttu-id="c943b-115">Sempre notifica.</span><span class="sxs-lookup"><span data-stu-id="c943b-115">Always notify.</span></span>|
|<span data-ttu-id="c943b-116">notifyOnAppChanges</span><span class="sxs-lookup"><span data-stu-id="c943b-116">notifyOnAppChanges</span></span>|<span data-ttu-id="c943b-117">2</span><span class="sxs-lookup"><span data-stu-id="c943b-117">2</span></span>|<span data-ttu-id="c943b-118">Notifica sobre alterações de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c943b-118">Notify on app changes.</span></span>|
|<span data-ttu-id="c943b-119">notifyOnAppChangesWithoutDimming</span><span class="sxs-lookup"><span data-stu-id="c943b-119">notifyOnAppChangesWithoutDimming</span></span>|<span data-ttu-id="c943b-120">3</span><span class="sxs-lookup"><span data-stu-id="c943b-120">3</span></span>|<span data-ttu-id="c943b-121">Notifica sobre mudanças de app sem escurecer a área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="c943b-121">Notify on app changes without dimming desktop.</span></span>|
|<span data-ttu-id="c943b-122">neverNotify</span><span class="sxs-lookup"><span data-stu-id="c943b-122">neverNotify</span></span>|<span data-ttu-id="c943b-123">4</span><span class="sxs-lookup"><span data-stu-id="c943b-123">4</span></span>|<span data-ttu-id="c943b-124">Nunca notifica.</span><span class="sxs-lookup"><span data-stu-id="c943b-124">Never notify.</span></span>|



