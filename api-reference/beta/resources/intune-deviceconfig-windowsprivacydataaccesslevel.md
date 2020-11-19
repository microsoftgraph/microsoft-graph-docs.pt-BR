---
title: tipo de enumeração windowsPrivacyDataAccessLevel
description: Determine o nível de acesso à categoria de dados de privacidade do Windows específica.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: acd71682d7e682dec53bb87885374aabdd38089d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49215188"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a><span data-ttu-id="8a271-103">tipo de enumeração windowsPrivacyDataAccessLevel</span><span class="sxs-lookup"><span data-stu-id="8a271-103">windowsPrivacyDataAccessLevel enum type</span></span>

<span data-ttu-id="8a271-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a271-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8a271-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8a271-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8a271-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8a271-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a271-107">Determine o nível de acesso à categoria de dados de privacidade do Windows específica.</span><span class="sxs-lookup"><span data-stu-id="8a271-107">Determine the access level to specific Windows privacy data category.</span></span>

## <a name="members"></a><span data-ttu-id="8a271-108">Membros</span><span class="sxs-lookup"><span data-stu-id="8a271-108">Members</span></span>
|<span data-ttu-id="8a271-109">Membro</span><span class="sxs-lookup"><span data-stu-id="8a271-109">Member</span></span>|<span data-ttu-id="8a271-110">Valor</span><span class="sxs-lookup"><span data-stu-id="8a271-110">Value</span></span>|<span data-ttu-id="8a271-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a271-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a271-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="8a271-112">notConfigured</span></span>|<span data-ttu-id="8a271-113">,0</span><span class="sxs-lookup"><span data-stu-id="8a271-113">0</span></span>|<span data-ttu-id="8a271-114">Nenhum nível de acesso especificado, sem tentativas.</span><span class="sxs-lookup"><span data-stu-id="8a271-114">No access level specified, no intents.</span></span> <span data-ttu-id="8a271-115">O dispositivo pode se comportar como no UserInControl ou no ForceAllow.</span><span class="sxs-lookup"><span data-stu-id="8a271-115">Device may behave either as in UserInControl or ForceAllow.</span></span> <span data-ttu-id="8a271-116">Pode depender que os dados de privacidade foram acessados, versões do Windows e outros fatores.</span><span class="sxs-lookup"><span data-stu-id="8a271-116">It may depend on the privacy data been accessed, Windows versions and other factors.</span></span>|
|<span data-ttu-id="8a271-117">forceAllow</span><span class="sxs-lookup"><span data-stu-id="8a271-117">forceAllow</span></span>|<span data-ttu-id="8a271-118">1</span><span class="sxs-lookup"><span data-stu-id="8a271-118">1</span></span>|<span data-ttu-id="8a271-119">Os aplicativos terão permissão para acessar os dados de privacidade especificados.</span><span class="sxs-lookup"><span data-stu-id="8a271-119">Apps will be allowed to access the specified privacy data.</span></span>|
|<span data-ttu-id="8a271-120">forceDeny</span><span class="sxs-lookup"><span data-stu-id="8a271-120">forceDeny</span></span>|<span data-ttu-id="8a271-121">duas</span><span class="sxs-lookup"><span data-stu-id="8a271-121">2</span></span>|<span data-ttu-id="8a271-122">Os aplicativos serão negados para acessar os dados de privacidade especificados.</span><span class="sxs-lookup"><span data-stu-id="8a271-122">Apps will be denied to access specified privacy data.</span></span>|
|<span data-ttu-id="8a271-123">userInControl</span><span class="sxs-lookup"><span data-stu-id="8a271-123">userInControl</span></span>|<span data-ttu-id="8a271-124">3D</span><span class="sxs-lookup"><span data-stu-id="8a271-124">3</span></span>|<span data-ttu-id="8a271-125">Os usuários serão solicitados quando os aplicativos tentarem acessar dados de privacidade especificados.</span><span class="sxs-lookup"><span data-stu-id="8a271-125">Users will be prompted when apps try to access specified privacy data.</span></span>|




