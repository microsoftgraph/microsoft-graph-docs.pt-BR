---
title: tipo de enum windowsInformationProtectionEnforcementLevel
description: Valores possíveis para níveis de imposição de proteção de WIP
author: tfitzmac
ms.openlocfilehash: cb30ffb58b129fc302d7896c148072a54b98c0a2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315159"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a><span data-ttu-id="b1e32-103">tipo de enum windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="b1e32-103">windowsInformationProtectionEnforcementLevel enum type</span></span>

> <span data-ttu-id="b1e32-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b1e32-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b1e32-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b1e32-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b1e32-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b1e32-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b1e32-107">Valores possíveis para níveis de imposição de proteção de WIP</span><span class="sxs-lookup"><span data-stu-id="b1e32-107">Possible values for WIP Protection enforcement levels</span></span>
## <a name="members"></a><span data-ttu-id="b1e32-108">Membros</span><span class="sxs-lookup"><span data-stu-id="b1e32-108">Members</span></span>
|<span data-ttu-id="b1e32-109">Membro</span><span class="sxs-lookup"><span data-stu-id="b1e32-109">Member</span></span>|<span data-ttu-id="b1e32-110">Valor</span><span class="sxs-lookup"><span data-stu-id="b1e32-110">Value</span></span>|<span data-ttu-id="b1e32-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1e32-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1e32-112">noProtection</span><span class="sxs-lookup"><span data-stu-id="b1e32-112">noProtection</span></span>|<span data-ttu-id="b1e32-113">0</span><span class="sxs-lookup"><span data-stu-id="b1e32-113">0</span></span>|<span data-ttu-id="b1e32-114">Nenhuma imposição de proteção</span><span class="sxs-lookup"><span data-stu-id="b1e32-114">No protection enforcement</span></span>|
|<span data-ttu-id="b1e32-115">encryptAndAuditOnly</span><span class="sxs-lookup"><span data-stu-id="b1e32-115">encryptAndAuditOnly</span></span>|<span data-ttu-id="b1e32-116">1</span><span class="sxs-lookup"><span data-stu-id="b1e32-116">1</span></span>|<span data-ttu-id="b1e32-117">Criptografar e auditoria somente</span><span class="sxs-lookup"><span data-stu-id="b1e32-117">Encrypt and Audit only</span></span>|
|<span data-ttu-id="b1e32-118">encryptAuditAndPrompt</span><span class="sxs-lookup"><span data-stu-id="b1e32-118">encryptAuditAndPrompt</span></span>|<span data-ttu-id="b1e32-119">2</span><span class="sxs-lookup"><span data-stu-id="b1e32-119">2</span></span>|<span data-ttu-id="b1e32-120">Criptografar, auditoria e solicitar</span><span class="sxs-lookup"><span data-stu-id="b1e32-120">Encrypt, Audit and Prompt</span></span>|
|<span data-ttu-id="b1e32-121">encryptAuditAndBlock</span><span class="sxs-lookup"><span data-stu-id="b1e32-121">encryptAuditAndBlock</span></span>|<span data-ttu-id="b1e32-122">3</span><span class="sxs-lookup"><span data-stu-id="b1e32-122">3</span></span>|<span data-ttu-id="b1e32-123">Criptografar, auditoria e bloquear</span><span class="sxs-lookup"><span data-stu-id="b1e32-123">Encrypt, Audit and Block</span></span>|





