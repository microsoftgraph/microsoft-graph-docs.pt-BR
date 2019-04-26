---
title: tipo de enumeração eapFastConfiguration
description: Configurações disponíveis para a configuração EAP-FAST.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7acf6ffbf7a93bc5002f7f81679fc789ab313e2f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567141"
---
# <a name="eapfastconfiguration-enum-type"></a><span data-ttu-id="06730-103">tipo de enumeração eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="06730-103">eapFastConfiguration enum type</span></span>

> <span data-ttu-id="06730-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="06730-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06730-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="06730-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06730-106">Configurações disponíveis para a configuração EAP-FAST.</span><span class="sxs-lookup"><span data-stu-id="06730-106">Available settings for EAP-FAST Configuration.</span></span>

## <a name="members"></a><span data-ttu-id="06730-107">Membros</span><span class="sxs-lookup"><span data-stu-id="06730-107">Members</span></span>
|<span data-ttu-id="06730-108">Membro</span><span class="sxs-lookup"><span data-stu-id="06730-108">Member</span></span>|<span data-ttu-id="06730-109">Valor</span><span class="sxs-lookup"><span data-stu-id="06730-109">Value</span></span>|<span data-ttu-id="06730-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="06730-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06730-111">noProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="06730-111">noProtectedAccessCredential</span></span>|<span data-ttu-id="06730-112">,0</span><span class="sxs-lookup"><span data-stu-id="06730-112">0</span></span>|<span data-ttu-id="06730-113">Use EAP-FAST sem PAC (credencial de acesso protegido).</span><span class="sxs-lookup"><span data-stu-id="06730-113">Use EAP-FAST without Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="06730-114">useProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="06730-114">useProtectedAccessCredential</span></span>|<span data-ttu-id="06730-115">1 </span><span class="sxs-lookup"><span data-stu-id="06730-115">1</span></span>|<span data-ttu-id="06730-116">Use a PAC (credencial de acesso protegido).</span><span class="sxs-lookup"><span data-stu-id="06730-116">Use Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="06730-117">useProtectedAccessCredentialAndProvision</span><span class="sxs-lookup"><span data-stu-id="06730-117">useProtectedAccessCredentialAndProvision</span></span>|<span data-ttu-id="06730-118">2 </span><span class="sxs-lookup"><span data-stu-id="06730-118">2</span></span>|<span data-ttu-id="06730-119">Use a PAC (credencial de acesso protegido) e proVisionar PAC.</span><span class="sxs-lookup"><span data-stu-id="06730-119">Use Protected Access Credential (PAC) and Provision PAC.</span></span>|
|<span data-ttu-id="06730-120">useProtectedAccessCredentialAndProvisionAnonymously</span><span class="sxs-lookup"><span data-stu-id="06730-120">useProtectedAccessCredentialAndProvisionAnonymously</span></span>|<span data-ttu-id="06730-121">3 </span><span class="sxs-lookup"><span data-stu-id="06730-121">3</span></span>|<span data-ttu-id="06730-122">Use a PAC (credencial de acesso protegido), proVisione PAC e faça isso de forma anônima.</span><span class="sxs-lookup"><span data-stu-id="06730-122">Use Protected Access Credential (PAC), Provision PAC, and do so anonymously.</span></span>|





