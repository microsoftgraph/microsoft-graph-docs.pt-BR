---
title: tipo de enumeração keyStorageProviderOption
description: Opções de importação do KSP (provedor de armazenamento de chave).
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1d3098daf1d2baf30788328e8cf5c5f665029ab0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439949"
---
# <a name="keystorageprovideroption-enum-type"></a><span data-ttu-id="a4e9f-103">tipo de enumeração keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="a4e9f-103">keyStorageProviderOption enum type</span></span>

<span data-ttu-id="a4e9f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4e9f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a4e9f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a4e9f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4e9f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a4e9f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4e9f-107">Opções de importação do KSP (provedor de armazenamento de chave).</span><span class="sxs-lookup"><span data-stu-id="a4e9f-107">Key Storage Provider (KSP) Import Options.</span></span>

## <a name="members"></a><span data-ttu-id="a4e9f-108">Membros</span><span class="sxs-lookup"><span data-stu-id="a4e9f-108">Members</span></span>
|<span data-ttu-id="a4e9f-109">Membro</span><span class="sxs-lookup"><span data-stu-id="a4e9f-109">Member</span></span>|<span data-ttu-id="a4e9f-110">Valor</span><span class="sxs-lookup"><span data-stu-id="a4e9f-110">Value</span></span>|<span data-ttu-id="a4e9f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4e9f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4e9f-112">useTpmKspOtherwiseUseSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="a4e9f-112">useTpmKspOtherwiseUseSoftwareKsp</span></span>|<span data-ttu-id="a4e9f-113">,0</span><span class="sxs-lookup"><span data-stu-id="a4e9f-113">0</span></span>|<span data-ttu-id="a4e9f-114">Importar para KSP de Trusted Platform Module (TPM) se presente, caso contrário, importe para o KSP de software.</span><span class="sxs-lookup"><span data-stu-id="a4e9f-114">Import to Trusted Platform Module (TPM) KSP if present, otherwise import to Software KSP.</span></span>|
|<span data-ttu-id="a4e9f-115">useTpmKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="a4e9f-115">useTpmKspOtherwiseFail</span></span>|<span data-ttu-id="a4e9f-116">1</span><span class="sxs-lookup"><span data-stu-id="a4e9f-116">1</span></span>|<span data-ttu-id="a4e9f-117">Importar para KSP de Trusted Platform Module (TPM) se presente, caso contrário, falha.</span><span class="sxs-lookup"><span data-stu-id="a4e9f-117">Import to Trusted Platform Module (TPM) KSP if present, otherwise fail.</span></span>|
|<span data-ttu-id="a4e9f-118">usePassportForWorkKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="a4e9f-118">usePassportForWorkKspOtherwiseFail</span></span>|<span data-ttu-id="a4e9f-119">duas</span><span class="sxs-lookup"><span data-stu-id="a4e9f-119">2</span></span>|<span data-ttu-id="a4e9f-120">Importe para o Passport para trabalho do KSP, se disponível, caso contrário, falha.</span><span class="sxs-lookup"><span data-stu-id="a4e9f-120">Import to Passport for work KSP if available, otherwise fail.</span></span>|
|<span data-ttu-id="a4e9f-121">useSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="a4e9f-121">useSoftwareKsp</span></span>|<span data-ttu-id="a4e9f-122">3D</span><span class="sxs-lookup"><span data-stu-id="a4e9f-122">3</span></span>|<span data-ttu-id="a4e9f-123">Importar para KSP de software.</span><span class="sxs-lookup"><span data-stu-id="a4e9f-123">Import to Software KSP.</span></span>|



