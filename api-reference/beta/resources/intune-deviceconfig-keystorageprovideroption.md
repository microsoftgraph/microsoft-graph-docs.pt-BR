---
title: tipo de enumeração keyStorageProviderOption
description: Opções de importação do KSP (provedor de armazenamento de chave).
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: a2612aeb2cded950023a14136b71a8c7a55555a9
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42790409"
---
# <a name="keystorageprovideroption-enum-type"></a><span data-ttu-id="f4e8c-103">tipo de enumeração keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="f4e8c-103">keyStorageProviderOption enum type</span></span>

> <span data-ttu-id="f4e8c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f4e8c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4e8c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f4e8c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4e8c-106">Opções de importação do KSP (provedor de armazenamento de chave).</span><span class="sxs-lookup"><span data-stu-id="f4e8c-106">Key Storage Provider (KSP) Import Options.</span></span>

## <a name="members"></a><span data-ttu-id="f4e8c-107">Membros</span><span class="sxs-lookup"><span data-stu-id="f4e8c-107">Members</span></span>
|<span data-ttu-id="f4e8c-108">Membro</span><span class="sxs-lookup"><span data-stu-id="f4e8c-108">Member</span></span>|<span data-ttu-id="f4e8c-109">Valor</span><span class="sxs-lookup"><span data-stu-id="f4e8c-109">Value</span></span>|<span data-ttu-id="f4e8c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4e8c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4e8c-111">useTpmKspOtherwiseUseSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="f4e8c-111">useTpmKspOtherwiseUseSoftwareKsp</span></span>|<span data-ttu-id="f4e8c-112">,0</span><span class="sxs-lookup"><span data-stu-id="f4e8c-112">0</span></span>|<span data-ttu-id="f4e8c-113">Importar para KSP de Trusted Platform Module (TPM) se presente, caso contrário, importe para o KSP de software.</span><span class="sxs-lookup"><span data-stu-id="f4e8c-113">Import to Trusted Platform Module (TPM) KSP if present, otherwise import to Software KSP.</span></span>|
|<span data-ttu-id="f4e8c-114">useTpmKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="f4e8c-114">useTpmKspOtherwiseFail</span></span>|<span data-ttu-id="f4e8c-115">1</span><span class="sxs-lookup"><span data-stu-id="f4e8c-115">1</span></span>|<span data-ttu-id="f4e8c-116">Importar para KSP de Trusted Platform Module (TPM) se presente, caso contrário, falha.</span><span class="sxs-lookup"><span data-stu-id="f4e8c-116">Import to Trusted Platform Module (TPM) KSP if present, otherwise fail.</span></span>|
|<span data-ttu-id="f4e8c-117">usePassportForWorkKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="f4e8c-117">usePassportForWorkKspOtherwiseFail</span></span>|<span data-ttu-id="f4e8c-118">duas</span><span class="sxs-lookup"><span data-stu-id="f4e8c-118">2</span></span>|<span data-ttu-id="f4e8c-119">Importe para o Passport para trabalho do KSP, se disponível, caso contrário, falha.</span><span class="sxs-lookup"><span data-stu-id="f4e8c-119">Import to Passport for work KSP if available, otherwise fail.</span></span>|
|<span data-ttu-id="f4e8c-120">useSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="f4e8c-120">useSoftwareKsp</span></span>|<span data-ttu-id="f4e8c-121">3D</span><span class="sxs-lookup"><span data-stu-id="f4e8c-121">3</span></span>|<span data-ttu-id="f4e8c-122">Importar para KSP de software.</span><span class="sxs-lookup"><span data-stu-id="f4e8c-122">Import to Software KSP.</span></span>|



