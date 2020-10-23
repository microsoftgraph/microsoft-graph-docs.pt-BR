---
title: tipo de enumeração firewallCertificateRevocationListCheckMethodType
description: Valores possíveis para firewallCertificateRevocationListCheckMethod
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 84ae3483976b9a6aa5763ba9f2229b4af582c3d9
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728981"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="7ff11-103">tipo de enumeração firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="7ff11-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

<span data-ttu-id="7ff11-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ff11-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7ff11-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7ff11-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ff11-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7ff11-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ff11-107">Valores possíveis para firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="7ff11-107">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="7ff11-108">Membros</span><span class="sxs-lookup"><span data-stu-id="7ff11-108">Members</span></span>
|<span data-ttu-id="7ff11-109">Membro</span><span class="sxs-lookup"><span data-stu-id="7ff11-109">Member</span></span>|<span data-ttu-id="7ff11-110">Valor</span><span class="sxs-lookup"><span data-stu-id="7ff11-110">Value</span></span>|<span data-ttu-id="7ff11-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ff11-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ff11-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="7ff11-112">deviceDefault</span></span>|<span data-ttu-id="7ff11-113">,0</span><span class="sxs-lookup"><span data-stu-id="7ff11-113">0</span></span>|<span data-ttu-id="7ff11-114">Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="7ff11-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="7ff11-115">none</span><span class="sxs-lookup"><span data-stu-id="7ff11-115">none</span></span>|<span data-ttu-id="7ff11-116">1</span><span class="sxs-lookup"><span data-stu-id="7ff11-116">1</span></span>|<span data-ttu-id="7ff11-117">Não verificar a lista de certificados revogados</span><span class="sxs-lookup"><span data-stu-id="7ff11-117">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="7ff11-118">Houve</span><span class="sxs-lookup"><span data-stu-id="7ff11-118">attempt</span></span>|<span data-ttu-id="7ff11-119">duas</span><span class="sxs-lookup"><span data-stu-id="7ff11-119">2</span></span>|<span data-ttu-id="7ff11-120">Tentar verificação de CRL e permitir um certificado somente se o certificado for confirmado pela verificação</span><span class="sxs-lookup"><span data-stu-id="7ff11-120">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="7ff11-121">precisa</span><span class="sxs-lookup"><span data-stu-id="7ff11-121">require</span></span>|<span data-ttu-id="7ff11-122">3D</span><span class="sxs-lookup"><span data-stu-id="7ff11-122">3</span></span>|<span data-ttu-id="7ff11-123">Exigir uma verificação de CRL bem-sucedida antes de permitir um certificado</span><span class="sxs-lookup"><span data-stu-id="7ff11-123">Require a successful CRL check before allowing a certificate</span></span>|





