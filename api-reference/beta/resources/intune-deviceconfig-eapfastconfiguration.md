---
title: tipo de enum eapFastConfiguration
description: Configurações disponíveis para a configuração de EAP-FAST.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 65165929d388ed57f2651a0d277996e56d2f046e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954453"
---
# <a name="eapfastconfiguration-enum-type"></a><span data-ttu-id="77cb9-103">tipo de enum eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="77cb9-103">eapFastConfiguration enum type</span></span>

> <span data-ttu-id="77cb9-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="77cb9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="77cb9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="77cb9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="77cb9-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="77cb9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="77cb9-107">Configurações disponíveis para a configuração de EAP-FAST.</span><span class="sxs-lookup"><span data-stu-id="77cb9-107">Available settings for EAP-FAST Configuration.</span></span>
## <a name="members"></a><span data-ttu-id="77cb9-108">Membros</span><span class="sxs-lookup"><span data-stu-id="77cb9-108">Members</span></span>
|<span data-ttu-id="77cb9-109">Membro</span><span class="sxs-lookup"><span data-stu-id="77cb9-109">Member</span></span>|<span data-ttu-id="77cb9-110">Valor</span><span class="sxs-lookup"><span data-stu-id="77cb9-110">Value</span></span>|<span data-ttu-id="77cb9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="77cb9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77cb9-112">noProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="77cb9-112">noProtectedAccessCredential</span></span>|<span data-ttu-id="77cb9-113">0</span><span class="sxs-lookup"><span data-stu-id="77cb9-113">0</span></span>|<span data-ttu-id="77cb9-114">Use EAP-FAST sem credencial de acesso protegido (PAC).</span><span class="sxs-lookup"><span data-stu-id="77cb9-114">Use EAP-FAST without Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="77cb9-115">useProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="77cb9-115">useProtectedAccessCredential</span></span>|<span data-ttu-id="77cb9-116">1</span><span class="sxs-lookup"><span data-stu-id="77cb9-116">1</span></span>|<span data-ttu-id="77cb9-117">Uso protegido credencial de acesso (PAC).</span><span class="sxs-lookup"><span data-stu-id="77cb9-117">Use Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="77cb9-118">useProtectedAccessCredentialAndProvision</span><span class="sxs-lookup"><span data-stu-id="77cb9-118">useProtectedAccessCredentialAndProvision</span></span>|<span data-ttu-id="77cb9-119">2</span><span class="sxs-lookup"><span data-stu-id="77cb9-119">2</span></span>|<span data-ttu-id="77cb9-120">Uso Protected Access credencial (PAC) e provisionar PAC.</span><span class="sxs-lookup"><span data-stu-id="77cb9-120">Use Protected Access Credential (PAC) and Provision PAC.</span></span>|
|<span data-ttu-id="77cb9-121">useProtectedAccessCredentialAndProvisionAnonymously</span><span class="sxs-lookup"><span data-stu-id="77cb9-121">useProtectedAccessCredentialAndProvisionAnonymously</span></span>|<span data-ttu-id="77cb9-122">3</span><span class="sxs-lookup"><span data-stu-id="77cb9-122">3</span></span>|<span data-ttu-id="77cb9-123">Use credenciais PAC (Protected Access), provisão PAC e fazê-lo anonimamente.</span><span class="sxs-lookup"><span data-stu-id="77cb9-123">Use Protected Access Credential (PAC), Provision PAC, and do so anonymously.</span></span>|





