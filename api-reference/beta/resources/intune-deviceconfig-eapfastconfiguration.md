---
title: tipo de enumeração eapFastConfiguration
description: Configurações disponíveis para a configuração EAP-FAST.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: db3f39eaeb375705c974e907ae4b0a177bd6c4ac
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526543"
---
# <a name="eapfastconfiguration-enum-type"></a><span data-ttu-id="d557a-103">tipo de enumeração eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="d557a-103">eapFastConfiguration enum type</span></span>

<span data-ttu-id="d557a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d557a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d557a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d557a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d557a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d557a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d557a-107">Configurações disponíveis para a configuração EAP-FAST.</span><span class="sxs-lookup"><span data-stu-id="d557a-107">Available settings for EAP-FAST Configuration.</span></span>

## <a name="members"></a><span data-ttu-id="d557a-108">Membros</span><span class="sxs-lookup"><span data-stu-id="d557a-108">Members</span></span>
|<span data-ttu-id="d557a-109">Membro</span><span class="sxs-lookup"><span data-stu-id="d557a-109">Member</span></span>|<span data-ttu-id="d557a-110">Valor</span><span class="sxs-lookup"><span data-stu-id="d557a-110">Value</span></span>|<span data-ttu-id="d557a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d557a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d557a-112">noProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="d557a-112">noProtectedAccessCredential</span></span>|<span data-ttu-id="d557a-113">,0</span><span class="sxs-lookup"><span data-stu-id="d557a-113">0</span></span>|<span data-ttu-id="d557a-114">Use EAP-FAST sem PAC (credencial de acesso protegido).</span><span class="sxs-lookup"><span data-stu-id="d557a-114">Use EAP-FAST without Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="d557a-115">useProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="d557a-115">useProtectedAccessCredential</span></span>|<span data-ttu-id="d557a-116">1 </span><span class="sxs-lookup"><span data-stu-id="d557a-116">1</span></span>|<span data-ttu-id="d557a-117">Use a PAC (credencial de acesso protegido).</span><span class="sxs-lookup"><span data-stu-id="d557a-117">Use Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="d557a-118">useProtectedAccessCredentialAndProvision</span><span class="sxs-lookup"><span data-stu-id="d557a-118">useProtectedAccessCredentialAndProvision</span></span>|<span data-ttu-id="d557a-119">2 </span><span class="sxs-lookup"><span data-stu-id="d557a-119">2</span></span>|<span data-ttu-id="d557a-120">Use a PAC (credencial de acesso protegido) e provisionar PAC.</span><span class="sxs-lookup"><span data-stu-id="d557a-120">Use Protected Access Credential (PAC) and Provision PAC.</span></span>|
|<span data-ttu-id="d557a-121">useProtectedAccessCredentialAndProvisionAnonymously</span><span class="sxs-lookup"><span data-stu-id="d557a-121">useProtectedAccessCredentialAndProvisionAnonymously</span></span>|<span data-ttu-id="d557a-122">3 </span><span class="sxs-lookup"><span data-stu-id="d557a-122">3</span></span>|<span data-ttu-id="d557a-123">Use a PAC (credencial de acesso protegido), provisione PAC e faça isso de forma anônima.</span><span class="sxs-lookup"><span data-stu-id="d557a-123">Use Protected Access Credential (PAC), Provision PAC, and do so anonymously.</span></span>|



