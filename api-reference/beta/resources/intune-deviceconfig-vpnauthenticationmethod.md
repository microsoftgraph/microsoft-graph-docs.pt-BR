---
title: tipo de enumeração vpnAuthenticationMethod
description: Método de autenticação VPN.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 300243146175c4884c8f8f44691ba02fa796210c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049153"
---
# <a name="vpnauthenticationmethod-enum-type"></a><span data-ttu-id="48cf7-103">tipo de enumeração vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="48cf7-103">vpnAuthenticationMethod enum type</span></span>

<span data-ttu-id="48cf7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48cf7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="48cf7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="48cf7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="48cf7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="48cf7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48cf7-107">Método de autenticação VPN.</span><span class="sxs-lookup"><span data-stu-id="48cf7-107">VPN Authentication Method.</span></span>

## <a name="members"></a><span data-ttu-id="48cf7-108">Membros</span><span class="sxs-lookup"><span data-stu-id="48cf7-108">Members</span></span>
|<span data-ttu-id="48cf7-109">Membro</span><span class="sxs-lookup"><span data-stu-id="48cf7-109">Member</span></span>|<span data-ttu-id="48cf7-110">Valor</span><span class="sxs-lookup"><span data-stu-id="48cf7-110">Value</span></span>|<span data-ttu-id="48cf7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="48cf7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48cf7-112">certificado</span><span class="sxs-lookup"><span data-stu-id="48cf7-112">certificate</span></span>|<span data-ttu-id="48cf7-113">,0</span><span class="sxs-lookup"><span data-stu-id="48cf7-113">0</span></span>|<span data-ttu-id="48cf7-114">Autenticar com um certificado.</span><span class="sxs-lookup"><span data-stu-id="48cf7-114">Authenticate with a certificate.</span></span>|
|<span data-ttu-id="48cf7-115">usernameAndPassword</span><span class="sxs-lookup"><span data-stu-id="48cf7-115">usernameAndPassword</span></span>|<span data-ttu-id="48cf7-116">1 </span><span class="sxs-lookup"><span data-stu-id="48cf7-116">1</span></span>|<span data-ttu-id="48cf7-117">Usar nome de usuário e senha para autenticação.</span><span class="sxs-lookup"><span data-stu-id="48cf7-117">Use username and password for authentication.</span></span>|
|<span data-ttu-id="48cf7-118">sharedSecret</span><span class="sxs-lookup"><span data-stu-id="48cf7-118">sharedSecret</span></span>|<span data-ttu-id="48cf7-119">2 </span><span class="sxs-lookup"><span data-stu-id="48cf7-119">2</span></span>|<span data-ttu-id="48cf7-120">Usar segredo compartilhado para autenticação.</span><span class="sxs-lookup"><span data-stu-id="48cf7-120">Use Shared Secret for Authentication.</span></span>  <span data-ttu-id="48cf7-121">Válido somente para iOS IKEv2.</span><span class="sxs-lookup"><span data-stu-id="48cf7-121">Only valid for iOS IKEv2.</span></span>|
|<span data-ttu-id="48cf7-122">derivedCredential</span><span class="sxs-lookup"><span data-stu-id="48cf7-122">derivedCredential</span></span>|<span data-ttu-id="48cf7-123">3 </span><span class="sxs-lookup"><span data-stu-id="48cf7-123">3</span></span>|<span data-ttu-id="48cf7-124">Use a credencial derivada para autenticação.</span><span class="sxs-lookup"><span data-stu-id="48cf7-124">Use Derived Credential for Authentication.</span></span>|
|<span data-ttu-id="48cf7-125">azureAD</span><span class="sxs-lookup"><span data-stu-id="48cf7-125">azureAD</span></span>|<span data-ttu-id="48cf7-126">4 </span><span class="sxs-lookup"><span data-stu-id="48cf7-126">4</span></span>|<span data-ttu-id="48cf7-127">Usar o Azure AD para autenticação.</span><span class="sxs-lookup"><span data-stu-id="48cf7-127">Use Azure AD for authentication.</span></span>|






