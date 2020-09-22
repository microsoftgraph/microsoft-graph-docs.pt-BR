---
title: Use a API de Descoberta Eletrônica do Microsoft Graph
description: As APIs de Descoberta Eletrônica do Microsoft 365 fornecem funcionalidade para as organizações automatizarem as tarefas repetitivas e se integrarem às ferramentas existentes de Descoberta Eletrônica para criar um fluxo de trabalho repetível que pode ser necessário com base nos regulamentos do setor. Você pode usar as APIs de Descoberta Eletrônica para ajudar com as suas necessidades legais.
localization_priority: Priority
author: mahage-msft
ms.prod: compliance
doc_type: conceptualPageType
ms.openlocfilehash: c7300fa41a6264b4006aca3a2d5049d10f30341f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47986095"
---
# <a name="use-the-microsoft-graph-ediscovery-api"></a><span data-ttu-id="76d5a-104">Use a API de Descoberta Eletrônica do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="76d5a-104">Use the Microsoft Graph eDiscovery API</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76d5a-105">As APIs do Microsoft Graph para Descoberta Eletrônica fornecem funcionalidade para que as organizações automatizem as tarefas repetitivas e se integrem às suas ferramentas existentes de Descoberta Eletrônica para criar fluxos de trabalho repetíveis que podem ser necessários com base nos regulamentos do setor.</span><span class="sxs-lookup"><span data-stu-id="76d5a-105">The Microsoft Graph APIs for eDiscovery provide functionality for organizations to automate repetitive tasks and integrate with their existing eDiscovery tools to build a repeatable workflows that might be required based on industry regulations.</span></span> <span data-ttu-id="76d5a-106">Você pode usar as APIs de Descoberta Eletrônica para ajudar com as suas necessidades legais.</span><span class="sxs-lookup"><span data-stu-id="76d5a-106">You can use the eDiscovery APIs to help with your legal needs.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="76d5a-107">As APIs do Microsoft Graph para Descoberta Eletrônica destinam-se ao uso de operações de Descoberta Eletrônica para requisições de Litígio, Investigação e regulamentação.</span><span class="sxs-lookup"><span data-stu-id="76d5a-107">The Microsoft Graph APIs for eDiscovery are intended for the use of eDiscovery operations for Litigation, Investigation and regulatory requests.</span></span> <span data-ttu-id="76d5a-108">Essas APIs não devem ser usadas como um substituto para os dados de registro no diário do sistema Microsoft 365 ou qualquer outro download em massa.</span><span class="sxs-lookup"><span data-stu-id="76d5a-108">These APIs should not be used as a substitute for journaling data out of the Microsoft 365 system or any other mass download.</span></span>

> [!NOTE]
> <span data-ttu-id="76d5a-109">Durante a visualização, o uso destas APIs pode exigir uma assinaturas de ofertas específicas da Microsoft e está sujeito aos [Termos de Uso de APIs Microsoft](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use?context=graph/context).</span><span class="sxs-lookup"><span data-stu-id="76d5a-109">During the preview, usage of these APIs may require subscriptions to specific Microsoft offerings and is subject to the [Microsoft APIs Terms of Use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use?context=graph/context).</span></span>  <span data-ttu-id="76d5a-110">Mediante disponibilidade geral, a Microsoft pode exigir que você ou o seu cliente paguem taxas adicionais.</span><span class="sxs-lookup"><span data-stu-id="76d5a-110">Upon general availability, Microsoft may require you or your customer to pay additional fees.</span></span>
>
> <span data-ttu-id="76d5a-111">Atualmente, as APIs de Descoberta Eletrônica no Microsoft Graph funcionam apenas em casos de Descoberta Eletrônica Avançada.</span><span class="sxs-lookup"><span data-stu-id="76d5a-111">Currently, the eDiscovery APIs in Microsoft Graph only work with Advanced eDiscovery cases.</span></span>

<span data-ttu-id="76d5a-112">A API do Microsoft Graph inclui as seguintes entidades principais.</span><span class="sxs-lookup"><span data-stu-id="76d5a-112">The Microsoft Graph API includes the following key entities.</span></span>

| <span data-ttu-id="76d5a-113">Nome</span><span class="sxs-lookup"><span data-stu-id="76d5a-113">Name</span></span> | <span data-ttu-id="76d5a-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="76d5a-114">Type</span></span>       | <span data-ttu-id="76d5a-115">Caso de uso</span><span class="sxs-lookup"><span data-stu-id="76d5a-115">Use case</span></span> |
|:-|:-|:-|
| <span data-ttu-id="76d5a-116">Caso de Descoberta Eletrônica</span><span class="sxs-lookup"><span data-stu-id="76d5a-116">eDiscovery case</span></span> | [<span data-ttu-id="76d5a-117">ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="76d5a-117">ediscoveryCase</span></span>](ediscoverycase.md) | <span data-ttu-id="76d5a-118">Os casos de Descoberta Eletrônica são o contêiner para todos os objetos de Descoberta Eletrônica, incluindo custodiantes, retenções, pesquisas, conjunto de revisões e exportações.</span><span class="sxs-lookup"><span data-stu-id="76d5a-118">eDiscovery cases are the container for all eDiscovery objects including custodians, holds, searches, review set and exports.</span></span> |
| <span data-ttu-id="76d5a-119">Conjunto de revisão de Descoberta Eletrônica</span><span class="sxs-lookup"><span data-stu-id="76d5a-119">eDiscovery review set</span></span>| [<span data-ttu-id="76d5a-120">reviewSet</span><span class="sxs-lookup"><span data-stu-id="76d5a-120">reviewSet</span></span>](reviewset.md) | <span data-ttu-id="76d5a-121">Os conjuntos de revisões de Descoberta Eletrônica são um conjunto estático de informações armazenadas eletronicamente coletadas para uso em um litígio, investigação ou solicitação regulatória.</span><span class="sxs-lookup"><span data-stu-id="76d5a-121">eDiscovery review sets are static set of electronically stored information collected for use in a litigation, investigation or regulatory request.</span></span> |
| <span data-ttu-id="76d5a-122">Consulta do conjunto de revisão de Descoberta Eletrônica</span><span class="sxs-lookup"><span data-stu-id="76d5a-122">eDiscovery review set query</span></span> | [<span data-ttu-id="76d5a-123">reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="76d5a-123">reviewSetQuery</span></span>](reviewsetquery.md) | <span data-ttu-id="76d5a-124">As consultas do conjunto de revisão de Descoberta Eletrônica são usadas para descobrir, selecionar, revisar e marcar [ ESI ](https://en.wikipedia.org/wiki/Electronically_stored_information_(Federal_Rules_of_Civil_Procedure)) com o objetivo final de produção para o solicitante ou o advogado adversário.</span><span class="sxs-lookup"><span data-stu-id="76d5a-124">eDiscovery review set queries are used to discover, cull, review and tag [ESI](https://en.wikipedia.org/wiki/Electronically_stored_information_(Federal_Rules_of_Civil_Procedure)) with the ultimate goal of production to the requestor or opposing counsel.</span></span>



