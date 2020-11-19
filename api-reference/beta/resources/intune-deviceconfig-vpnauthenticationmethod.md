---
title: tipo de enumeração vpnAuthenticationMethod
description: Método de autenticação VPN.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3ffc71fa17385ad1e0d00dd77958e65fb7a4aed9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49276312"
---
# <a name="vpnauthenticationmethod-enum-type"></a><span data-ttu-id="f3f27-103">tipo de enumeração vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f3f27-103">vpnAuthenticationMethod enum type</span></span>

<span data-ttu-id="f3f27-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3f27-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f3f27-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f3f27-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3f27-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f3f27-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3f27-107">Método de autenticação VPN.</span><span class="sxs-lookup"><span data-stu-id="f3f27-107">VPN Authentication Method.</span></span>

## <a name="members"></a><span data-ttu-id="f3f27-108">Membros</span><span class="sxs-lookup"><span data-stu-id="f3f27-108">Members</span></span>
|<span data-ttu-id="f3f27-109">Membro</span><span class="sxs-lookup"><span data-stu-id="f3f27-109">Member</span></span>|<span data-ttu-id="f3f27-110">Valor</span><span class="sxs-lookup"><span data-stu-id="f3f27-110">Value</span></span>|<span data-ttu-id="f3f27-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3f27-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3f27-112">certificado</span><span class="sxs-lookup"><span data-stu-id="f3f27-112">certificate</span></span>|<span data-ttu-id="f3f27-113">,0</span><span class="sxs-lookup"><span data-stu-id="f3f27-113">0</span></span>|<span data-ttu-id="f3f27-114">Autenticar com um certificado.</span><span class="sxs-lookup"><span data-stu-id="f3f27-114">Authenticate with a certificate.</span></span>|
|<span data-ttu-id="f3f27-115">usernameAndPassword</span><span class="sxs-lookup"><span data-stu-id="f3f27-115">usernameAndPassword</span></span>|<span data-ttu-id="f3f27-116">1</span><span class="sxs-lookup"><span data-stu-id="f3f27-116">1</span></span>|<span data-ttu-id="f3f27-117">Usar nome de usuário e senha para autenticação.</span><span class="sxs-lookup"><span data-stu-id="f3f27-117">Use username and password for authentication.</span></span>|
|<span data-ttu-id="f3f27-118">sharedSecret</span><span class="sxs-lookup"><span data-stu-id="f3f27-118">sharedSecret</span></span>|<span data-ttu-id="f3f27-119">duas</span><span class="sxs-lookup"><span data-stu-id="f3f27-119">2</span></span>|<span data-ttu-id="f3f27-120">Usar segredo compartilhado para autenticação.</span><span class="sxs-lookup"><span data-stu-id="f3f27-120">Use Shared Secret for Authentication.</span></span>  <span data-ttu-id="f3f27-121">Válido somente para iOS IKEv2.</span><span class="sxs-lookup"><span data-stu-id="f3f27-121">Only valid for iOS IKEv2.</span></span>|
|<span data-ttu-id="f3f27-122">derivedCredential</span><span class="sxs-lookup"><span data-stu-id="f3f27-122">derivedCredential</span></span>|<span data-ttu-id="f3f27-123">3D</span><span class="sxs-lookup"><span data-stu-id="f3f27-123">3</span></span>|<span data-ttu-id="f3f27-124">Use a credencial derivada para autenticação.</span><span class="sxs-lookup"><span data-stu-id="f3f27-124">Use Derived Credential for Authentication.</span></span>|
|<span data-ttu-id="f3f27-125">azureAD</span><span class="sxs-lookup"><span data-stu-id="f3f27-125">azureAD</span></span>|<span data-ttu-id="f3f27-126">4 </span><span class="sxs-lookup"><span data-stu-id="f3f27-126">4</span></span>|<span data-ttu-id="f3f27-127">Usar o Azure AD para autenticação.</span><span class="sxs-lookup"><span data-stu-id="f3f27-127">Use Azure AD for authentication.</span></span>|




