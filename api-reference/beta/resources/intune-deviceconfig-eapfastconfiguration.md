---
title: tipo de enumeração eapFastConfiguration
description: Configurações disponíveis para a configuração EAP-FAST.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f0d045252c058b2557fd9bb4448e0275953e0b09
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43469129"
---
# <a name="eapfastconfiguration-enum-type"></a><span data-ttu-id="c89fe-103">tipo de enumeração eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="c89fe-103">eapFastConfiguration enum type</span></span>

<span data-ttu-id="c89fe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c89fe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c89fe-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c89fe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c89fe-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c89fe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c89fe-107">Configurações disponíveis para a configuração EAP-FAST.</span><span class="sxs-lookup"><span data-stu-id="c89fe-107">Available settings for EAP-FAST Configuration.</span></span>

## <a name="members"></a><span data-ttu-id="c89fe-108">Membros</span><span class="sxs-lookup"><span data-stu-id="c89fe-108">Members</span></span>
|<span data-ttu-id="c89fe-109">Membro</span><span class="sxs-lookup"><span data-stu-id="c89fe-109">Member</span></span>|<span data-ttu-id="c89fe-110">Valor</span><span class="sxs-lookup"><span data-stu-id="c89fe-110">Value</span></span>|<span data-ttu-id="c89fe-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c89fe-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c89fe-112">noProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="c89fe-112">noProtectedAccessCredential</span></span>|<span data-ttu-id="c89fe-113">,0</span><span class="sxs-lookup"><span data-stu-id="c89fe-113">0</span></span>|<span data-ttu-id="c89fe-114">Use EAP-FAST sem PAC (credencial de acesso protegido).</span><span class="sxs-lookup"><span data-stu-id="c89fe-114">Use EAP-FAST without Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="c89fe-115">useProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="c89fe-115">useProtectedAccessCredential</span></span>|<span data-ttu-id="c89fe-116">1</span><span class="sxs-lookup"><span data-stu-id="c89fe-116">1</span></span>|<span data-ttu-id="c89fe-117">Use a PAC (credencial de acesso protegido).</span><span class="sxs-lookup"><span data-stu-id="c89fe-117">Use Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="c89fe-118">useProtectedAccessCredentialAndProvision</span><span class="sxs-lookup"><span data-stu-id="c89fe-118">useProtectedAccessCredentialAndProvision</span></span>|<span data-ttu-id="c89fe-119">duas</span><span class="sxs-lookup"><span data-stu-id="c89fe-119">2</span></span>|<span data-ttu-id="c89fe-120">Use a PAC (credencial de acesso protegido) e provisionar PAC.</span><span class="sxs-lookup"><span data-stu-id="c89fe-120">Use Protected Access Credential (PAC) and Provision PAC.</span></span>|
|<span data-ttu-id="c89fe-121">useProtectedAccessCredentialAndProvisionAnonymously</span><span class="sxs-lookup"><span data-stu-id="c89fe-121">useProtectedAccessCredentialAndProvisionAnonymously</span></span>|<span data-ttu-id="c89fe-122">3D</span><span class="sxs-lookup"><span data-stu-id="c89fe-122">3</span></span>|<span data-ttu-id="c89fe-123">Use a PAC (credencial de acesso protegido), provisione PAC e faça isso de forma anônima.</span><span class="sxs-lookup"><span data-stu-id="c89fe-123">Use Protected Access Credential (PAC), Provision PAC, and do so anonymously.</span></span>|



