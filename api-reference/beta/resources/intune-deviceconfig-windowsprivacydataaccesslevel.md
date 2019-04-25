---
title: tipo de enumeração windowsPrivacyDataAccessLevel
description: Determine o nível de acesso à categoria de dados de privacidade do Windows específica.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 10486899094cf275cb3fb9254114d92cb7d12388
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541346"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a><span data-ttu-id="ea20a-103">tipo de enumeração windowsPrivacyDataAccessLevel</span><span class="sxs-lookup"><span data-stu-id="ea20a-103">windowsPrivacyDataAccessLevel enum type</span></span>

> <span data-ttu-id="ea20a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ea20a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea20a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ea20a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea20a-106">Determine o nível de acesso à categoria de dados de privacidade do Windows específica.</span><span class="sxs-lookup"><span data-stu-id="ea20a-106">Determine the access level to specific Windows privacy data category.</span></span>

## <a name="members"></a><span data-ttu-id="ea20a-107">Membros</span><span class="sxs-lookup"><span data-stu-id="ea20a-107">Members</span></span>
|<span data-ttu-id="ea20a-108">Membro</span><span class="sxs-lookup"><span data-stu-id="ea20a-108">Member</span></span>|<span data-ttu-id="ea20a-109">Valor</span><span class="sxs-lookup"><span data-stu-id="ea20a-109">Value</span></span>|<span data-ttu-id="ea20a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea20a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea20a-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="ea20a-111">notConfigured</span></span>|<span data-ttu-id="ea20a-112">,0</span><span class="sxs-lookup"><span data-stu-id="ea20a-112">0</span></span>|<span data-ttu-id="ea20a-113">Nenhum nível de acesso especificado, sem tentativas.</span><span class="sxs-lookup"><span data-stu-id="ea20a-113">No access level specified, no intents.</span></span> <span data-ttu-id="ea20a-114">O dispositivo pode se comportar como no UserInControl ou no ForceAllow.</span><span class="sxs-lookup"><span data-stu-id="ea20a-114">Device may behave either as in UserInControl or ForceAllow.</span></span> <span data-ttu-id="ea20a-115">Pode depender que os dados de privacidade foram acessados, versões do Windows e outros fatores.</span><span class="sxs-lookup"><span data-stu-id="ea20a-115">It may depend on the privacy data been accessed, Windows versions and other factors.</span></span>|
|<span data-ttu-id="ea20a-116">forceAllow</span><span class="sxs-lookup"><span data-stu-id="ea20a-116">forceAllow</span></span>|<span data-ttu-id="ea20a-117">1 </span><span class="sxs-lookup"><span data-stu-id="ea20a-117">1</span></span>|<span data-ttu-id="ea20a-118">Os aplicativos terão permissão para acessar os dados de privacidade especificados.</span><span class="sxs-lookup"><span data-stu-id="ea20a-118">Apps will be allowed to access the specified privacy data.</span></span>|
|<span data-ttu-id="ea20a-119">forceDeny</span><span class="sxs-lookup"><span data-stu-id="ea20a-119">forceDeny</span></span>|<span data-ttu-id="ea20a-120">2 </span><span class="sxs-lookup"><span data-stu-id="ea20a-120">2</span></span>|<span data-ttu-id="ea20a-121">Os aplicativos serão negados para acessar os dados de privacidade especificados.</span><span class="sxs-lookup"><span data-stu-id="ea20a-121">Apps will be denied to access specified privacy data.</span></span>|
|<span data-ttu-id="ea20a-122">userInControl</span><span class="sxs-lookup"><span data-stu-id="ea20a-122">userInControl</span></span>|<span data-ttu-id="ea20a-123">3 </span><span class="sxs-lookup"><span data-stu-id="ea20a-123">3</span></span>|<span data-ttu-id="ea20a-124">Os usuários serão solicitados quando os aplicativos tentarem acessar dados de privacidade especificados.</span><span class="sxs-lookup"><span data-stu-id="ea20a-124">Users will be prompted when apps try to access specified privacy data.</span></span>|





