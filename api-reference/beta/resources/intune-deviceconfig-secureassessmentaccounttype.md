---
title: tipo de enumeração secureAssessmentAccountType
description: Tipo de contas permitidas para o Windows10SecureAssessment ConfigurationAccount.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f1f7e2b6b9cbc32ee41840d96b706322660fd2b2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36000554"
---
# <a name="secureassessmentaccounttype-enum-type"></a><span data-ttu-id="9ba31-103">tipo de enumeração secureAssessmentAccountType</span><span class="sxs-lookup"><span data-stu-id="9ba31-103">secureAssessmentAccountType enum type</span></span>

> <span data-ttu-id="9ba31-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9ba31-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ba31-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9ba31-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ba31-106">Tipo de contas permitidas para o Windows10SecureAssessment ConfigurationAccount.</span><span class="sxs-lookup"><span data-stu-id="9ba31-106">Type of accounts that are allowed for Windows10SecureAssessment ConfigurationAccount.</span></span>

## <a name="members"></a><span data-ttu-id="9ba31-107">Membros</span><span class="sxs-lookup"><span data-stu-id="9ba31-107">Members</span></span>
|<span data-ttu-id="9ba31-108">Membro</span><span class="sxs-lookup"><span data-stu-id="9ba31-108">Member</span></span>|<span data-ttu-id="9ba31-109">Valor</span><span class="sxs-lookup"><span data-stu-id="9ba31-109">Value</span></span>|<span data-ttu-id="9ba31-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ba31-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ba31-111">azureADAccount</span><span class="sxs-lookup"><span data-stu-id="9ba31-111">azureADAccount</span></span>|<span data-ttu-id="9ba31-112">,0</span><span class="sxs-lookup"><span data-stu-id="9ba31-112">0</span></span>|<span data-ttu-id="9ba31-113">Indica uma conta do Azure AD no formato AzureAD\username@tenant.com.</span><span class="sxs-lookup"><span data-stu-id="9ba31-113">Indicates an Azure AD account in format of AzureAD\username@tenant.com.</span></span>|
|<span data-ttu-id="9ba31-114">domainAccount</span><span class="sxs-lookup"><span data-stu-id="9ba31-114">domainAccount</span></span>|<span data-ttu-id="9ba31-115">1</span><span class="sxs-lookup"><span data-stu-id="9ba31-115">1</span></span>|<span data-ttu-id="9ba31-116">Indica uma conta de domínio no formato domínio \ usuário ou user@domain.com.</span><span class="sxs-lookup"><span data-stu-id="9ba31-116">Indicates a domain account in format of domain\user or user@domain.com.</span></span>|
|<span data-ttu-id="9ba31-117">localAccount</span><span class="sxs-lookup"><span data-stu-id="9ba31-117">localAccount</span></span>|<span data-ttu-id="9ba31-118">duas</span><span class="sxs-lookup"><span data-stu-id="9ba31-118">2</span></span>|<span data-ttu-id="9ba31-119">Indica uma conta local em formato de nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="9ba31-119">Indicates a local account in format of username.</span></span>|
|<span data-ttu-id="9ba31-120">localGuestAccount</span><span class="sxs-lookup"><span data-stu-id="9ba31-120">localGuestAccount</span></span>|<span data-ttu-id="9ba31-121">3D</span><span class="sxs-lookup"><span data-stu-id="9ba31-121">3</span></span>|<span data-ttu-id="9ba31-122">Indica uma conta de convidado local em formato de nome de teste.</span><span class="sxs-lookup"><span data-stu-id="9ba31-122">Indicates a local guest account in format of test name.</span></span>|





