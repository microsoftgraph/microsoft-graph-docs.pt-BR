---
title: tipo de enumeração keyStorageProviderOption
description: Opções de importação do KSP (provedor de armazenamento de chave).
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8580688edbdacb150a37ee5cf2a52fdc77dd490f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526252"
---
# <a name="keystorageprovideroption-enum-type"></a><span data-ttu-id="c334f-103">tipo de enumeração keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="c334f-103">keyStorageProviderOption enum type</span></span>

<span data-ttu-id="c334f-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c334f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c334f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c334f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c334f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c334f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c334f-107">Opções de importação do KSP (provedor de armazenamento de chave).</span><span class="sxs-lookup"><span data-stu-id="c334f-107">Key Storage Provider (KSP) Import Options.</span></span>

## <a name="members"></a><span data-ttu-id="c334f-108">Membros</span><span class="sxs-lookup"><span data-stu-id="c334f-108">Members</span></span>
|<span data-ttu-id="c334f-109">Membro</span><span class="sxs-lookup"><span data-stu-id="c334f-109">Member</span></span>|<span data-ttu-id="c334f-110">Valor</span><span class="sxs-lookup"><span data-stu-id="c334f-110">Value</span></span>|<span data-ttu-id="c334f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c334f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c334f-112">useTpmKspOtherwiseUseSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="c334f-112">useTpmKspOtherwiseUseSoftwareKsp</span></span>|<span data-ttu-id="c334f-113">,0</span><span class="sxs-lookup"><span data-stu-id="c334f-113">0</span></span>|<span data-ttu-id="c334f-114">Importar para KSP de Trusted Platform Module (TPM) se presente, caso contrário, importe para o KSP de software.</span><span class="sxs-lookup"><span data-stu-id="c334f-114">Import to Trusted Platform Module (TPM) KSP if present, otherwise import to Software KSP.</span></span>|
|<span data-ttu-id="c334f-115">useTpmKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="c334f-115">useTpmKspOtherwiseFail</span></span>|<span data-ttu-id="c334f-116">1 </span><span class="sxs-lookup"><span data-stu-id="c334f-116">1</span></span>|<span data-ttu-id="c334f-117">Importar para KSP de Trusted Platform Module (TPM) se presente, caso contrário, falha.</span><span class="sxs-lookup"><span data-stu-id="c334f-117">Import to Trusted Platform Module (TPM) KSP if present, otherwise fail.</span></span>|
|<span data-ttu-id="c334f-118">usePassportForWorkKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="c334f-118">usePassportForWorkKspOtherwiseFail</span></span>|<span data-ttu-id="c334f-119">2 </span><span class="sxs-lookup"><span data-stu-id="c334f-119">2</span></span>|<span data-ttu-id="c334f-120">Importe para o Passport para trabalho do KSP, se disponível, caso contrário, falha.</span><span class="sxs-lookup"><span data-stu-id="c334f-120">Import to Passport for work KSP if available, otherwise fail.</span></span>|
|<span data-ttu-id="c334f-121">useSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="c334f-121">useSoftwareKsp</span></span>|<span data-ttu-id="c334f-122">3 </span><span class="sxs-lookup"><span data-stu-id="c334f-122">3</span></span>|<span data-ttu-id="c334f-123">Importar para KSP de software.</span><span class="sxs-lookup"><span data-stu-id="c334f-123">Import to Software KSP.</span></span>|



