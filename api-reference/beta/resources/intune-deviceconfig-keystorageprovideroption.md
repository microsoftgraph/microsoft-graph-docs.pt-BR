---
title: tipo de enumeração keyStorageProviderOption
description: Opções de importação do KSP (provedor de armazenamento de chave).
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e345e5c3b8490c15edd83fd4d7a4eb70e4be40d5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001037"
---
# <a name="keystorageprovideroption-enum-type"></a><span data-ttu-id="a85dd-103">tipo de enumeração keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="a85dd-103">keyStorageProviderOption enum type</span></span>

> <span data-ttu-id="a85dd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a85dd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a85dd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a85dd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a85dd-106">Opções de importação do KSP (provedor de armazenamento de chave).</span><span class="sxs-lookup"><span data-stu-id="a85dd-106">Key Storage Provider (KSP) Import Options.</span></span>

## <a name="members"></a><span data-ttu-id="a85dd-107">Membros</span><span class="sxs-lookup"><span data-stu-id="a85dd-107">Members</span></span>
|<span data-ttu-id="a85dd-108">Membro</span><span class="sxs-lookup"><span data-stu-id="a85dd-108">Member</span></span>|<span data-ttu-id="a85dd-109">Valor</span><span class="sxs-lookup"><span data-stu-id="a85dd-109">Value</span></span>|<span data-ttu-id="a85dd-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a85dd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a85dd-111">useTpmKspOtherwiseUseSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="a85dd-111">useTpmKspOtherwiseUseSoftwareKsp</span></span>|<span data-ttu-id="a85dd-112">,0</span><span class="sxs-lookup"><span data-stu-id="a85dd-112">0</span></span>|<span data-ttu-id="a85dd-113">Importar para KSP de Trusted Platform Module (TPM) se presente, caso contrário, importe para o KSP de software.</span><span class="sxs-lookup"><span data-stu-id="a85dd-113">Import to Trusted Platform Module (TPM) KSP if present, otherwise import to Software KSP.</span></span>|
|<span data-ttu-id="a85dd-114">useTpmKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="a85dd-114">useTpmKspOtherwiseFail</span></span>|<span data-ttu-id="a85dd-115">1</span><span class="sxs-lookup"><span data-stu-id="a85dd-115">1</span></span>|<span data-ttu-id="a85dd-116">Importar para KSP de Trusted Platform Module (TPM) se presente, caso contrário, falha.</span><span class="sxs-lookup"><span data-stu-id="a85dd-116">Import to Trusted Platform Module (TPM) KSP if present, otherwise fail.</span></span>|
|<span data-ttu-id="a85dd-117">usePassportForWorkKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="a85dd-117">usePassportForWorkKspOtherwiseFail</span></span>|<span data-ttu-id="a85dd-118">duas</span><span class="sxs-lookup"><span data-stu-id="a85dd-118">2</span></span>|<span data-ttu-id="a85dd-119">Importe para o Passport para trabalho do KSP, se disponível, caso contrário, falha.</span><span class="sxs-lookup"><span data-stu-id="a85dd-119">Import to Passport for work KSP if available, otherwise fail.</span></span>|
|<span data-ttu-id="a85dd-120">useSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="a85dd-120">useSoftwareKsp</span></span>|<span data-ttu-id="a85dd-121">3D</span><span class="sxs-lookup"><span data-stu-id="a85dd-121">3</span></span>|<span data-ttu-id="a85dd-122">Importar para KSP de software.</span><span class="sxs-lookup"><span data-stu-id="a85dd-122">Import to Software KSP.</span></span>|





