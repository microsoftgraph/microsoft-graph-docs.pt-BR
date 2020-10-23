---
title: tipo de enumeração vpnAuthenticationMethod
description: Método de autenticação VPN.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: dbb441bfc32e2de64f5950c033bdd24a3b05c59e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726374"
---
# <a name="vpnauthenticationmethod-enum-type"></a><span data-ttu-id="6efde-103">tipo de enumeração vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6efde-103">vpnAuthenticationMethod enum type</span></span>

<span data-ttu-id="6efde-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6efde-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6efde-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6efde-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6efde-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6efde-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6efde-107">Método de autenticação VPN.</span><span class="sxs-lookup"><span data-stu-id="6efde-107">VPN Authentication Method.</span></span>

## <a name="members"></a><span data-ttu-id="6efde-108">Membros</span><span class="sxs-lookup"><span data-stu-id="6efde-108">Members</span></span>
|<span data-ttu-id="6efde-109">Membro</span><span class="sxs-lookup"><span data-stu-id="6efde-109">Member</span></span>|<span data-ttu-id="6efde-110">Valor</span><span class="sxs-lookup"><span data-stu-id="6efde-110">Value</span></span>|<span data-ttu-id="6efde-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6efde-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6efde-112">certificado</span><span class="sxs-lookup"><span data-stu-id="6efde-112">certificate</span></span>|<span data-ttu-id="6efde-113">,0</span><span class="sxs-lookup"><span data-stu-id="6efde-113">0</span></span>|<span data-ttu-id="6efde-114">Autenticar com um certificado.</span><span class="sxs-lookup"><span data-stu-id="6efde-114">Authenticate with a certificate.</span></span>|
|<span data-ttu-id="6efde-115">usernameAndPassword</span><span class="sxs-lookup"><span data-stu-id="6efde-115">usernameAndPassword</span></span>|<span data-ttu-id="6efde-116">1</span><span class="sxs-lookup"><span data-stu-id="6efde-116">1</span></span>|<span data-ttu-id="6efde-117">Usar nome de usuário e senha para autenticação.</span><span class="sxs-lookup"><span data-stu-id="6efde-117">Use username and password for authentication.</span></span>|
|<span data-ttu-id="6efde-118">sharedSecret</span><span class="sxs-lookup"><span data-stu-id="6efde-118">sharedSecret</span></span>|<span data-ttu-id="6efde-119">duas</span><span class="sxs-lookup"><span data-stu-id="6efde-119">2</span></span>|<span data-ttu-id="6efde-120">Usar segredo compartilhado para autenticação.</span><span class="sxs-lookup"><span data-stu-id="6efde-120">Use Shared Secret for Authentication.</span></span>  <span data-ttu-id="6efde-121">Válido somente para iOS IKEv2.</span><span class="sxs-lookup"><span data-stu-id="6efde-121">Only valid for iOS IKEv2.</span></span>|
|<span data-ttu-id="6efde-122">derivedCredential</span><span class="sxs-lookup"><span data-stu-id="6efde-122">derivedCredential</span></span>|<span data-ttu-id="6efde-123">3D</span><span class="sxs-lookup"><span data-stu-id="6efde-123">3</span></span>|<span data-ttu-id="6efde-124">Use a credencial derivada para autenticação.</span><span class="sxs-lookup"><span data-stu-id="6efde-124">Use Derived Credential for Authentication.</span></span>|
|<span data-ttu-id="6efde-125">azureAD</span><span class="sxs-lookup"><span data-stu-id="6efde-125">azureAD</span></span>|<span data-ttu-id="6efde-126">4 </span><span class="sxs-lookup"><span data-stu-id="6efde-126">4</span></span>|<span data-ttu-id="6efde-127">Usar o Azure AD para autenticação.</span><span class="sxs-lookup"><span data-stu-id="6efde-127">Use Azure AD for authentication.</span></span>|





