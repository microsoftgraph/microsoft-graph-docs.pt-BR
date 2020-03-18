---
title: tipo de enumeração eapFastConfiguration
description: Configurações disponíveis para a configuração EAP-FAST.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b70e2688473f9af93dcd3b0f0d4d05b77d81446f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791951"
---
# <a name="eapfastconfiguration-enum-type"></a><span data-ttu-id="cb470-103">tipo de enumeração eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="cb470-103">eapFastConfiguration enum type</span></span>

> <span data-ttu-id="cb470-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cb470-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb470-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cb470-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb470-106">Configurações disponíveis para a configuração EAP-FAST.</span><span class="sxs-lookup"><span data-stu-id="cb470-106">Available settings for EAP-FAST Configuration.</span></span>

## <a name="members"></a><span data-ttu-id="cb470-107">Membros</span><span class="sxs-lookup"><span data-stu-id="cb470-107">Members</span></span>
|<span data-ttu-id="cb470-108">Membro</span><span class="sxs-lookup"><span data-stu-id="cb470-108">Member</span></span>|<span data-ttu-id="cb470-109">Valor</span><span class="sxs-lookup"><span data-stu-id="cb470-109">Value</span></span>|<span data-ttu-id="cb470-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb470-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb470-111">noProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="cb470-111">noProtectedAccessCredential</span></span>|<span data-ttu-id="cb470-112">,0</span><span class="sxs-lookup"><span data-stu-id="cb470-112">0</span></span>|<span data-ttu-id="cb470-113">Use EAP-FAST sem PAC (credencial de acesso protegido).</span><span class="sxs-lookup"><span data-stu-id="cb470-113">Use EAP-FAST without Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="cb470-114">useProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="cb470-114">useProtectedAccessCredential</span></span>|<span data-ttu-id="cb470-115">1</span><span class="sxs-lookup"><span data-stu-id="cb470-115">1</span></span>|<span data-ttu-id="cb470-116">Use a PAC (credencial de acesso protegido).</span><span class="sxs-lookup"><span data-stu-id="cb470-116">Use Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="cb470-117">useProtectedAccessCredentialAndProvision</span><span class="sxs-lookup"><span data-stu-id="cb470-117">useProtectedAccessCredentialAndProvision</span></span>|<span data-ttu-id="cb470-118">duas</span><span class="sxs-lookup"><span data-stu-id="cb470-118">2</span></span>|<span data-ttu-id="cb470-119">Use a PAC (credencial de acesso protegido) e provisionar PAC.</span><span class="sxs-lookup"><span data-stu-id="cb470-119">Use Protected Access Credential (PAC) and Provision PAC.</span></span>|
|<span data-ttu-id="cb470-120">useProtectedAccessCredentialAndProvisionAnonymously</span><span class="sxs-lookup"><span data-stu-id="cb470-120">useProtectedAccessCredentialAndProvisionAnonymously</span></span>|<span data-ttu-id="cb470-121">3D</span><span class="sxs-lookup"><span data-stu-id="cb470-121">3</span></span>|<span data-ttu-id="cb470-122">Use a PAC (credencial de acesso protegido), provisione PAC e faça isso de forma anônima.</span><span class="sxs-lookup"><span data-stu-id="cb470-122">Use Protected Access Credential (PAC), Provision PAC, and do so anonymously.</span></span>|



