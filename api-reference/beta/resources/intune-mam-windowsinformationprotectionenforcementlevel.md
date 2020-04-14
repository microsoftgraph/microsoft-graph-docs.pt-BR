---
title: tipo de enumeração windowsInformationProtectionEnforcementLevel
description: Valores possíveis para níveis de imposição de proteção WIP
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: cf07d4023b979b213165b6665f6d8dc65d45b66d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43443694"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a><span data-ttu-id="e4462-103">tipo de enumeração windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="e4462-103">windowsInformationProtectionEnforcementLevel enum type</span></span>

<span data-ttu-id="e4462-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4462-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e4462-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e4462-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4462-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e4462-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4462-107">Valores possíveis para níveis de imposição de proteção WIP</span><span class="sxs-lookup"><span data-stu-id="e4462-107">Possible values for WIP Protection enforcement levels</span></span>

## <a name="members"></a><span data-ttu-id="e4462-108">Membros</span><span class="sxs-lookup"><span data-stu-id="e4462-108">Members</span></span>
|<span data-ttu-id="e4462-109">Membro</span><span class="sxs-lookup"><span data-stu-id="e4462-109">Member</span></span>|<span data-ttu-id="e4462-110">Valor</span><span class="sxs-lookup"><span data-stu-id="e4462-110">Value</span></span>|<span data-ttu-id="e4462-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4462-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4462-112">noprotection</span><span class="sxs-lookup"><span data-stu-id="e4462-112">noProtection</span></span>|<span data-ttu-id="e4462-113">,0</span><span class="sxs-lookup"><span data-stu-id="e4462-113">0</span></span>|<span data-ttu-id="e4462-114">Nenhuma imposição de proteção</span><span class="sxs-lookup"><span data-stu-id="e4462-114">No protection enforcement</span></span>|
|<span data-ttu-id="e4462-115">encryptAndAuditOnly</span><span class="sxs-lookup"><span data-stu-id="e4462-115">encryptAndAuditOnly</span></span>|<span data-ttu-id="e4462-116">1</span><span class="sxs-lookup"><span data-stu-id="e4462-116">1</span></span>|<span data-ttu-id="e4462-117">Somente criptografia e auditoria</span><span class="sxs-lookup"><span data-stu-id="e4462-117">Encrypt and Audit only</span></span>|
|<span data-ttu-id="e4462-118">encryptAuditAndPrompt</span><span class="sxs-lookup"><span data-stu-id="e4462-118">encryptAuditAndPrompt</span></span>|<span data-ttu-id="e4462-119">duas</span><span class="sxs-lookup"><span data-stu-id="e4462-119">2</span></span>|<span data-ttu-id="e4462-120">Criptografar, auditar e solicitar</span><span class="sxs-lookup"><span data-stu-id="e4462-120">Encrypt, Audit and Prompt</span></span>|
|<span data-ttu-id="e4462-121">encryptAuditAndBlock</span><span class="sxs-lookup"><span data-stu-id="e4462-121">encryptAuditAndBlock</span></span>|<span data-ttu-id="e4462-122">3D</span><span class="sxs-lookup"><span data-stu-id="e4462-122">3</span></span>|<span data-ttu-id="e4462-123">Criptografar, auditar e bloquear</span><span class="sxs-lookup"><span data-stu-id="e4462-123">Encrypt, Audit and Block</span></span>|



