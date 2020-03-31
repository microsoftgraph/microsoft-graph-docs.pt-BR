---
title: Visão geral da API de Impressão Universal
description: A Impressão Universal é uma solução moderna que as organizações podem usar para gerir a infraestrutura de impressão através de serviços de nuvem da Microsoft.
author: braedenp-msft
localization_priority: Priority
ms.prod: universal-print
ms.custom: scenarios:getting-started
ms.openlocfilehash: 7a35c68acc3fd5d3d4f1750b9c3f2d80c3ed1985
ms.sourcegitcommit: 66a52d2e63cf3447ec50bd28e562d99e7c344814
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2020
ms.locfileid: "43061920"
---
# <a name="universal-print-api-overview"></a><span data-ttu-id="15718-103">Visão geral da API de Impressão Universal</span><span class="sxs-lookup"><span data-stu-id="15718-103">Universal Print API overview</span></span>

<span data-ttu-id="15718-104">A Impressão Universal é uma solução moderna que as organizações podem usar para gerir a infraestrutura de impressão através de serviços de nuvem da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="15718-104">Universal Print is a modern print solution that organizations can use to manage their print infrastructure through cloud services from Microsoft.</span></span>

![Captura de tela da página inicial do portal da Impressão Universal do Azure](images/universal-print-portal-homepage.png)

## <a name="why-use-universal-print"></a><span data-ttu-id="15718-106">Por que usar a Impressão Universal?</span><span class="sxs-lookup"><span data-stu-id="15718-106">Why use Universal Print?</span></span>

<span data-ttu-id="15718-107">A Impressão Universal move a funcionalidade de impressão do Windows Server para a nuvem do Microsoft 365, para que as organizações não precisem mais de servidores de impressão locais e não precisem instalar drivers de impressora em dispositivos.</span><span class="sxs-lookup"><span data-stu-id="15718-107">Universal Print moves key Windows Server print functionality to the Microsoft 365 cloud, so organizations no longer need on-premises print servers and do not need to install printer drivers on devices.</span></span> <span data-ttu-id="15718-108">Além disso, a Impressão Universal adiciona funcionalidades fundamentais, como grupos de segurança para acesso à impressora, descoberta de impressora baseada no local e uma experiência de administrador avançada.</span><span class="sxs-lookup"><span data-stu-id="15718-108">In addition, Universal Print adds key functionality like security groups for printer access, location-based printer discovery, and a rich administrator experience.</span></span>

<span data-ttu-id="15718-109">Como as organizações adotam a Impressão Universal, as organizações e os fornecedores independentes de software (ISVs) podem usar a API de Impressão Universal no Microsoft Graph para criar e ampliar aplicativos para suportar novos cenários.</span><span class="sxs-lookup"><span data-stu-id="15718-109">As organizations adopt Universal Print, organizations and independent software vendors (ISVs) can use the Universal Print API in Microsoft Graph to build and extend applications to support new scenarios.</span></span>

### <a name="print-documents-from-web-and-mobile-applications"></a><span data-ttu-id="15718-110">Imprimir documentos de aplicativos da Web e móveis</span><span class="sxs-lookup"><span data-stu-id="15718-110">Print documents from web and mobile applications</span></span>

<span data-ttu-id="15718-111">Mover a infraestrutura de impressão para a nuvem permite imprimir documentos diretamente de aplicativos da Web e móveis.</span><span class="sxs-lookup"><span data-stu-id="15718-111">Moving print infrastructure to the cloud enables printing documents directly from web and mobile applications.</span></span>

<span data-ttu-id="15718-112">Introdução à API de Impressão Universal:</span><span class="sxs-lookup"><span data-stu-id="15718-112">To get started with the Universal Print API:</span></span>

1. <span data-ttu-id="15718-113">[Criar um trabalho de impressão](/graph/api/printer-post-jobs?view=graph-rest-beta) e armazenar a ID do documento resultante.</span><span class="sxs-lookup"><span data-stu-id="15718-113">[Create a print job](/graph/api/printer-post-jobs?view=graph-rest-beta) and store the resulting document ID.</span></span>
2. <span data-ttu-id="15718-114">[Carregar dados](/graph/api/printdocument-uploaddata?view=graph-rest-beta) para o documento.</span><span class="sxs-lookup"><span data-stu-id="15718-114">[Upload document data](/graph/api/printdocument-uploaddata?view=graph-rest-beta) to the document.</span></span>
3. <span data-ttu-id="15718-115">[Iniciar o trabalho de impressão](/graph/api/printjob-startprintjob?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="15718-115">[Start the print job](/graph/api/printjob-startprintjob?view=graph-rest-beta).</span></span>

### <a name="manage-printers"></a><span data-ttu-id="15718-116">Gerenciar impressoras</span><span class="sxs-lookup"><span data-stu-id="15718-116">Manage printers</span></span>

<span data-ttu-id="15718-117">É uma tarefa complexa acompanhar as impressoras de uma organização, suas configurações e uso.</span><span class="sxs-lookup"><span data-stu-id="15718-117">Keeping track of an organization's printers, printer configurations, and printer usage is a complex task.</span></span> <span data-ttu-id="15718-118">A API de Impressão Universal permite a integração em todas as três áreas.</span><span class="sxs-lookup"><span data-stu-id="15718-118">The Universal Print API enables integration in all three areas.</span></span>

* <span data-ttu-id="15718-119">**Fique de olho no estado, configurações e disponibilidade da impressora**, usando a [Lista de impressoras](/graph/api/print-list-printers?view=graph-rest-beta) e o [printerStatus](/graph/api/resources/printerstatus?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="15718-119">**Keep an eye on printer status, configurations, and availability** by using [List printers](/graph/api/print-list-printers?view=graph-rest-beta) and [printerStatus](/graph/api/resources/printerstatus?view=graph-rest-beta).</span></span>

* <span data-ttu-id="15718-120">**Veja quem está usando as impressoras e o quanto elas estão imprimindo** usando as APIs de relatórios:</span><span class="sxs-lookup"><span data-stu-id="15718-120">**See who's using your printers and how much they're printing** by using the reporting APIs:</span></span>
  * [<span data-ttu-id="15718-121">Listar dailyPrintUsageSummariesByUser</span><span class="sxs-lookup"><span data-stu-id="15718-121">List dailyPrintUsageSummariesByUser</span></span>](/graph/api/reportroot-list-dailyprintusagesummariesbyuser?view=graph-rest-beta)
  * [<span data-ttu-id="15718-122">Listar monthlyPrintUsageSummariesByUser</span><span class="sxs-lookup"><span data-stu-id="15718-122">List monthlyPrintUsageSummariesByUser</span></span>](/graph/api/reportroot-list-monthlyprintusagesummariesbyuser?view=graph-rest-beta)
  * [<span data-ttu-id="15718-123">Listar dailyPrintUsageSummariesByPrinter</span><span class="sxs-lookup"><span data-stu-id="15718-123">List dailyPrintUsageSummariesByPrinter</span></span>](/graph/api/reportroot-list-dailyprintusagesummariesbyprinter?view=graph-rest-beta)
  * [<span data-ttu-id="15718-124">Listar monthlyPrintUsageSummariesByPrinter</span><span class="sxs-lookup"><span data-stu-id="15718-124">List monthlyPrintUsageSummariesByPrinter</span></span>](/graph/api/reportroot-list-monthlyprintusagesummariesbyprinter?view=graph-rest-beta)

* <span data-ttu-id="15718-125">**Configurar permissões de usuário** modificando a associação de usuários e grupos das impressoras:</span><span class="sxs-lookup"><span data-stu-id="15718-125">**Configure user permissions** by modifying user and group membership on printers:</span></span>
  * [<span data-ttu-id="15718-126">Listar allowedUsers</span><span class="sxs-lookup"><span data-stu-id="15718-126">List allowedUsers</span></span>](/graph/api/printer-list-allowedusers?view=graph-rest-beta)
  * [<span data-ttu-id="15718-127">Adicionar allowedUser</span><span class="sxs-lookup"><span data-stu-id="15718-127">Add allowedUser</span></span>](/graph/api/printer-post-allowedusers?view=graph-rest-beta)
  * [<span data-ttu-id="15718-128">Remover allowedUser</span><span class="sxs-lookup"><span data-stu-id="15718-128">Remove allowedUser</span></span>](/graph/api/printer-delete-alloweduser?view=graph-rest-beta)
  * [<span data-ttu-id="15718-129">Listar allowedGroups</span><span class="sxs-lookup"><span data-stu-id="15718-129">List allowedGroups</span></span>](/graph/api/printer-list-allowedgroups?view=graph-rest-beta)
  * [<span data-ttu-id="15718-130">Adicionar allowedGroup</span><span class="sxs-lookup"><span data-stu-id="15718-130">Add allowedGroup</span></span>](/graph/api/printer-post-allowedgroups?view=graph-rest-beta)
  * [<span data-ttu-id="15718-131">Remover allowedGroup</span><span class="sxs-lookup"><span data-stu-id="15718-131">Remove allowedGroup</span></span>](/graph/api/printer-delete-allowedgroup?view=graph-rest-beta)

### <a name="seamlessly-replace-or-update-printer-hardware"></a><span data-ttu-id="15718-132">Substituir ou atualizar o hardware da impressora sem problemas</span><span class="sxs-lookup"><span data-stu-id="15718-132">Seamlessly replace or update printer hardware</span></span>

<span data-ttu-id="15718-133">As impressoras não estarão visíveis para os usuários até que sejam [compartilhadas](/graph/api/print-post-printershares?view=graph-rest-beta), proporcionando aos administradores um controle detalhado sobre qual hardware de impressora estará disponível em um determinado momento.</span><span class="sxs-lookup"><span data-stu-id="15718-133">Printers are not visible to users until they are [shared](/graph/api/print-post-printershares?view=graph-rest-beta), providing administrators fine-grained control over which printer hardware is available at a given time.</span></span>

<span data-ttu-id="15718-134">O compartilhamento de uma impressora cria um recurso [printerShare](/graph/api/resources/printershare?view=graph-rest-beta) que pode ser atualizado a qualquer momento para indicar uma impressora diferente, facilitando a substituição de hardware de uma impressora quebrada ou a desativação de impressoras para manutenção.</span><span class="sxs-lookup"><span data-stu-id="15718-134">Sharing a printer creates a [printerShare](/graph/api/resources/printershare?view=graph-rest-beta) resource that can be updated at any time to point to a different printer, making it easy to replace broken printer hardware or take printers offline for maintenance.</span></span>

<span data-ttu-id="15718-135">Para usá-lo em seu aplicativo, use [Update printerShare](/graph/api/printershare-update?view=graph-rest-beta) para atualizar a referência `printer` de printerShare.</span><span class="sxs-lookup"><span data-stu-id="15718-135">To use this in your application, use [Update printerShare](/graph/api/printershare-update?view=graph-rest-beta) to update the printerShare's `printer` reference.</span></span>

## <a name="api-reference"></a><span data-ttu-id="15718-136">Referência da API</span><span class="sxs-lookup"><span data-stu-id="15718-136">API reference</span></span>
<span data-ttu-id="15718-137">Está procurando a referência de API para esse serviço?</span><span class="sxs-lookup"><span data-stu-id="15718-137">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="15718-138">API de Impressão Universal no Microsoft Graph beta</span><span class="sxs-lookup"><span data-stu-id="15718-138">Universal Print API in Microsoft Graph beta</span></span>](/graph/api/resources/print?view=graph-rest-beta)

## <a name="see-also"></a><span data-ttu-id="15718-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="15718-139">See also</span></span>

- [<span data-ttu-id="15718-140">O que é a impressão universal?</span><span class="sxs-lookup"><span data-stu-id="15718-140">What is Universal Print</span></span>](https://docs.microsoft.com/universal-print/fundamentals/universal-print-whatis)
- <span data-ttu-id="15718-141">Gostaríamos de ouvir seus comentários sobre as APIs de Impressão Universal em [UserVoice](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)!</span><span class="sxs-lookup"><span data-stu-id="15718-141">We'd love to hear your feedback about the Universal Print APIs over at [UserVoice](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)!</span></span>
