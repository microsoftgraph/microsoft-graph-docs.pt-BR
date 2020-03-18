---
title: tipo de enumeração vpnAuthenticationMethod
description: Método de autenticação VPN.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 048b31bd835c1e94d3afcef87b6bd8e93f3ddeec
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42787415"
---
# <a name="vpnauthenticationmethod-enum-type"></a><span data-ttu-id="aa056-103">tipo de enumeração vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="aa056-103">vpnAuthenticationMethod enum type</span></span>

> <span data-ttu-id="aa056-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="aa056-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aa056-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="aa056-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa056-106">Método de autenticação VPN.</span><span class="sxs-lookup"><span data-stu-id="aa056-106">VPN Authentication Method.</span></span>

## <a name="members"></a><span data-ttu-id="aa056-107">Membros</span><span class="sxs-lookup"><span data-stu-id="aa056-107">Members</span></span>
|<span data-ttu-id="aa056-108">Membro</span><span class="sxs-lookup"><span data-stu-id="aa056-108">Member</span></span>|<span data-ttu-id="aa056-109">Valor</span><span class="sxs-lookup"><span data-stu-id="aa056-109">Value</span></span>|<span data-ttu-id="aa056-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa056-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa056-111">certificado</span><span class="sxs-lookup"><span data-stu-id="aa056-111">certificate</span></span>|<span data-ttu-id="aa056-112">,0</span><span class="sxs-lookup"><span data-stu-id="aa056-112">0</span></span>|<span data-ttu-id="aa056-113">Autenticar com um certificado.</span><span class="sxs-lookup"><span data-stu-id="aa056-113">Authenticate with a certificate.</span></span>|
|<span data-ttu-id="aa056-114">usernameAndPassword</span><span class="sxs-lookup"><span data-stu-id="aa056-114">usernameAndPassword</span></span>|<span data-ttu-id="aa056-115">1</span><span class="sxs-lookup"><span data-stu-id="aa056-115">1</span></span>|<span data-ttu-id="aa056-116">Usar nome de usuário e senha para autenticação.</span><span class="sxs-lookup"><span data-stu-id="aa056-116">Use username and password for authentication.</span></span>|
|<span data-ttu-id="aa056-117">sharedSecret</span><span class="sxs-lookup"><span data-stu-id="aa056-117">sharedSecret</span></span>|<span data-ttu-id="aa056-118">duas</span><span class="sxs-lookup"><span data-stu-id="aa056-118">2</span></span>|<span data-ttu-id="aa056-119">Usar segredo compartilhado para autenticação.</span><span class="sxs-lookup"><span data-stu-id="aa056-119">Use Shared Secret for Authentication.</span></span>  <span data-ttu-id="aa056-120">Válido somente para iOS IKEv2.</span><span class="sxs-lookup"><span data-stu-id="aa056-120">Only valid for iOS IKEv2.</span></span>|
|<span data-ttu-id="aa056-121">derivedCredential</span><span class="sxs-lookup"><span data-stu-id="aa056-121">derivedCredential</span></span>|<span data-ttu-id="aa056-122">3D</span><span class="sxs-lookup"><span data-stu-id="aa056-122">3</span></span>|<span data-ttu-id="aa056-123">Use a credencial derivada para autenticação.</span><span class="sxs-lookup"><span data-stu-id="aa056-123">Use Derived Credential for Authentication.</span></span>|



