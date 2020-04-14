---
title: tipo de enumeração secureAssessmentAccountType
description: Tipo de contas permitidas para o Windows10SecureAssessment ConfigurationAccount.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 6eae52aade876f7097838b476c0865dba7986e68
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43444836"
---
# <a name="secureassessmentaccounttype-enum-type"></a><span data-ttu-id="c67ca-103">tipo de enumeração secureAssessmentAccountType</span><span class="sxs-lookup"><span data-stu-id="c67ca-103">secureAssessmentAccountType enum type</span></span>

<span data-ttu-id="c67ca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c67ca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c67ca-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c67ca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c67ca-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c67ca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c67ca-107">Tipo de contas permitidas para o Windows10SecureAssessment ConfigurationAccount.</span><span class="sxs-lookup"><span data-stu-id="c67ca-107">Type of accounts that are allowed for Windows10SecureAssessment ConfigurationAccount.</span></span>

## <a name="members"></a><span data-ttu-id="c67ca-108">Membros</span><span class="sxs-lookup"><span data-stu-id="c67ca-108">Members</span></span>
|<span data-ttu-id="c67ca-109">Membro</span><span class="sxs-lookup"><span data-stu-id="c67ca-109">Member</span></span>|<span data-ttu-id="c67ca-110">Valor</span><span class="sxs-lookup"><span data-stu-id="c67ca-110">Value</span></span>|<span data-ttu-id="c67ca-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c67ca-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c67ca-112">azureADAccount</span><span class="sxs-lookup"><span data-stu-id="c67ca-112">azureADAccount</span></span>|<span data-ttu-id="c67ca-113">,0</span><span class="sxs-lookup"><span data-stu-id="c67ca-113">0</span></span>|<span data-ttu-id="c67ca-114">Indica uma conta do Azure AD no formato AzureAD\username@tenant.com.</span><span class="sxs-lookup"><span data-stu-id="c67ca-114">Indicates an Azure AD account in format of AzureAD\username@tenant.com.</span></span>|
|<span data-ttu-id="c67ca-115">domainAccount</span><span class="sxs-lookup"><span data-stu-id="c67ca-115">domainAccount</span></span>|<span data-ttu-id="c67ca-116">1</span><span class="sxs-lookup"><span data-stu-id="c67ca-116">1</span></span>|<span data-ttu-id="c67ca-117">Indica uma conta de domínio no formato domínio \ usuário ou user@domain.com.</span><span class="sxs-lookup"><span data-stu-id="c67ca-117">Indicates a domain account in format of domain\user or user@domain.com.</span></span>|
|<span data-ttu-id="c67ca-118">localAccount</span><span class="sxs-lookup"><span data-stu-id="c67ca-118">localAccount</span></span>|<span data-ttu-id="c67ca-119">duas</span><span class="sxs-lookup"><span data-stu-id="c67ca-119">2</span></span>|<span data-ttu-id="c67ca-120">Indica uma conta local em formato de nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="c67ca-120">Indicates a local account in format of username.</span></span>|
|<span data-ttu-id="c67ca-121">localGuestAccount</span><span class="sxs-lookup"><span data-stu-id="c67ca-121">localGuestAccount</span></span>|<span data-ttu-id="c67ca-122">3D</span><span class="sxs-lookup"><span data-stu-id="c67ca-122">3</span></span>|<span data-ttu-id="c67ca-123">Indica uma conta de convidado local em formato de nome de teste.</span><span class="sxs-lookup"><span data-stu-id="c67ca-123">Indicates a local guest account in format of test name.</span></span>|



