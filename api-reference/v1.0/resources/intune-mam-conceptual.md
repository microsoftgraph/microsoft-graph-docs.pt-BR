---
title: Como proteger dados de aplicativos corporativos com o Microsoft Intune
description: As políticas de proteção de aplicativos do Microsoft Intune ajudam a proteger os dados da empresa e evitar a perda de dados.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: 5f655e8b80a2f07164a8560146e1f1e2d4c1f7ec
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356552"
---
# <a name="how-to-protect-your-company-app-data-with-microsoft-intune"></a><span data-ttu-id="3d8ec-103">Como proteger dados de aplicativos corporativos com o Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="3d8ec-103">How to protect your company app data with Microsoft Intune</span></span>

> <span data-ttu-id="3d8ec-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3d8ec-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="3d8ec-105">As políticas de proteção de aplicativos do Microsoft Intune ajudam a proteger os dados da empresa e evitar a perda de dados.</span><span class="sxs-lookup"><span data-stu-id="3d8ec-105">Microsoft Intune app protection policies help protect your company data and prevent data loss.</span></span>

<span data-ttu-id="3d8ec-106">Use as políticas de proteção de aplicativos do Intune para ajudar a proteger os dados da sua empresa.</span><span class="sxs-lookup"><span data-stu-id="3d8ec-106">You can use Intune app protection policies to help protect your company’s data.</span></span> <span data-ttu-id="3d8ec-107">Como as políticas de proteção de aplicativos do Intune podem ser usadas independentemente de qualquer solução de gerenciamento de dispositivo móvel (MDM), você protege os dados da sua empresa com ou sem o registro de dispositivos em uma solução de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3d8ec-107">Because Intune app protection policies can be used independent of any mobile-device management (MDM) solution, you protect your company’s data with or without enrolling devices in a device management solution.</span></span> <span data-ttu-id="3d8ec-108">Implementando as políticas de nível de aplicativo, é possível restringir o acesso aos recursos da empresa e manter os dados dentro do âmbito do seu departamento de TI.</span><span class="sxs-lookup"><span data-stu-id="3d8ec-108">By implementing app-level policies, you can restrict access to company resources and keep data within the purview of your IT department.</span></span>

<span data-ttu-id="3d8ec-109">Os seguintes recursos do Graph estão disponíveis para gerenciar políticas de proteção de aplicativos no Intune:</span><span class="sxs-lookup"><span data-stu-id="3d8ec-109">The following Graph resources are available to manage app protection polices in Intune:</span></span>  

- [<span data-ttu-id="3d8ec-110">Proteção de aplicativo gerenciado Android</span><span class="sxs-lookup"><span data-stu-id="3d8ec-110">Android managed app protection</span></span>](intune-mam-androidmanagedappprotection.md)
- [<span data-ttu-id="3d8ec-111">Registro de aplicativo gerenciado Android</span><span class="sxs-lookup"><span data-stu-id="3d8ec-111">Android managed app registration</span></span>](intune-mam-androidmanagedappregistration.md)
- [<span data-ttu-id="3d8ec-112">Identificador de aplicativo móvel Android</span><span class="sxs-lookup"><span data-stu-id="3d8ec-112">Android mobile app identifier</span></span>](intune-mam-androidmobileappidentifier.md)
- [<span data-ttu-id="3d8ec-113">Tipo de aplicativo</span><span class="sxs-lookup"><span data-stu-id="3d8ec-113">Application type</span></span>](intune-wip-applicationtype.md)
- [<span data-ttu-id="3d8ec-114">Proteção de aplicativo gerenciado padrão</span><span class="sxs-lookup"><span data-stu-id="3d8ec-114">Default managed app protection</span></span>](intune-mam-defaultmanagedappprotection.md)
- [<span data-ttu-id="3d8ec-115">Proteção de aplicativo gerenciado iOS</span><span class="sxs-lookup"><span data-stu-id="3d8ec-115">iOS managed app protection</span></span>](intune-mam-iosmanagedappprotection.md)
- [<span data-ttu-id="3d8ec-116">Registro de aplicativo gerenciado iOS</span><span class="sxs-lookup"><span data-stu-id="3d8ec-116">iOS managed app registration</span></span>](intune-mam-iosmanagedappregistration.md)
- [<span data-ttu-id="3d8ec-117">Identificador de aplicativo móvel iOS</span><span class="sxs-lookup"><span data-stu-id="3d8ec-117">iOS mobile app identifier</span></span>](intune-mam-iosmobileappidentifier.md)
- [<span data-ttu-id="3d8ec-118">Intervalo de IP</span><span class="sxs-lookup"><span data-stu-id="3d8ec-118">IP range</span></span>](intune-mam-iprange.md)
- [<span data-ttu-id="3d8ec-119">Intervalo de IPv4</span><span class="sxs-lookup"><span data-stu-id="3d8ec-119">IPv4 range</span></span>](intune-mam-ipv4range.md)
- [<span data-ttu-id="3d8ec-120">Intervalo de IPv6</span><span class="sxs-lookup"><span data-stu-id="3d8ec-120">IPv6 range</span></span>](intune-mam-ipv6range.md)
- [<span data-ttu-id="3d8ec-121">JSON</span><span class="sxs-lookup"><span data-stu-id="3d8ec-121">JSON</span></span>](intune-mam-json.md)
- [<span data-ttu-id="3d8ec-122">Par chave/valor</span><span class="sxs-lookup"><span data-stu-id="3d8ec-122">Key/value pair</span></span>](intune-mam-keyvaluepair.md)
- [<span data-ttu-id="3d8ec-123">Nível de compartilhamento de área de transferência do aplicativo gerenciado</span><span class="sxs-lookup"><span data-stu-id="3d8ec-123">Managed app clipboard sharing level</span></span>](intune-mam-managedappclipboardsharinglevel.md)
- [<span data-ttu-id="3d8ec-124">Configuração de aplicativo gerenciado</span><span class="sxs-lookup"><span data-stu-id="3d8ec-124">Managed app configuration</span></span>](intune-mam-managedappconfiguration.md)
- [<span data-ttu-id="3d8ec-125">Tipo de criptografia de dados do aplicativo gerenciado</span><span class="sxs-lookup"><span data-stu-id="3d8ec-125">Managed app data encryption type</span></span>](intune-mam-managedappdataencryptiontype.md)
- [<span data-ttu-id="3d8ec-126">Local de armazenamento de dados do aplicativo gerenciado</span><span class="sxs-lookup"><span data-stu-id="3d8ec-126">Managed app data storage location</span></span>](intune-mam-managedappdatastoragelocation.md)
- [<span data-ttu-id="3d8ec-127">Nível de transferência de dados do aplicativo gerenciado</span><span class="sxs-lookup"><span data-stu-id="3d8ec-127">Managed app data transfer level</span></span>](intune-mam-managedappdatatransferlevel.md)
- [<span data-ttu-id="3d8ec-128">Status de diagnóstico de aplicativo gerenciado</span><span class="sxs-lookup"><span data-stu-id="3d8ec-128">Managed app diagnostic status</span></span>](intune-mam-managedappdiagnosticstatus.md)
- [<span data-ttu-id="3d8ec-129">Motivo de sinalização do aplicativo gerenciado</span><span class="sxs-lookup"><span data-stu-id="3d8ec-129">Managed app flagged reason</span></span>](intune-mam-managedappflaggedreason.md)
- [<span data-ttu-id="3d8ec-130">Operação de aplicativo gerenciado</span><span class="sxs-lookup"><span data-stu-id="3d8ec-130">Managed app operation</span></span>](intune-mam-managedappoperation.md)
- [<span data-ttu-id="3d8ec-131">Conjunto de caracteres do PIN do aplicativo gerenciado</span><span class="sxs-lookup"><span data-stu-id="3d8ec-131">Managed app PIN character set</span></span>](intune-mam-managedapppincharacterset.md)
- [<span data-ttu-id="3d8ec-132">Política de aplicativo gerenciado</span><span class="sxs-lookup"><span data-stu-id="3d8ec-132">Managed app policy</span></span>](intune-mam-managedapppolicy.md)
- [<span data-ttu-id="3d8ec-133">Resumo da implantação da política de aplicativo gerenciado</span><span class="sxs-lookup"><span data-stu-id="3d8ec-133">Managed app policy deployment summary</span></span>](intune-mam-managedapppolicydeploymentsummary.md)
- [<span data-ttu-id="3d8ec-134">Resumo por aplicativo da implantação da política de aplicativo gerenciado</span><span class="sxs-lookup"><span data-stu-id="3d8ec-134">Managed app policy deployment summary per app</span></span>](intune-mam-managedapppolicydeploymentsummaryperapp.md)
- [<span data-ttu-id="3d8ec-135">Proteção de aplicativo gerenciado</span><span class="sxs-lookup"><span data-stu-id="3d8ec-135">Managed app protection</span></span>](intune-mam-managedappprotection.md)
- [<span data-ttu-id="3d8ec-136">Registro de aplicativo gerenciado</span><span class="sxs-lookup"><span data-stu-id="3d8ec-136">Managed app registration</span></span>](intune-mam-managedappregistration.md)
- [<span data-ttu-id="3d8ec-137">Status de aplicativo gerenciado</span><span class="sxs-lookup"><span data-stu-id="3d8ec-137">Managed app status</span></span>](intune-mam-managedappstatus.md)
- [<span data-ttu-id="3d8ec-138">Status bruto de aplicativo gerenciado</span><span class="sxs-lookup"><span data-stu-id="3d8ec-138">Managed app status raw</span></span>](intune-mam-managedappstatusraw.md)
- [<span data-ttu-id="3d8ec-139">Aplicativo móvel gerenciado</span><span class="sxs-lookup"><span data-stu-id="3d8ec-139">Managed mobile app</span></span>](intune-mam-managedmobileapp.md)
- [<span data-ttu-id="3d8ec-140">Política de proteção de informações do Windows MDM</span><span class="sxs-lookup"><span data-stu-id="3d8ec-140">MDM windows information protection policy</span></span>](intune-mam-mdmwindowsinformationprotectionpolicy.md)
- [<span data-ttu-id="3d8ec-141">Identificador de aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="3d8ec-141">Mobile app identifier</span></span>](intune-mam-mobileappidentifier.md)
- [<span data-ttu-id="3d8ec-142">Domínio com proxy</span><span class="sxs-lookup"><span data-stu-id="3d8ec-142">Proxied domain</span></span>](intune-mam-proxieddomain.md)
- [<span data-ttu-id="3d8ec-143">Configuração direcionada de aplicativo gerenciado</span><span class="sxs-lookup"><span data-stu-id="3d8ec-143">Targeted managed app configuration</span></span>](intune-mam-targetedmanagedappconfiguration.md)
- [<span data-ttu-id="3d8ec-144">Atribuição de política de proteção de aplicativo gerenciado direcionado</span><span class="sxs-lookup"><span data-stu-id="3d8ec-144">Targeted managed app policy assignment</span></span>](intune-mam-targetedmanagedapppolicyassignment.md)
- [<span data-ttu-id="3d8ec-145">Proteção de aplicativo gerenciado direcionado</span><span class="sxs-lookup"><span data-stu-id="3d8ec-145">Targeted managed app protection</span></span>](intune-mam-targetedmanagedappprotection.md)
- [<span data-ttu-id="3d8ec-146">Proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="3d8ec-146">Windows information protection</span></span>](intune-mam-windowsinformationprotection.md)
- [<span data-ttu-id="3d8ec-147">Arquivo de proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="3d8ec-147">Windows information protection app</span></span>](intune-mam-windowsinformationprotectionapp.md)
- [<span data-ttu-id="3d8ec-148">Resumo de aprendizagem de aplicativos da proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="3d8ec-148">Windows information protection app learning summary</span></span>](intune-wip-windowsinformationprotectionapplearningsummary.md)
- [<span data-ttu-id="3d8ec-149">Arquivo do bloqueador de aplicativos da proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="3d8ec-149">Windows information protection app locker file</span></span>](intune-mam-windowsinformationprotectionapplockerfile.md)
- [<span data-ttu-id="3d8ec-150">Certificado de recuperação de dados de proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="3d8ec-150">Windows information protection data recovery certificate</span></span>](intune-mam-windowsinformationprotectiondatarecoverycertificate.md)
- [<span data-ttu-id="3d8ec-151">Aplicativo da área de trabalho da proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="3d8ec-151">Windows information protection desktop app</span></span>](intune-mam-windowsinformationprotectiondesktopapp.md)
- [<span data-ttu-id="3d8ec-152">Nível de aplicação da proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="3d8ec-152">Windows information protection enforcement level</span></span>](intune-mam-windowsinformationprotectionenforcementlevel.md)
- [<span data-ttu-id="3d8ec-153">Coleção de intervalos de IP da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="3d8ec-153">Windows information protection IP range collection</span></span>](intune-mam-windowsinformationprotectioniprangecollection.md)
- [<span data-ttu-id="3d8ec-154">Resumo de aprendizagem da rede de proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="3d8ec-154">Windows information protection network learning summary</span></span>](intune-wip-windowsinformationprotectionnetworklearningsummary.md)
- [<span data-ttu-id="3d8ec-155">Requisitos de caracteres do PIN de proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="3d8ec-155">Windows information protection PIN character requirements</span></span>](intune-mam-windowsinformationprotectionpincharacterrequirements.md)
- [<span data-ttu-id="3d8ec-156">Política de proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="3d8ec-156">Windows information protection policy</span></span>](intune-mam-windowsinformationprotectionpolicy.md)
- [<span data-ttu-id="3d8ec-157">Coleção de domínios como proxy da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="3d8ec-157">Windows information protection proxied domain collection</span></span>](intune-mam-windowsinformationprotectionproxieddomaincollection.md)
- [<span data-ttu-id="3d8ec-158">Coleção de recursos da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="3d8ec-158">Windows information protection resource collection</span></span>](intune-mam-windowsinformationprotectionresourcecollection.md)
- [<span data-ttu-id="3d8ec-159">Aplicativo de loja de proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="3d8ec-159">Windows information protection store app</span></span>](intune-mam-windowsinformationprotectionstoreapp.md)

