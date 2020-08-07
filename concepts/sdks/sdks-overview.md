---
title: Visão geral dos SDKs do Microsoft Graph
description: Descreve os SDKs que estão disponíveis, as plataformas que eles dão suporte e o valor que eles fornecem aos desenvolvedores.
localization_priority: Normal
author: MichaelMainer
ms.custom: scenarios:getting-started
ms.openlocfilehash: b839b9a7ae0a32a22c9d20a61c96d021137388e3
ms.sourcegitcommit: 93b6781adf2c889235022d34ab50e2a4d62760c5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/07/2020
ms.locfileid: "46589302"
---
# <a name="microsoft-graph-sdks-overview"></a><span data-ttu-id="0da97-103">Visão geral dos SDKs do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="0da97-103">Microsoft Graph SDKs overview</span></span>

<span data-ttu-id="0da97-104">Os SDKs do Microsoft Graph foram projetados para simplificar a criação de aplicativos de alta qualidade, eficientes e resistentes que acessam o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="0da97-104">The Microsoft Graph SDKs are designed to simplify building high-quality, efficient, and resilient applications that access Microsoft Graph.</span></span> <span data-ttu-id="0da97-105">Os SDKs incluem dois componentes: uma biblioteca de serviços e uma biblioteca principal.</span><span class="sxs-lookup"><span data-stu-id="0da97-105">The SDKs include two components: a service library and a core library.</span></span>

<span data-ttu-id="0da97-106">A biblioteca de serviços contém modelos e criadores de solicitação que são gerados a partir de metadados do Microsoft Graph para fornecer uma experiência avançada, fortemente tipada e detectável, ao trabalhar com os vários conjuntos de valores disponíveis no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="0da97-106">The service library contains models and request builders that are generated from Microsoft Graph metadata to provide a rich, strongly typed, and discoverable experience when working with the many datasets available in Microsoft Graph.</span></span>

<span data-ttu-id="0da97-107">A biblioteca principal fornece um conjunto de recursos que melhoram o trabalho com todos os serviços do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="0da97-107">The core library provide a set of features that enhance working with all the Microsoft Graph services.</span></span> <span data-ttu-id="0da97-108">Suporte incorporado para tratamento de repetição, redirecionamentos de segurança, autenticação transparente e compactação de carga, melhore a qualidade das interações de seu aplicativo com o Microsoft Graph, sem complexidade adicional, enquanto deixa você totalmente no controle.</span><span class="sxs-lookup"><span data-stu-id="0da97-108">Embedded support for retry handling, secure redirects, transparent authentication, and payload compression, improve the quality of your application's interactions with Microsoft Graph, with no added complexity, while leaving you completely in control.</span></span> <span data-ttu-id="0da97-109">A biblioteca principal também fornece suporte para tarefas comuns, como paginação através de coleções e criação de solicitações em lote.</span><span class="sxs-lookup"><span data-stu-id="0da97-109">The core library also provides support for common tasks such as paging through collections and creating batch requests.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/hDnsd2nJf88]


## <a name="supported-platforms"></a><span data-ttu-id="0da97-110">Plataformas compatíveis</span><span class="sxs-lookup"><span data-stu-id="0da97-110">Supported platforms</span></span>

<span data-ttu-id="0da97-111">Os SDKs estão disponíveis atualmente para os seguintes idiomas e plataformas:</span><span class="sxs-lookup"><span data-stu-id="0da97-111">SDKs are currently available for the following languages and platforms:</span></span>

- [<span data-ttu-id="0da97-112">Android</span><span class="sxs-lookup"><span data-stu-id="0da97-112">Android</span></span>](https://developer.microsoft.com/en-us/graph/get-started/android)
- [<span data-ttu-id="0da97-113">Angular</span><span class="sxs-lookup"><span data-stu-id="0da97-113">Angular</span></span>](https://developer.microsoft.com/en-us/graph/get-started/angular)
- [<span data-ttu-id="0da97-114">ASP.NET</span><span class="sxs-lookup"><span data-stu-id="0da97-114">ASP.NET</span></span>](https://developer.microsoft.com/en-us/graph/get-started/asp.net)
- [<span data-ttu-id="0da97-115">iOS</span><span class="sxs-lookup"><span data-stu-id="0da97-115">iOS</span></span>](https://developer.microsoft.com/en-us/graph/get-started/ios)
- [<span data-ttu-id="0da97-116">Javascript</span><span class="sxs-lookup"><span data-stu-id="0da97-116">Javascript</span></span>](https://developer.microsoft.com/en-us/graph/get-started/javascript)
- [<span data-ttu-id="0da97-117">Node.js</span><span class="sxs-lookup"><span data-stu-id="0da97-117">Node.js</span></span>](https://developer.microsoft.com/en-us/graph/get-started/node.js)
- [<span data-ttu-id="0da97-118">Java</span><span class="sxs-lookup"><span data-stu-id="0da97-118">Java</span></span>](https://developer.microsoft.com/en-us/graph/get-started/java)
- [<span data-ttu-id="0da97-119">PHP</span><span class="sxs-lookup"><span data-stu-id="0da97-119">PHP</span></span>](https://developer.microsoft.com/en-us/graph/get-started/php)
- [<span data-ttu-id="0da97-120">Python</span><span class="sxs-lookup"><span data-stu-id="0da97-120">Python</span></span>](https://developer.microsoft.com/en-us/graph/get-started/python)
- [<span data-ttu-id="0da97-121">Ruby</span><span class="sxs-lookup"><span data-stu-id="0da97-121">Ruby</span></span>](https://developer.microsoft.com/en-us/graph/get-started/ruby)

## <a name="microsoft-365-developer-subscription"></a><span data-ttu-id="0da97-122">Assinatura do desenvolvedor do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="0da97-122">Microsoft 365 developer subscription</span></span>

<span data-ttu-id="0da97-123">Ao criar aplicativos usando o Microsoft Graph, recomendamos que você obtenha uma assinatura gratuita do desenvolvedor do Microsoft 365 inscrevendo-se no [programa de desenvolvedor do microsoft 365](https://developer.microsoft.com/microsoft-365/dev-program).</span><span class="sxs-lookup"><span data-stu-id="0da97-123">When building applications using Microsoft Graph, we recommend that you get a free Microsoft 365 developer subscription by signing up for the [Microsoft 365 Developer Program](https://developer.microsoft.com/microsoft-365/dev-program).</span></span>

## <a name="see-also"></a><span data-ttu-id="0da97-124">Confira também</span><span class="sxs-lookup"><span data-stu-id="0da97-124">See also</span></span>

<span data-ttu-id="0da97-125">A [documentação de requisitos de design](https://github.com/microsoftgraph/msgraph-sdk-design) do SDK fornece mais detalhes sobre os recursos e recursos do SDK.</span><span class="sxs-lookup"><span data-stu-id="0da97-125">The SDK [design requirements documentation](https://github.com/microsoftgraph/msgraph-sdk-design) provides more details about the features and capabilities of the SDK.</span></span> <span data-ttu-id="0da97-126">Solicitar ou votar em recursos adicionais no site do [Microsoft Graph UserVoice](https://microsoftgraph.uservoice.com) .</span><span class="sxs-lookup"><span data-stu-id="0da97-126">Request or vote on additional features at the [Microsoft Graph UserVoice](https://microsoftgraph.uservoice.com) site.</span></span> <span data-ttu-id="0da97-127">Para obter uma lista de SDKs e exemplos do Microsoft Graph, consulte a [página recursos do Microsoft Graph](https://developer.microsoft.com/en-us/graph/gallery/?filterBy=Samples,SDKs).</span><span class="sxs-lookup"><span data-stu-id="0da97-127">For a list of SDKs and samples for Microsoft Graph, see the [Microsoft Graph resources page](https://developer.microsoft.com/en-us/graph/gallery/?filterBy=Samples,SDKs).</span></span>
