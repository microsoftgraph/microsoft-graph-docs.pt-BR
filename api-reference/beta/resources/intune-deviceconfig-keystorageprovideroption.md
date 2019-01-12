---
title: tipo de enum keyStorageProviderOption
description: Opções de importação do armazenamento de chave KSP (provedor).
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8f3a8169b4bb6cd2357f02aa7fec89ba640780f7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946550"
---
# <a name="keystorageprovideroption-enum-type"></a><span data-ttu-id="49f5b-103">tipo de enum keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="49f5b-103">keyStorageProviderOption enum type</span></span>

> <span data-ttu-id="49f5b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="49f5b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="49f5b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="49f5b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="49f5b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="49f5b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="49f5b-107">Opções de importação do armazenamento de chave KSP (provedor).</span><span class="sxs-lookup"><span data-stu-id="49f5b-107">Key Storage Provider (KSP) Import Options.</span></span>
## <a name="members"></a><span data-ttu-id="49f5b-108">Membros</span><span class="sxs-lookup"><span data-stu-id="49f5b-108">Members</span></span>
|<span data-ttu-id="49f5b-109">Membro</span><span class="sxs-lookup"><span data-stu-id="49f5b-109">Member</span></span>|<span data-ttu-id="49f5b-110">Valor</span><span class="sxs-lookup"><span data-stu-id="49f5b-110">Value</span></span>|<span data-ttu-id="49f5b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="49f5b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49f5b-112">useTpmKspOtherwiseUseSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="49f5b-112">useTpmKspOtherwiseUseSoftwareKsp</span></span>|<span data-ttu-id="49f5b-113">0</span><span class="sxs-lookup"><span data-stu-id="49f5b-113">0</span></span>|<span data-ttu-id="49f5b-114">Importação para Trusted Platform Module (TPM) KSP se presente, caso contrário, importe para KSP de Software.</span><span class="sxs-lookup"><span data-stu-id="49f5b-114">Import to Trusted Platform Module (TPM) KSP if present, otherwise import to Software KSP.</span></span>|
|<span data-ttu-id="49f5b-115">useTpmKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="49f5b-115">useTpmKspOtherwiseFail</span></span>|<span data-ttu-id="49f5b-116">1</span><span class="sxs-lookup"><span data-stu-id="49f5b-116">1</span></span>|<span data-ttu-id="49f5b-117">Importação para Trusted Platform Module (TPM) KSP se presente, caso contrário falhar.</span><span class="sxs-lookup"><span data-stu-id="49f5b-117">Import to Trusted Platform Module (TPM) KSP if present, otherwise fail.</span></span>|
|<span data-ttu-id="49f5b-118">usePassportForWorkKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="49f5b-118">usePassportForWorkKspOtherwiseFail</span></span>|<span data-ttu-id="49f5b-119">2</span><span class="sxs-lookup"><span data-stu-id="49f5b-119">2</span></span>|<span data-ttu-id="49f5b-120">Importar Passport trabalho KSP se estiver disponível, caso contrário falhar.</span><span class="sxs-lookup"><span data-stu-id="49f5b-120">Import to Passport for work KSP if available, otherwise fail.</span></span>|
|<span data-ttu-id="49f5b-121">useSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="49f5b-121">useSoftwareKsp</span></span>|<span data-ttu-id="49f5b-122">3</span><span class="sxs-lookup"><span data-stu-id="49f5b-122">3</span></span>|<span data-ttu-id="49f5b-123">Importação ao Software KSP.</span><span class="sxs-lookup"><span data-stu-id="49f5b-123">Import to Software KSP.</span></span>|





