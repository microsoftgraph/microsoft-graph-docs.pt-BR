---
title: tipo de enumeração vpnAuthenticationMethod
description: Método de autenticação VPN.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ad3ff24cc902a943fd9c146310d58cd1f1bfbd8d
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38088116"
---
# <a name="vpnauthenticationmethod-enum-type"></a><span data-ttu-id="9c66a-103">tipo de enumeração vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="9c66a-103">vpnAuthenticationMethod enum type</span></span>

> <span data-ttu-id="9c66a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9c66a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c66a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9c66a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c66a-106">Método de autenticação VPN.</span><span class="sxs-lookup"><span data-stu-id="9c66a-106">VPN Authentication Method.</span></span>

## <a name="members"></a><span data-ttu-id="9c66a-107">Membros</span><span class="sxs-lookup"><span data-stu-id="9c66a-107">Members</span></span>
|<span data-ttu-id="9c66a-108">Membro</span><span class="sxs-lookup"><span data-stu-id="9c66a-108">Member</span></span>|<span data-ttu-id="9c66a-109">Valor</span><span class="sxs-lookup"><span data-stu-id="9c66a-109">Value</span></span>|<span data-ttu-id="9c66a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c66a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c66a-111">certificado</span><span class="sxs-lookup"><span data-stu-id="9c66a-111">certificate</span></span>|<span data-ttu-id="9c66a-112">,0</span><span class="sxs-lookup"><span data-stu-id="9c66a-112">0</span></span>|<span data-ttu-id="9c66a-113">Autenticar com um certificado.</span><span class="sxs-lookup"><span data-stu-id="9c66a-113">Authenticate with a certificate.</span></span>|
|<span data-ttu-id="9c66a-114">usernameAndPassword</span><span class="sxs-lookup"><span data-stu-id="9c66a-114">usernameAndPassword</span></span>|<span data-ttu-id="9c66a-115">1</span><span class="sxs-lookup"><span data-stu-id="9c66a-115">1</span></span>|<span data-ttu-id="9c66a-116">Usar nome de usuário e senha para autenticação.</span><span class="sxs-lookup"><span data-stu-id="9c66a-116">Use username and password for authentication.</span></span>|
|<span data-ttu-id="9c66a-117">sharedSecret</span><span class="sxs-lookup"><span data-stu-id="9c66a-117">sharedSecret</span></span>|<span data-ttu-id="9c66a-118">duas</span><span class="sxs-lookup"><span data-stu-id="9c66a-118">2</span></span>|<span data-ttu-id="9c66a-119">Usar segredo compartilhado para autenticação.</span><span class="sxs-lookup"><span data-stu-id="9c66a-119">Use Shared Secret for Authentication.</span></span>  <span data-ttu-id="9c66a-120">Válido somente para iOS IKEv2.</span><span class="sxs-lookup"><span data-stu-id="9c66a-120">Only valid for iOS IKEv2.</span></span>|
|<span data-ttu-id="9c66a-121">derivedCredential</span><span class="sxs-lookup"><span data-stu-id="9c66a-121">derivedCredential</span></span>|<span data-ttu-id="9c66a-122">3D</span><span class="sxs-lookup"><span data-stu-id="9c66a-122">3</span></span>|<span data-ttu-id="9c66a-123">Use a credencial derivada para autenticação.</span><span class="sxs-lookup"><span data-stu-id="9c66a-123">Use Derived Credential for Authentication.</span></span>|



