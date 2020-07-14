---
title: tipo de enumeração vpnAuthenticationMethod
description: Método de autenticação VPN.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ef477b17b8ae7e8aedc3b95ce70b66115a3c8712
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123887"
---
# <a name="vpnauthenticationmethod-enum-type"></a><span data-ttu-id="e48b3-103">tipo de enumeração vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="e48b3-103">vpnAuthenticationMethod enum type</span></span>

<span data-ttu-id="e48b3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e48b3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e48b3-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e48b3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e48b3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e48b3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e48b3-107">Método de autenticação VPN.</span><span class="sxs-lookup"><span data-stu-id="e48b3-107">VPN Authentication Method.</span></span>

## <a name="members"></a><span data-ttu-id="e48b3-108">Membros</span><span class="sxs-lookup"><span data-stu-id="e48b3-108">Members</span></span>
|<span data-ttu-id="e48b3-109">Membro</span><span class="sxs-lookup"><span data-stu-id="e48b3-109">Member</span></span>|<span data-ttu-id="e48b3-110">Valor</span><span class="sxs-lookup"><span data-stu-id="e48b3-110">Value</span></span>|<span data-ttu-id="e48b3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e48b3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e48b3-112">certificado</span><span class="sxs-lookup"><span data-stu-id="e48b3-112">certificate</span></span>|<span data-ttu-id="e48b3-113">,0</span><span class="sxs-lookup"><span data-stu-id="e48b3-113">0</span></span>|<span data-ttu-id="e48b3-114">Autenticar com um certificado.</span><span class="sxs-lookup"><span data-stu-id="e48b3-114">Authenticate with a certificate.</span></span>|
|<span data-ttu-id="e48b3-115">usernameAndPassword</span><span class="sxs-lookup"><span data-stu-id="e48b3-115">usernameAndPassword</span></span>|<span data-ttu-id="e48b3-116">1 </span><span class="sxs-lookup"><span data-stu-id="e48b3-116">1</span></span>|<span data-ttu-id="e48b3-117">Usar nome de usuário e senha para autenticação.</span><span class="sxs-lookup"><span data-stu-id="e48b3-117">Use username and password for authentication.</span></span>|
|<span data-ttu-id="e48b3-118">sharedSecret</span><span class="sxs-lookup"><span data-stu-id="e48b3-118">sharedSecret</span></span>|<span data-ttu-id="e48b3-119">2 </span><span class="sxs-lookup"><span data-stu-id="e48b3-119">2</span></span>|<span data-ttu-id="e48b3-120">Usar segredo compartilhado para autenticação.</span><span class="sxs-lookup"><span data-stu-id="e48b3-120">Use Shared Secret for Authentication.</span></span>  <span data-ttu-id="e48b3-121">Válido somente para iOS IKEv2.</span><span class="sxs-lookup"><span data-stu-id="e48b3-121">Only valid for iOS IKEv2.</span></span>|
|<span data-ttu-id="e48b3-122">derivedCredential</span><span class="sxs-lookup"><span data-stu-id="e48b3-122">derivedCredential</span></span>|<span data-ttu-id="e48b3-123">3 </span><span class="sxs-lookup"><span data-stu-id="e48b3-123">3</span></span>|<span data-ttu-id="e48b3-124">Use a credencial derivada para autenticação.</span><span class="sxs-lookup"><span data-stu-id="e48b3-124">Use Derived Credential for Authentication.</span></span>|
|<span data-ttu-id="e48b3-125">azureAD</span><span class="sxs-lookup"><span data-stu-id="e48b3-125">azureAD</span></span>|<span data-ttu-id="e48b3-126">4 </span><span class="sxs-lookup"><span data-stu-id="e48b3-126">4</span></span>|<span data-ttu-id="e48b3-127">Usar o Azure AD para autenticação.</span><span class="sxs-lookup"><span data-stu-id="e48b3-127">Use Azure AD for authentication.</span></span>|



