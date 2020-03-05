---
title: tipo de enumeração vpnAuthenticationMethod
description: Método de autenticação VPN.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 035fe88bbcde357fd67c42252c6e903f1c610275
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525793"
---
# <a name="vpnauthenticationmethod-enum-type"></a><span data-ttu-id="174d9-103">tipo de enumeração vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="174d9-103">vpnAuthenticationMethod enum type</span></span>

<span data-ttu-id="174d9-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="174d9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="174d9-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="174d9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="174d9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="174d9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="174d9-107">Método de autenticação VPN.</span><span class="sxs-lookup"><span data-stu-id="174d9-107">VPN Authentication Method.</span></span>

## <a name="members"></a><span data-ttu-id="174d9-108">Membros</span><span class="sxs-lookup"><span data-stu-id="174d9-108">Members</span></span>
|<span data-ttu-id="174d9-109">Membro</span><span class="sxs-lookup"><span data-stu-id="174d9-109">Member</span></span>|<span data-ttu-id="174d9-110">Valor</span><span class="sxs-lookup"><span data-stu-id="174d9-110">Value</span></span>|<span data-ttu-id="174d9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="174d9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="174d9-112">certificado</span><span class="sxs-lookup"><span data-stu-id="174d9-112">certificate</span></span>|<span data-ttu-id="174d9-113">,0</span><span class="sxs-lookup"><span data-stu-id="174d9-113">0</span></span>|<span data-ttu-id="174d9-114">Autenticar com um certificado.</span><span class="sxs-lookup"><span data-stu-id="174d9-114">Authenticate with a certificate.</span></span>|
|<span data-ttu-id="174d9-115">usernameAndPassword</span><span class="sxs-lookup"><span data-stu-id="174d9-115">usernameAndPassword</span></span>|<span data-ttu-id="174d9-116">1 </span><span class="sxs-lookup"><span data-stu-id="174d9-116">1</span></span>|<span data-ttu-id="174d9-117">Usar nome de usuário e senha para autenticação.</span><span class="sxs-lookup"><span data-stu-id="174d9-117">Use username and password for authentication.</span></span>|
|<span data-ttu-id="174d9-118">sharedSecret</span><span class="sxs-lookup"><span data-stu-id="174d9-118">sharedSecret</span></span>|<span data-ttu-id="174d9-119">2 </span><span class="sxs-lookup"><span data-stu-id="174d9-119">2</span></span>|<span data-ttu-id="174d9-120">Usar segredo compartilhado para autenticação.</span><span class="sxs-lookup"><span data-stu-id="174d9-120">Use Shared Secret for Authentication.</span></span>  <span data-ttu-id="174d9-121">Válido somente para iOS IKEv2.</span><span class="sxs-lookup"><span data-stu-id="174d9-121">Only valid for iOS IKEv2.</span></span>|
|<span data-ttu-id="174d9-122">derivedCredential</span><span class="sxs-lookup"><span data-stu-id="174d9-122">derivedCredential</span></span>|<span data-ttu-id="174d9-123">3 </span><span class="sxs-lookup"><span data-stu-id="174d9-123">3</span></span>|<span data-ttu-id="174d9-124">Use a credencial derivada para autenticação.</span><span class="sxs-lookup"><span data-stu-id="174d9-124">Use Derived Credential for Authentication.</span></span>|



