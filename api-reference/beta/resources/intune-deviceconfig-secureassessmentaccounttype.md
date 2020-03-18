---
title: tipo de enumeração secureAssessmentAccountType
description: Tipo de contas permitidas para o Windows10SecureAssessment ConfigurationAccount.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7a459e086b0b6ec44e625ca8a0932ea96422699a
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42787576"
---
# <a name="secureassessmentaccounttype-enum-type"></a><span data-ttu-id="09409-103">tipo de enumeração secureAssessmentAccountType</span><span class="sxs-lookup"><span data-stu-id="09409-103">secureAssessmentAccountType enum type</span></span>

> <span data-ttu-id="09409-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="09409-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09409-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="09409-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09409-106">Tipo de contas permitidas para o Windows10SecureAssessment ConfigurationAccount.</span><span class="sxs-lookup"><span data-stu-id="09409-106">Type of accounts that are allowed for Windows10SecureAssessment ConfigurationAccount.</span></span>

## <a name="members"></a><span data-ttu-id="09409-107">Membros</span><span class="sxs-lookup"><span data-stu-id="09409-107">Members</span></span>
|<span data-ttu-id="09409-108">Membro</span><span class="sxs-lookup"><span data-stu-id="09409-108">Member</span></span>|<span data-ttu-id="09409-109">Valor</span><span class="sxs-lookup"><span data-stu-id="09409-109">Value</span></span>|<span data-ttu-id="09409-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="09409-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09409-111">azureADAccount</span><span class="sxs-lookup"><span data-stu-id="09409-111">azureADAccount</span></span>|<span data-ttu-id="09409-112">,0</span><span class="sxs-lookup"><span data-stu-id="09409-112">0</span></span>|<span data-ttu-id="09409-113">Indica uma conta do Azure AD no formato AzureAD\username@tenant.com.</span><span class="sxs-lookup"><span data-stu-id="09409-113">Indicates an Azure AD account in format of AzureAD\username@tenant.com.</span></span>|
|<span data-ttu-id="09409-114">domainAccount</span><span class="sxs-lookup"><span data-stu-id="09409-114">domainAccount</span></span>|<span data-ttu-id="09409-115">1</span><span class="sxs-lookup"><span data-stu-id="09409-115">1</span></span>|<span data-ttu-id="09409-116">Indica uma conta de domínio no formato domínio \ usuário ou user@domain.com.</span><span class="sxs-lookup"><span data-stu-id="09409-116">Indicates a domain account in format of domain\user or user@domain.com.</span></span>|
|<span data-ttu-id="09409-117">localAccount</span><span class="sxs-lookup"><span data-stu-id="09409-117">localAccount</span></span>|<span data-ttu-id="09409-118">duas</span><span class="sxs-lookup"><span data-stu-id="09409-118">2</span></span>|<span data-ttu-id="09409-119">Indica uma conta local em formato de nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="09409-119">Indicates a local account in format of username.</span></span>|
|<span data-ttu-id="09409-120">localGuestAccount</span><span class="sxs-lookup"><span data-stu-id="09409-120">localGuestAccount</span></span>|<span data-ttu-id="09409-121">3D</span><span class="sxs-lookup"><span data-stu-id="09409-121">3</span></span>|<span data-ttu-id="09409-122">Indica uma conta de convidado local em formato de nome de teste.</span><span class="sxs-lookup"><span data-stu-id="09409-122">Indicates a local guest account in format of test name.</span></span>|



