---
title: tipo de enumeração windowsInformationProtectionEnforcementLevel
description: Valores possíveis para níveis de imposição de proteção WIP
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 46488043220297617dfc4eb807d94ef2a9c0ba19
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527837"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a><span data-ttu-id="b6102-103">tipo de enumeração windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="b6102-103">windowsInformationProtectionEnforcementLevel enum type</span></span>

<span data-ttu-id="b6102-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b6102-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b6102-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b6102-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6102-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b6102-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6102-107">Valores possíveis para níveis de imposição de proteção WIP</span><span class="sxs-lookup"><span data-stu-id="b6102-107">Possible values for WIP Protection enforcement levels</span></span>

## <a name="members"></a><span data-ttu-id="b6102-108">Membros</span><span class="sxs-lookup"><span data-stu-id="b6102-108">Members</span></span>
|<span data-ttu-id="b6102-109">Membro</span><span class="sxs-lookup"><span data-stu-id="b6102-109">Member</span></span>|<span data-ttu-id="b6102-110">Valor</span><span class="sxs-lookup"><span data-stu-id="b6102-110">Value</span></span>|<span data-ttu-id="b6102-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6102-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6102-112">noprotection</span><span class="sxs-lookup"><span data-stu-id="b6102-112">noProtection</span></span>|<span data-ttu-id="b6102-113">,0</span><span class="sxs-lookup"><span data-stu-id="b6102-113">0</span></span>|<span data-ttu-id="b6102-114">Nenhuma imposição de proteção</span><span class="sxs-lookup"><span data-stu-id="b6102-114">No protection enforcement</span></span>|
|<span data-ttu-id="b6102-115">encryptAndAuditOnly</span><span class="sxs-lookup"><span data-stu-id="b6102-115">encryptAndAuditOnly</span></span>|<span data-ttu-id="b6102-116">1 </span><span class="sxs-lookup"><span data-stu-id="b6102-116">1</span></span>|<span data-ttu-id="b6102-117">Somente criptografia e auditoria</span><span class="sxs-lookup"><span data-stu-id="b6102-117">Encrypt and Audit only</span></span>|
|<span data-ttu-id="b6102-118">encryptAuditAndPrompt</span><span class="sxs-lookup"><span data-stu-id="b6102-118">encryptAuditAndPrompt</span></span>|<span data-ttu-id="b6102-119">2 </span><span class="sxs-lookup"><span data-stu-id="b6102-119">2</span></span>|<span data-ttu-id="b6102-120">Criptografar, auditar e solicitar</span><span class="sxs-lookup"><span data-stu-id="b6102-120">Encrypt, Audit and Prompt</span></span>|
|<span data-ttu-id="b6102-121">encryptAuditAndBlock</span><span class="sxs-lookup"><span data-stu-id="b6102-121">encryptAuditAndBlock</span></span>|<span data-ttu-id="b6102-122">3 </span><span class="sxs-lookup"><span data-stu-id="b6102-122">3</span></span>|<span data-ttu-id="b6102-123">Criptografar, auditar e bloquear</span><span class="sxs-lookup"><span data-stu-id="b6102-123">Encrypt, Audit and Block</span></span>|



