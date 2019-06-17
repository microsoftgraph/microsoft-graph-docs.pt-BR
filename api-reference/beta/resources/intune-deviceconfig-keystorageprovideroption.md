---
title: tipo de enumeração keyStorageProviderOption
description: Opções de importação do KSP (provedor de armazenamento de chave).
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4ed06e011bbd9f64645541ded8929b0f2b5984fc
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34989424"
---
# <a name="keystorageprovideroption-enum-type"></a><span data-ttu-id="6bb9f-103">tipo de enumeração keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="6bb9f-103">keyStorageProviderOption enum type</span></span>

> <span data-ttu-id="6bb9f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6bb9f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6bb9f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6bb9f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6bb9f-106">Opções de importação do KSP (provedor de armazenamento de chave).</span><span class="sxs-lookup"><span data-stu-id="6bb9f-106">Key Storage Provider (KSP) Import Options.</span></span>

## <a name="members"></a><span data-ttu-id="6bb9f-107">Membros</span><span class="sxs-lookup"><span data-stu-id="6bb9f-107">Members</span></span>
|<span data-ttu-id="6bb9f-108">Membro</span><span class="sxs-lookup"><span data-stu-id="6bb9f-108">Member</span></span>|<span data-ttu-id="6bb9f-109">Valor</span><span class="sxs-lookup"><span data-stu-id="6bb9f-109">Value</span></span>|<span data-ttu-id="6bb9f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6bb9f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bb9f-111">useTpmKspOtherwiseUseSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="6bb9f-111">useTpmKspOtherwiseUseSoftwareKsp</span></span>|<span data-ttu-id="6bb9f-112">,0</span><span class="sxs-lookup"><span data-stu-id="6bb9f-112">0</span></span>|<span data-ttu-id="6bb9f-113">Importar para KSP de Trusted Platform Module (TPM) se presente, caso contrário, importe para o KSP de software.</span><span class="sxs-lookup"><span data-stu-id="6bb9f-113">Import to Trusted Platform Module (TPM) KSP if present, otherwise import to Software KSP.</span></span>|
|<span data-ttu-id="6bb9f-114">useTpmKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="6bb9f-114">useTpmKspOtherwiseFail</span></span>|<span data-ttu-id="6bb9f-115">1</span><span class="sxs-lookup"><span data-stu-id="6bb9f-115">1</span></span>|<span data-ttu-id="6bb9f-116">Importar para KSP de Trusted Platform Module (TPM) se presente, caso contrário, falha.</span><span class="sxs-lookup"><span data-stu-id="6bb9f-116">Import to Trusted Platform Module (TPM) KSP if present, otherwise fail.</span></span>|
|<span data-ttu-id="6bb9f-117">usePassportForWorkKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="6bb9f-117">usePassportForWorkKspOtherwiseFail</span></span>|<span data-ttu-id="6bb9f-118">duas</span><span class="sxs-lookup"><span data-stu-id="6bb9f-118">2</span></span>|<span data-ttu-id="6bb9f-119">Importe para o Passport para trabalho do KSP, se disponível, caso contrário, falha.</span><span class="sxs-lookup"><span data-stu-id="6bb9f-119">Import to Passport for work KSP if available, otherwise fail.</span></span>|
|<span data-ttu-id="6bb9f-120">useSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="6bb9f-120">useSoftwareKsp</span></span>|<span data-ttu-id="6bb9f-121">3D</span><span class="sxs-lookup"><span data-stu-id="6bb9f-121">3</span></span>|<span data-ttu-id="6bb9f-122">Importar para KSP de software.</span><span class="sxs-lookup"><span data-stu-id="6bb9f-122">Import to Software KSP.</span></span>|





