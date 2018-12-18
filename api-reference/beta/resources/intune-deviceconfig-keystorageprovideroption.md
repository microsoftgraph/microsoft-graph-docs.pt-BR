---
title: tipo de enum keyStorageProviderOption
description: Opções de importação do armazenamento de chave KSP (provedor).
author: tfitzmac
ms.openlocfilehash: 7923dd5c4b8a09d834d29b65928430828f3dafac
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342214"
---
# <a name="keystorageprovideroption-enum-type"></a><span data-ttu-id="79890-103">tipo de enum keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="79890-103">keyStorageProviderOption enum type</span></span>

> <span data-ttu-id="79890-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="79890-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="79890-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="79890-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="79890-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="79890-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="79890-107">Opções de importação do armazenamento de chave KSP (provedor).</span><span class="sxs-lookup"><span data-stu-id="79890-107">Key Storage Provider (KSP) Import Options.</span></span>
## <a name="members"></a><span data-ttu-id="79890-108">Membros</span><span class="sxs-lookup"><span data-stu-id="79890-108">Members</span></span>
|<span data-ttu-id="79890-109">Membro</span><span class="sxs-lookup"><span data-stu-id="79890-109">Member</span></span>|<span data-ttu-id="79890-110">Valor</span><span class="sxs-lookup"><span data-stu-id="79890-110">Value</span></span>|<span data-ttu-id="79890-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="79890-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79890-112">useTpmKspOtherwiseUseSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="79890-112">useTpmKspOtherwiseUseSoftwareKsp</span></span>|<span data-ttu-id="79890-113">0</span><span class="sxs-lookup"><span data-stu-id="79890-113">0</span></span>|<span data-ttu-id="79890-114">Importação para Trusted Platform Module (TPM) KSP se presente, caso contrário, importe para KSP de Software.</span><span class="sxs-lookup"><span data-stu-id="79890-114">Import to Trusted Platform Module (TPM) KSP if present, otherwise import to Software KSP.</span></span>|
|<span data-ttu-id="79890-115">useTpmKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="79890-115">useTpmKspOtherwiseFail</span></span>|<span data-ttu-id="79890-116">1</span><span class="sxs-lookup"><span data-stu-id="79890-116">1</span></span>|<span data-ttu-id="79890-117">Importação para Trusted Platform Module (TPM) KSP se presente, caso contrário falhar.</span><span class="sxs-lookup"><span data-stu-id="79890-117">Import to Trusted Platform Module (TPM) KSP if present, otherwise fail.</span></span>|
|<span data-ttu-id="79890-118">usePassportForWorkKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="79890-118">usePassportForWorkKspOtherwiseFail</span></span>|<span data-ttu-id="79890-119">2</span><span class="sxs-lookup"><span data-stu-id="79890-119">2</span></span>|<span data-ttu-id="79890-120">Importar Passport trabalho KSP se estiver disponível, caso contrário falhar.</span><span class="sxs-lookup"><span data-stu-id="79890-120">Import to Passport for work KSP if available, otherwise fail.</span></span>|
|<span data-ttu-id="79890-121">useSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="79890-121">useSoftwareKsp</span></span>|<span data-ttu-id="79890-122">3</span><span class="sxs-lookup"><span data-stu-id="79890-122">3</span></span>|<span data-ttu-id="79890-123">Importação ao Software KSP.</span><span class="sxs-lookup"><span data-stu-id="79890-123">Import to Software KSP.</span></span>|





