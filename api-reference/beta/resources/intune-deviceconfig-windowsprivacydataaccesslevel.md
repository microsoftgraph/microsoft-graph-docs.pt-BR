---
title: tipo de enum windowsPrivacyDataAccessLevel
description: Determine o nível de acesso a categoria de dados de privacidade Windows específica.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 74ab32a703422203fec7a6c9ed1bc035e01949a9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888771"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a><span data-ttu-id="5000c-103">tipo de enum windowsPrivacyDataAccessLevel</span><span class="sxs-lookup"><span data-stu-id="5000c-103">windowsPrivacyDataAccessLevel enum type</span></span>

> <span data-ttu-id="5000c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5000c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5000c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5000c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5000c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5000c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5000c-107">Determine o nível de acesso a categoria de dados de privacidade Windows específica.</span><span class="sxs-lookup"><span data-stu-id="5000c-107">Determine the access level to specific Windows privacy data category.</span></span>
## <a name="members"></a><span data-ttu-id="5000c-108">Membros</span><span class="sxs-lookup"><span data-stu-id="5000c-108">Members</span></span>
|<span data-ttu-id="5000c-109">Membro</span><span class="sxs-lookup"><span data-stu-id="5000c-109">Member</span></span>|<span data-ttu-id="5000c-110">Valor</span><span class="sxs-lookup"><span data-stu-id="5000c-110">Value</span></span>|<span data-ttu-id="5000c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5000c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5000c-112">não-configuradas</span><span class="sxs-lookup"><span data-stu-id="5000c-112">notConfigured</span></span>|<span data-ttu-id="5000c-113">0</span><span class="sxs-lookup"><span data-stu-id="5000c-113">0</span></span>|<span data-ttu-id="5000c-114">Nenhum nível de acesso não especificado, nenhum propósitos.</span><span class="sxs-lookup"><span data-stu-id="5000c-114">No access level specified, no intents.</span></span> <span data-ttu-id="5000c-115">Dispositivo pode se comportam tanto como UserInControl ou ForceAllow.</span><span class="sxs-lookup"><span data-stu-id="5000c-115">Device may behave either as in UserInControl or ForceAllow.</span></span> <span data-ttu-id="5000c-116">Ele pode depender os dados de privacidade foram acessados, versões do Windows e outros fatores.</span><span class="sxs-lookup"><span data-stu-id="5000c-116">It may depend on the privacy data been accessed, Windows versions and other factors.</span></span>|
|<span data-ttu-id="5000c-117">forceAllow</span><span class="sxs-lookup"><span data-stu-id="5000c-117">forceAllow</span></span>|<span data-ttu-id="5000c-118">1</span><span class="sxs-lookup"><span data-stu-id="5000c-118">1</span></span>|<span data-ttu-id="5000c-119">Aplicativos poderão acessar os dados de privacidade especificado.</span><span class="sxs-lookup"><span data-stu-id="5000c-119">Apps will be allowed to access the specified privacy data.</span></span>|
|<span data-ttu-id="5000c-120">forceDeny</span><span class="sxs-lookup"><span data-stu-id="5000c-120">forceDeny</span></span>|<span data-ttu-id="5000c-121">2</span><span class="sxs-lookup"><span data-stu-id="5000c-121">2</span></span>|<span data-ttu-id="5000c-122">Aplicativos serão negados para acessar os dados de privacidade especificado.</span><span class="sxs-lookup"><span data-stu-id="5000c-122">Apps will be denied to access specified privacy data.</span></span>|
|<span data-ttu-id="5000c-123">userInControl</span><span class="sxs-lookup"><span data-stu-id="5000c-123">userInControl</span></span>|<span data-ttu-id="5000c-124">3</span><span class="sxs-lookup"><span data-stu-id="5000c-124">3</span></span>|<span data-ttu-id="5000c-125">Os usuários serão solicitados quando apps tentam acessar os dados de privacidade especificado.</span><span class="sxs-lookup"><span data-stu-id="5000c-125">Users will be prompted when apps try to access specified privacy data.</span></span>|





