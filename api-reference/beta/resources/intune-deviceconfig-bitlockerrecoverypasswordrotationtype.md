---
title: tipo de enumeração bitLockerRecoveryPasswordRotationType
description: Tipo de rotação da senha de recuperação do BitLocker
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c8a597619c0fa7358f6d86fec3ce12d89257b849
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43469669"
---
# <a name="bitlockerrecoverypasswordrotationtype-enum-type"></a><span data-ttu-id="6e035-103">tipo de enumeração bitLockerRecoveryPasswordRotationType</span><span class="sxs-lookup"><span data-stu-id="6e035-103">bitLockerRecoveryPasswordRotationType enum type</span></span>

<span data-ttu-id="6e035-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e035-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6e035-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6e035-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6e035-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6e035-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e035-107">Tipo de rotação da senha de recuperação do BitLocker</span><span class="sxs-lookup"><span data-stu-id="6e035-107">BitLocker recovery password rotation type</span></span>

## <a name="members"></a><span data-ttu-id="6e035-108">Membros</span><span class="sxs-lookup"><span data-stu-id="6e035-108">Members</span></span>
|<span data-ttu-id="6e035-109">Membro</span><span class="sxs-lookup"><span data-stu-id="6e035-109">Member</span></span>|<span data-ttu-id="6e035-110">Valor</span><span class="sxs-lookup"><span data-stu-id="6e035-110">Value</span></span>|<span data-ttu-id="6e035-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e035-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e035-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="6e035-112">notConfigured</span></span>|<span data-ttu-id="6e035-113">,0</span><span class="sxs-lookup"><span data-stu-id="6e035-113">0</span></span>|<span data-ttu-id="6e035-114">Não configurado</span><span class="sxs-lookup"><span data-stu-id="6e035-114">Not configured</span></span>|
|<span data-ttu-id="6e035-115">desabilitadas</span><span class="sxs-lookup"><span data-stu-id="6e035-115">disabled</span></span>|<span data-ttu-id="6e035-116">1</span><span class="sxs-lookup"><span data-stu-id="6e035-116">1</span></span>|<span data-ttu-id="6e035-117">Rotação da senha de recuperação desativada</span><span class="sxs-lookup"><span data-stu-id="6e035-117">Recovery password rotation off</span></span>|
|<span data-ttu-id="6e035-118">enabledForAzureAd</span><span class="sxs-lookup"><span data-stu-id="6e035-118">enabledForAzureAd</span></span>|<span data-ttu-id="6e035-119">duas</span><span class="sxs-lookup"><span data-stu-id="6e035-119">2</span></span>|<span data-ttu-id="6e035-120">Rotação da senha de recuperação em dispositivos ingressados no Azure AD</span><span class="sxs-lookup"><span data-stu-id="6e035-120">Recovery password rotation on for Azure AD joined devices</span></span>|
|<span data-ttu-id="6e035-121">enabledForAzureAdAndHybrid</span><span class="sxs-lookup"><span data-stu-id="6e035-121">enabledForAzureAdAndHybrid</span></span>|<span data-ttu-id="6e035-122">3D</span><span class="sxs-lookup"><span data-stu-id="6e035-122">3</span></span>|<span data-ttu-id="6e035-123">Rotação da senha de recuperação para os dispositivos ingressados e híbridos do Azure AD</span><span class="sxs-lookup"><span data-stu-id="6e035-123">Recovery password rotation on for both Azure AD joined and hybrid joined devices</span></span>|



