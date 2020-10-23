---
title: tipo de enumeração secureAssessmentAccountType
description: Tipo de contas permitidas para o Windows10SecureAssessment ConfigurationAccount.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ff6c3bf31b1fbe390bb53d4166c961dd2bcef3e4
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48709933"
---
# <a name="secureassessmentaccounttype-enum-type"></a><span data-ttu-id="67ff9-103">tipo de enumeração secureAssessmentAccountType</span><span class="sxs-lookup"><span data-stu-id="67ff9-103">secureAssessmentAccountType enum type</span></span>

<span data-ttu-id="67ff9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67ff9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="67ff9-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="67ff9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67ff9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="67ff9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67ff9-107">Tipo de contas permitidas para o Windows10SecureAssessment ConfigurationAccount.</span><span class="sxs-lookup"><span data-stu-id="67ff9-107">Type of accounts that are allowed for Windows10SecureAssessment ConfigurationAccount.</span></span>

## <a name="members"></a><span data-ttu-id="67ff9-108">Membros</span><span class="sxs-lookup"><span data-stu-id="67ff9-108">Members</span></span>
|<span data-ttu-id="67ff9-109">Membro</span><span class="sxs-lookup"><span data-stu-id="67ff9-109">Member</span></span>|<span data-ttu-id="67ff9-110">Valor</span><span class="sxs-lookup"><span data-stu-id="67ff9-110">Value</span></span>|<span data-ttu-id="67ff9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="67ff9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67ff9-112">azureADAccount</span><span class="sxs-lookup"><span data-stu-id="67ff9-112">azureADAccount</span></span>|<span data-ttu-id="67ff9-113">,0</span><span class="sxs-lookup"><span data-stu-id="67ff9-113">0</span></span>|<span data-ttu-id="67ff9-114">Indica uma conta do Azure AD no formato AzureAD\username@tenant.com.</span><span class="sxs-lookup"><span data-stu-id="67ff9-114">Indicates an Azure AD account in format of AzureAD\username@tenant.com.</span></span>|
|<span data-ttu-id="67ff9-115">domainAccount</span><span class="sxs-lookup"><span data-stu-id="67ff9-115">domainAccount</span></span>|<span data-ttu-id="67ff9-116">1</span><span class="sxs-lookup"><span data-stu-id="67ff9-116">1</span></span>|<span data-ttu-id="67ff9-117">Indica uma conta de domínio no formato domínio \ usuário ou user@domain.com.</span><span class="sxs-lookup"><span data-stu-id="67ff9-117">Indicates a domain account in format of domain\user or user@domain.com.</span></span>|
|<span data-ttu-id="67ff9-118">localAccount</span><span class="sxs-lookup"><span data-stu-id="67ff9-118">localAccount</span></span>|<span data-ttu-id="67ff9-119">duas</span><span class="sxs-lookup"><span data-stu-id="67ff9-119">2</span></span>|<span data-ttu-id="67ff9-120">Indica uma conta local em formato de nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="67ff9-120">Indicates a local account in format of username.</span></span>|
|<span data-ttu-id="67ff9-121">localGuestAccount</span><span class="sxs-lookup"><span data-stu-id="67ff9-121">localGuestAccount</span></span>|<span data-ttu-id="67ff9-122">3D</span><span class="sxs-lookup"><span data-stu-id="67ff9-122">3</span></span>|<span data-ttu-id="67ff9-123">Indica uma conta de convidado local em formato de nome de teste.</span><span class="sxs-lookup"><span data-stu-id="67ff9-123">Indicates a local guest account in format of test name.</span></span>|





