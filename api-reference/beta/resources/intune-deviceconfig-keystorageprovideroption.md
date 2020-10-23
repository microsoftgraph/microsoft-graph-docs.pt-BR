---
title: tipo de enumeração keyStorageProviderOption
description: Opções de importação do KSP (provedor de armazenamento de chave).
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 2c97c592f7e7f3a3d2a154d24dc4c331ba62c5b1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48697928"
---
# <a name="keystorageprovideroption-enum-type"></a><span data-ttu-id="56640-103">tipo de enumeração keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="56640-103">keyStorageProviderOption enum type</span></span>

<span data-ttu-id="56640-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56640-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="56640-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="56640-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="56640-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="56640-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56640-107">Opções de importação do KSP (provedor de armazenamento de chave).</span><span class="sxs-lookup"><span data-stu-id="56640-107">Key Storage Provider (KSP) Import Options.</span></span>

## <a name="members"></a><span data-ttu-id="56640-108">Membros</span><span class="sxs-lookup"><span data-stu-id="56640-108">Members</span></span>
|<span data-ttu-id="56640-109">Membro</span><span class="sxs-lookup"><span data-stu-id="56640-109">Member</span></span>|<span data-ttu-id="56640-110">Valor</span><span class="sxs-lookup"><span data-stu-id="56640-110">Value</span></span>|<span data-ttu-id="56640-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="56640-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56640-112">useTpmKspOtherwiseUseSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="56640-112">useTpmKspOtherwiseUseSoftwareKsp</span></span>|<span data-ttu-id="56640-113">,0</span><span class="sxs-lookup"><span data-stu-id="56640-113">0</span></span>|<span data-ttu-id="56640-114">Importar para KSP de Trusted Platform Module (TPM) se presente, caso contrário, importe para o KSP de software.</span><span class="sxs-lookup"><span data-stu-id="56640-114">Import to Trusted Platform Module (TPM) KSP if present, otherwise import to Software KSP.</span></span>|
|<span data-ttu-id="56640-115">useTpmKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="56640-115">useTpmKspOtherwiseFail</span></span>|<span data-ttu-id="56640-116">1</span><span class="sxs-lookup"><span data-stu-id="56640-116">1</span></span>|<span data-ttu-id="56640-117">Importar para KSP de Trusted Platform Module (TPM) se presente, caso contrário, falha.</span><span class="sxs-lookup"><span data-stu-id="56640-117">Import to Trusted Platform Module (TPM) KSP if present, otherwise fail.</span></span>|
|<span data-ttu-id="56640-118">usePassportForWorkKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="56640-118">usePassportForWorkKspOtherwiseFail</span></span>|<span data-ttu-id="56640-119">duas</span><span class="sxs-lookup"><span data-stu-id="56640-119">2</span></span>|<span data-ttu-id="56640-120">Importe para o Passport para trabalho do KSP, se disponível, caso contrário, falha.</span><span class="sxs-lookup"><span data-stu-id="56640-120">Import to Passport for work KSP if available, otherwise fail.</span></span>|
|<span data-ttu-id="56640-121">useSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="56640-121">useSoftwareKsp</span></span>|<span data-ttu-id="56640-122">3D</span><span class="sxs-lookup"><span data-stu-id="56640-122">3</span></span>|<span data-ttu-id="56640-123">Importar para KSP de software.</span><span class="sxs-lookup"><span data-stu-id="56640-123">Import to Software KSP.</span></span>|





