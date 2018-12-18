---
title: tipo de enum eapFastConfiguration
description: Configurações disponíveis para a configuração de EAP-FAST.
author: tfitzmac
ms.openlocfilehash: ba84adb86e9910df47bd236fd2bd348cbc9c8e6f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326359"
---
# <a name="eapfastconfiguration-enum-type"></a><span data-ttu-id="f8989-103">tipo de enum eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="f8989-103">eapFastConfiguration enum type</span></span>

> <span data-ttu-id="f8989-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f8989-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f8989-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f8989-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f8989-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f8989-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f8989-107">Configurações disponíveis para a configuração de EAP-FAST.</span><span class="sxs-lookup"><span data-stu-id="f8989-107">Available settings for EAP-FAST Configuration.</span></span>
## <a name="members"></a><span data-ttu-id="f8989-108">Membros</span><span class="sxs-lookup"><span data-stu-id="f8989-108">Members</span></span>
|<span data-ttu-id="f8989-109">Membro</span><span class="sxs-lookup"><span data-stu-id="f8989-109">Member</span></span>|<span data-ttu-id="f8989-110">Valor</span><span class="sxs-lookup"><span data-stu-id="f8989-110">Value</span></span>|<span data-ttu-id="f8989-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8989-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8989-112">noProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="f8989-112">noProtectedAccessCredential</span></span>|<span data-ttu-id="f8989-113">0</span><span class="sxs-lookup"><span data-stu-id="f8989-113">0</span></span>|<span data-ttu-id="f8989-114">Use EAP-FAST sem credencial de acesso protegido (PAC).</span><span class="sxs-lookup"><span data-stu-id="f8989-114">Use EAP-FAST without Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="f8989-115">useProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="f8989-115">useProtectedAccessCredential</span></span>|<span data-ttu-id="f8989-116">1</span><span class="sxs-lookup"><span data-stu-id="f8989-116">1</span></span>|<span data-ttu-id="f8989-117">Uso protegido credencial de acesso (PAC).</span><span class="sxs-lookup"><span data-stu-id="f8989-117">Use Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="f8989-118">useProtectedAccessCredentialAndProvision</span><span class="sxs-lookup"><span data-stu-id="f8989-118">useProtectedAccessCredentialAndProvision</span></span>|<span data-ttu-id="f8989-119">2</span><span class="sxs-lookup"><span data-stu-id="f8989-119">2</span></span>|<span data-ttu-id="f8989-120">Uso Protected Access credencial (PAC) e provisionar PAC.</span><span class="sxs-lookup"><span data-stu-id="f8989-120">Use Protected Access Credential (PAC) and Provision PAC.</span></span>|
|<span data-ttu-id="f8989-121">useProtectedAccessCredentialAndProvisionAnonymously</span><span class="sxs-lookup"><span data-stu-id="f8989-121">useProtectedAccessCredentialAndProvisionAnonymously</span></span>|<span data-ttu-id="f8989-122">3</span><span class="sxs-lookup"><span data-stu-id="f8989-122">3</span></span>|<span data-ttu-id="f8989-123">Use credenciais PAC (Protected Access), provisão PAC e fazê-lo anonimamente.</span><span class="sxs-lookup"><span data-stu-id="f8989-123">Use Protected Access Credential (PAC), Provision PAC, and do so anonymously.</span></span>|





