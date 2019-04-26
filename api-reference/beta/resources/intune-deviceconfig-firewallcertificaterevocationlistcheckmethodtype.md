---
title: tipo de enumeração firewallCertificateRevocationListCheckMethodType
description: Valores possíveis para firewallCertificateRevocationListCheckMethod
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 789ba503887a7200491f3fdc307ccaeb302b3f05
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32556264"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="ca5db-103">tipo de enumeração firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="ca5db-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="ca5db-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ca5db-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca5db-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ca5db-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca5db-106">Valores possíveis para firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="ca5db-106">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="ca5db-107">Membros</span><span class="sxs-lookup"><span data-stu-id="ca5db-107">Members</span></span>
|<span data-ttu-id="ca5db-108">Membro</span><span class="sxs-lookup"><span data-stu-id="ca5db-108">Member</span></span>|<span data-ttu-id="ca5db-109">Valor</span><span class="sxs-lookup"><span data-stu-id="ca5db-109">Value</span></span>|<span data-ttu-id="ca5db-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca5db-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca5db-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="ca5db-111">deviceDefault</span></span>|<span data-ttu-id="ca5db-112">,0</span><span class="sxs-lookup"><span data-stu-id="ca5db-112">0</span></span>|<span data-ttu-id="ca5db-113">Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="ca5db-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="ca5db-114">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="ca5db-114">none</span></span>|<span data-ttu-id="ca5db-115">1 </span><span class="sxs-lookup"><span data-stu-id="ca5db-115">1</span></span>|<span data-ttu-id="ca5db-116">Não verificar a lista de certificados revogados</span><span class="sxs-lookup"><span data-stu-id="ca5db-116">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="ca5db-117">Houve</span><span class="sxs-lookup"><span data-stu-id="ca5db-117">attempt</span></span>|<span data-ttu-id="ca5db-118">2 </span><span class="sxs-lookup"><span data-stu-id="ca5db-118">2</span></span>|<span data-ttu-id="ca5db-119">Tentar verificação de CRL e permitir um certificado somente se o certificado for confirmado pela verificação</span><span class="sxs-lookup"><span data-stu-id="ca5db-119">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="ca5db-120">precisa</span><span class="sxs-lookup"><span data-stu-id="ca5db-120">require</span></span>|<span data-ttu-id="ca5db-121">3 </span><span class="sxs-lookup"><span data-stu-id="ca5db-121">3</span></span>|<span data-ttu-id="ca5db-122">Exigir uma verificação de CRL bem-sucedida antes de permitir um certificado</span><span class="sxs-lookup"><span data-stu-id="ca5db-122">Require a successful CRL check before allowing a certificate</span></span>|





