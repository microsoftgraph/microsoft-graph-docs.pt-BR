---
title: tipo de enum keyStorageProviderOption
description: Opções de importação do armazenamento de chave KSP (provedor).
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4609092c3022b62331bbb6226a5b91e4b287ff79
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826464"
---
# <a name="keystorageprovideroption-enum-type"></a><span data-ttu-id="bb20a-103">tipo de enum keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="bb20a-103">keyStorageProviderOption enum type</span></span>

> <span data-ttu-id="bb20a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bb20a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bb20a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bb20a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bb20a-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="bb20a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bb20a-107">Opções de importação do armazenamento de chave KSP (provedor).</span><span class="sxs-lookup"><span data-stu-id="bb20a-107">Key Storage Provider (KSP) Import Options.</span></span>
## <a name="members"></a><span data-ttu-id="bb20a-108">Membros</span><span class="sxs-lookup"><span data-stu-id="bb20a-108">Members</span></span>
|<span data-ttu-id="bb20a-109">Membro</span><span class="sxs-lookup"><span data-stu-id="bb20a-109">Member</span></span>|<span data-ttu-id="bb20a-110">Valor</span><span class="sxs-lookup"><span data-stu-id="bb20a-110">Value</span></span>|<span data-ttu-id="bb20a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb20a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb20a-112">useTpmKspOtherwiseUseSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="bb20a-112">useTpmKspOtherwiseUseSoftwareKsp</span></span>|<span data-ttu-id="bb20a-113">0</span><span class="sxs-lookup"><span data-stu-id="bb20a-113">0</span></span>|<span data-ttu-id="bb20a-114">Importação para Trusted Platform Module (TPM) KSP se presente, caso contrário, importe para KSP de Software.</span><span class="sxs-lookup"><span data-stu-id="bb20a-114">Import to Trusted Platform Module (TPM) KSP if present, otherwise import to Software KSP.</span></span>|
|<span data-ttu-id="bb20a-115">useTpmKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="bb20a-115">useTpmKspOtherwiseFail</span></span>|<span data-ttu-id="bb20a-116">1</span><span class="sxs-lookup"><span data-stu-id="bb20a-116">1</span></span>|<span data-ttu-id="bb20a-117">Importação para Trusted Platform Module (TPM) KSP se presente, caso contrário falhar.</span><span class="sxs-lookup"><span data-stu-id="bb20a-117">Import to Trusted Platform Module (TPM) KSP if present, otherwise fail.</span></span>|
|<span data-ttu-id="bb20a-118">usePassportForWorkKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="bb20a-118">usePassportForWorkKspOtherwiseFail</span></span>|<span data-ttu-id="bb20a-119">2</span><span class="sxs-lookup"><span data-stu-id="bb20a-119">2</span></span>|<span data-ttu-id="bb20a-120">Importar Passport trabalho KSP se estiver disponível, caso contrário falhar.</span><span class="sxs-lookup"><span data-stu-id="bb20a-120">Import to Passport for work KSP if available, otherwise fail.</span></span>|
|<span data-ttu-id="bb20a-121">useSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="bb20a-121">useSoftwareKsp</span></span>|<span data-ttu-id="bb20a-122">3</span><span class="sxs-lookup"><span data-stu-id="bb20a-122">3</span></span>|<span data-ttu-id="bb20a-123">Importação ao Software KSP.</span><span class="sxs-lookup"><span data-stu-id="bb20a-123">Import to Software KSP.</span></span>|





