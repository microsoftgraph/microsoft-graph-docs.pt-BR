---
title: tipo de enumeração vpnAuthenticationMethod
description: Método de autenticação VPN.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: dd3cc6887f5434df00a2ed9a817c0ca79c8c880e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43412448"
---
# <a name="vpnauthenticationmethod-enum-type"></a><span data-ttu-id="cbb3b-103">tipo de enumeração vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="cbb3b-103">vpnAuthenticationMethod enum type</span></span>

<span data-ttu-id="cbb3b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cbb3b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cbb3b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cbb3b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cbb3b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cbb3b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cbb3b-107">Método de autenticação VPN.</span><span class="sxs-lookup"><span data-stu-id="cbb3b-107">VPN Authentication Method.</span></span>

## <a name="members"></a><span data-ttu-id="cbb3b-108">Membros</span><span class="sxs-lookup"><span data-stu-id="cbb3b-108">Members</span></span>
|<span data-ttu-id="cbb3b-109">Membro</span><span class="sxs-lookup"><span data-stu-id="cbb3b-109">Member</span></span>|<span data-ttu-id="cbb3b-110">Valor</span><span class="sxs-lookup"><span data-stu-id="cbb3b-110">Value</span></span>|<span data-ttu-id="cbb3b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="cbb3b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cbb3b-112">certificado</span><span class="sxs-lookup"><span data-stu-id="cbb3b-112">certificate</span></span>|<span data-ttu-id="cbb3b-113">,0</span><span class="sxs-lookup"><span data-stu-id="cbb3b-113">0</span></span>|<span data-ttu-id="cbb3b-114">Autenticar com um certificado.</span><span class="sxs-lookup"><span data-stu-id="cbb3b-114">Authenticate with a certificate.</span></span>|
|<span data-ttu-id="cbb3b-115">usernameAndPassword</span><span class="sxs-lookup"><span data-stu-id="cbb3b-115">usernameAndPassword</span></span>|<span data-ttu-id="cbb3b-116">1</span><span class="sxs-lookup"><span data-stu-id="cbb3b-116">1</span></span>|<span data-ttu-id="cbb3b-117">Usar nome de usuário e senha para autenticação.</span><span class="sxs-lookup"><span data-stu-id="cbb3b-117">Use username and password for authentication.</span></span>|
|<span data-ttu-id="cbb3b-118">sharedSecret</span><span class="sxs-lookup"><span data-stu-id="cbb3b-118">sharedSecret</span></span>|<span data-ttu-id="cbb3b-119">duas</span><span class="sxs-lookup"><span data-stu-id="cbb3b-119">2</span></span>|<span data-ttu-id="cbb3b-120">Usar segredo compartilhado para autenticação.</span><span class="sxs-lookup"><span data-stu-id="cbb3b-120">Use Shared Secret for Authentication.</span></span>  <span data-ttu-id="cbb3b-121">Válido somente para iOS IKEv2.</span><span class="sxs-lookup"><span data-stu-id="cbb3b-121">Only valid for iOS IKEv2.</span></span>|
|<span data-ttu-id="cbb3b-122">derivedCredential</span><span class="sxs-lookup"><span data-stu-id="cbb3b-122">derivedCredential</span></span>|<span data-ttu-id="cbb3b-123">3D</span><span class="sxs-lookup"><span data-stu-id="cbb3b-123">3</span></span>|<span data-ttu-id="cbb3b-124">Use a credencial derivada para autenticação.</span><span class="sxs-lookup"><span data-stu-id="cbb3b-124">Use Derived Credential for Authentication.</span></span>|



