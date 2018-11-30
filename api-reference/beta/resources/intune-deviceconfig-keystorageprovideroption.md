---
title: tipo de enum keyStorageProviderOption
description: Opções de importação do armazenamento de chave KSP (provedor).
ms.openlocfilehash: 236489d288ec0be70a818e1c51b8c634ad3933a8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034040"
---
# <a name="keystorageprovideroption-enum-type"></a><span data-ttu-id="f1c09-103">tipo de enum keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="f1c09-103">keyStorageProviderOption enum type</span></span>

> <span data-ttu-id="f1c09-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f1c09-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f1c09-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f1c09-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f1c09-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f1c09-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f1c09-107">Opções de importação do armazenamento de chave KSP (provedor).</span><span class="sxs-lookup"><span data-stu-id="f1c09-107">Key Storage Provider (KSP) Import Options.</span></span>
## <a name="members"></a><span data-ttu-id="f1c09-108">Membros</span><span class="sxs-lookup"><span data-stu-id="f1c09-108">Members</span></span>
|<span data-ttu-id="f1c09-109">Membro</span><span class="sxs-lookup"><span data-stu-id="f1c09-109">Member</span></span>|<span data-ttu-id="f1c09-110">Valor</span><span class="sxs-lookup"><span data-stu-id="f1c09-110">Value</span></span>|<span data-ttu-id="f1c09-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1c09-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1c09-112">useTpmKspOtherwiseUseSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="f1c09-112">useTpmKspOtherwiseUseSoftwareKsp</span></span>|<span data-ttu-id="f1c09-113">0</span><span class="sxs-lookup"><span data-stu-id="f1c09-113">0</span></span>|<span data-ttu-id="f1c09-114">Importação para Trusted Platform Module (TPM) KSP se presente, caso contrário, importe para KSP de Software.</span><span class="sxs-lookup"><span data-stu-id="f1c09-114">Import to Trusted Platform Module (TPM) KSP if present, otherwise import to Software KSP.</span></span>|
|<span data-ttu-id="f1c09-115">useTpmKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="f1c09-115">useTpmKspOtherwiseFail</span></span>|<span data-ttu-id="f1c09-116">1</span><span class="sxs-lookup"><span data-stu-id="f1c09-116">1</span></span>|<span data-ttu-id="f1c09-117">Importação para Trusted Platform Module (TPM) KSP se presente, caso contrário falhar.</span><span class="sxs-lookup"><span data-stu-id="f1c09-117">Import to Trusted Platform Module (TPM) KSP if present, otherwise fail.</span></span>|
|<span data-ttu-id="f1c09-118">usePassportForWorkKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="f1c09-118">usePassportForWorkKspOtherwiseFail</span></span>|<span data-ttu-id="f1c09-119">2</span><span class="sxs-lookup"><span data-stu-id="f1c09-119">2</span></span>|<span data-ttu-id="f1c09-120">Importar Passport trabalho KSP se estiver disponível, caso contrário falhar.</span><span class="sxs-lookup"><span data-stu-id="f1c09-120">Import to Passport for work KSP if available, otherwise fail.</span></span>|
|<span data-ttu-id="f1c09-121">useSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="f1c09-121">useSoftwareKsp</span></span>|<span data-ttu-id="f1c09-122">3</span><span class="sxs-lookup"><span data-stu-id="f1c09-122">3</span></span>|<span data-ttu-id="f1c09-123">Importação ao Software KSP.</span><span class="sxs-lookup"><span data-stu-id="f1c09-123">Import to Software KSP.</span></span>|





