---
title: tipo de enum keyStorageProviderOption
description: Opções de importação do armazenamento de chave KSP (provedor).
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6993d7e241ef94c572975c709c286a14f6eabf5b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424221"
---
# <a name="keystorageprovideroption-enum-type"></a><span data-ttu-id="85dd2-103">tipo de enum keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="85dd2-103">keyStorageProviderOption enum type</span></span>

> <span data-ttu-id="85dd2-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="85dd2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="85dd2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="85dd2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="85dd2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="85dd2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85dd2-107">Opções de importação do armazenamento de chave KSP (provedor).</span><span class="sxs-lookup"><span data-stu-id="85dd2-107">Key Storage Provider (KSP) Import Options.</span></span>

## <a name="members"></a><span data-ttu-id="85dd2-108">Membros</span><span class="sxs-lookup"><span data-stu-id="85dd2-108">Members</span></span>
|<span data-ttu-id="85dd2-109">Membro</span><span class="sxs-lookup"><span data-stu-id="85dd2-109">Member</span></span>|<span data-ttu-id="85dd2-110">Valor</span><span class="sxs-lookup"><span data-stu-id="85dd2-110">Value</span></span>|<span data-ttu-id="85dd2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="85dd2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85dd2-112">useTpmKspOtherwiseUseSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="85dd2-112">useTpmKspOtherwiseUseSoftwareKsp</span></span>|<span data-ttu-id="85dd2-113">0</span><span class="sxs-lookup"><span data-stu-id="85dd2-113">0</span></span>|<span data-ttu-id="85dd2-114">Importação para Trusted Platform Module (TPM) KSP se presente, caso contrário, importe para KSP de Software.</span><span class="sxs-lookup"><span data-stu-id="85dd2-114">Import to Trusted Platform Module (TPM) KSP if present, otherwise import to Software KSP.</span></span>|
|<span data-ttu-id="85dd2-115">useTpmKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="85dd2-115">useTpmKspOtherwiseFail</span></span>|<span data-ttu-id="85dd2-116">1</span><span class="sxs-lookup"><span data-stu-id="85dd2-116">1</span></span>|<span data-ttu-id="85dd2-117">Importação para Trusted Platform Module (TPM) KSP se presente, caso contrário falhar.</span><span class="sxs-lookup"><span data-stu-id="85dd2-117">Import to Trusted Platform Module (TPM) KSP if present, otherwise fail.</span></span>|
|<span data-ttu-id="85dd2-118">usePassportForWorkKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="85dd2-118">usePassportForWorkKspOtherwiseFail</span></span>|<span data-ttu-id="85dd2-119">2</span><span class="sxs-lookup"><span data-stu-id="85dd2-119">2</span></span>|<span data-ttu-id="85dd2-120">Importar Passport trabalho KSP se estiver disponível, caso contrário falhar.</span><span class="sxs-lookup"><span data-stu-id="85dd2-120">Import to Passport for work KSP if available, otherwise fail.</span></span>|
|<span data-ttu-id="85dd2-121">useSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="85dd2-121">useSoftwareKsp</span></span>|<span data-ttu-id="85dd2-122">3</span><span class="sxs-lookup"><span data-stu-id="85dd2-122">3</span></span>|<span data-ttu-id="85dd2-123">Importação ao Software KSP.</span><span class="sxs-lookup"><span data-stu-id="85dd2-123">Import to Software KSP.</span></span>|




