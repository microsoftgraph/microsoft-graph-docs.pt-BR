---
title: tipo de enumeração keyStorageProviderOption
description: Opções de importação do KSP (provedor de armazenamento de chave).
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4013afe6f39decefec32cc3fe68f3236b43ee60f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092493"
---
# <a name="keystorageprovideroption-enum-type"></a><span data-ttu-id="3c431-103">tipo de enumeração keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="3c431-103">keyStorageProviderOption enum type</span></span>

<span data-ttu-id="3c431-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c431-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3c431-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3c431-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c431-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3c431-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c431-107">Opções de importação do KSP (provedor de armazenamento de chave).</span><span class="sxs-lookup"><span data-stu-id="3c431-107">Key Storage Provider (KSP) Import Options.</span></span>

## <a name="members"></a><span data-ttu-id="3c431-108">Membros</span><span class="sxs-lookup"><span data-stu-id="3c431-108">Members</span></span>
|<span data-ttu-id="3c431-109">Membro</span><span class="sxs-lookup"><span data-stu-id="3c431-109">Member</span></span>|<span data-ttu-id="3c431-110">Valor</span><span class="sxs-lookup"><span data-stu-id="3c431-110">Value</span></span>|<span data-ttu-id="3c431-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c431-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c431-112">useTpmKspOtherwiseUseSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="3c431-112">useTpmKspOtherwiseUseSoftwareKsp</span></span>|<span data-ttu-id="3c431-113">,0</span><span class="sxs-lookup"><span data-stu-id="3c431-113">0</span></span>|<span data-ttu-id="3c431-114">Importar para KSP de Trusted Platform Module (TPM) se presente, caso contrário, importe para o KSP de software.</span><span class="sxs-lookup"><span data-stu-id="3c431-114">Import to Trusted Platform Module (TPM) KSP if present, otherwise import to Software KSP.</span></span>|
|<span data-ttu-id="3c431-115">useTpmKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="3c431-115">useTpmKspOtherwiseFail</span></span>|<span data-ttu-id="3c431-116">1 </span><span class="sxs-lookup"><span data-stu-id="3c431-116">1</span></span>|<span data-ttu-id="3c431-117">Importar para KSP de Trusted Platform Module (TPM) se presente, caso contrário, falha.</span><span class="sxs-lookup"><span data-stu-id="3c431-117">Import to Trusted Platform Module (TPM) KSP if present, otherwise fail.</span></span>|
|<span data-ttu-id="3c431-118">usePassportForWorkKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="3c431-118">usePassportForWorkKspOtherwiseFail</span></span>|<span data-ttu-id="3c431-119">2 </span><span class="sxs-lookup"><span data-stu-id="3c431-119">2</span></span>|<span data-ttu-id="3c431-120">Importe para o Passport para trabalho do KSP, se disponível, caso contrário, falha.</span><span class="sxs-lookup"><span data-stu-id="3c431-120">Import to Passport for work KSP if available, otherwise fail.</span></span>|
|<span data-ttu-id="3c431-121">useSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="3c431-121">useSoftwareKsp</span></span>|<span data-ttu-id="3c431-122">3D</span><span class="sxs-lookup"><span data-stu-id="3c431-122">3</span></span>|<span data-ttu-id="3c431-123">Importar para KSP de software.</span><span class="sxs-lookup"><span data-stu-id="3c431-123">Import to Software KSP.</span></span>|






