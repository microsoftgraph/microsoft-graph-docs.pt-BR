---
title: Visão geral Graph SDKs da Microsoft
description: Descreve os SDKs que estão disponíveis, as plataformas que eles suportam e o valor que eles fornecem aos desenvolvedores.
localization_priority: Normal
author: MichaelMainer
ms.custom: scenarios:getting-started
ms.openlocfilehash: 764bfe113c0bd66170eec1e21c2a1abddaf8b28e
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546914"
---
# <a name="microsoft-graph-sdks-overview"></a><span data-ttu-id="2c34a-103">Visão geral Graph SDKs da Microsoft</span><span class="sxs-lookup"><span data-stu-id="2c34a-103">Microsoft Graph SDKs overview</span></span>

<span data-ttu-id="2c34a-104">Os SDKs Graph Microsoft foram projetados para simplificar a criação de aplicativos de alta qualidade, eficientes e resilientes que acessam o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2c34a-104">The Microsoft Graph SDKs are designed to simplify building high-quality, efficient, and resilient applications that access Microsoft Graph.</span></span> <span data-ttu-id="2c34a-105">Os SDKs incluem dois componentes: uma biblioteca de serviços e uma biblioteca principal.</span><span class="sxs-lookup"><span data-stu-id="2c34a-105">The SDKs include two components: a service library and a core library.</span></span>

<span data-ttu-id="2c34a-106">A biblioteca de serviços contém modelos e construtores de solicitação que são gerados a partir dos metadados do Microsoft Graph para fornecer uma experiência rica, fortemente digitada e descobrivel ao trabalhar com os muitos conjuntos de dados disponíveis no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2c34a-106">The service library contains models and request builders that are generated from Microsoft Graph metadata to provide a rich, strongly typed, and discoverable experience when working with the many datasets available in Microsoft Graph.</span></span>

<span data-ttu-id="2c34a-107">A biblioteca principal fornece um conjunto de recursos que aprimoram o trabalho com todos os serviços Graph Microsoft.</span><span class="sxs-lookup"><span data-stu-id="2c34a-107">The core library provides a set of features that enhance working with all the Microsoft Graph services.</span></span> <span data-ttu-id="2c34a-108">O suporte incorporado para tratamento de nova tentativa, redirecionamentos seguros, autenticação transparente e compactação de carga, melhora a qualidade das interações do aplicativo com o Microsoft Graph, sem nenhuma complexidade adicionada, deixando você completamente no controle.</span><span class="sxs-lookup"><span data-stu-id="2c34a-108">Embedded support for retry handling, secure redirects, transparent authentication, and payload compression, improve the quality of your application's interactions with Microsoft Graph, with no added complexity, while leaving you completely in control.</span></span> <span data-ttu-id="2c34a-109">A biblioteca principal também oferece suporte para tarefas comuns, como pajamento por meio de coleções e criação de solicitações em lotes.</span><span class="sxs-lookup"><span data-stu-id="2c34a-109">The core library also provides support for common tasks such as paging through collections and creating batch requests.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/hDnsd2nJf88]


## <a name="supported-platforms"></a><span data-ttu-id="2c34a-110">Plataformas compatíveis</span><span class="sxs-lookup"><span data-stu-id="2c34a-110">Supported platforms</span></span>

<span data-ttu-id="2c34a-111">Atualmente, os SDKs estão disponíveis para os seguintes idiomas e plataformas:</span><span class="sxs-lookup"><span data-stu-id="2c34a-111">SDKs are currently available for the following languages and platforms:</span></span>

- [<span data-ttu-id="2c34a-112">Android</span><span class="sxs-lookup"><span data-stu-id="2c34a-112">Android</span></span>](https://developer.microsoft.com/en-us/graph/get-started/android)
- [<span data-ttu-id="2c34a-113">Angular</span><span class="sxs-lookup"><span data-stu-id="2c34a-113">Angular</span></span>](https://developer.microsoft.com/en-us/graph/get-started/angular)
- [<span data-ttu-id="2c34a-114">ASP.NET</span><span class="sxs-lookup"><span data-stu-id="2c34a-114">ASP.NET</span></span>](https://developer.microsoft.com/en-us/graph/get-started/asp.net)
- [<span data-ttu-id="2c34a-115">iOS</span><span class="sxs-lookup"><span data-stu-id="2c34a-115">iOS</span></span>](https://developer.microsoft.com/en-us/graph/get-started/ios)
- [<span data-ttu-id="2c34a-116">Javascript</span><span class="sxs-lookup"><span data-stu-id="2c34a-116">Javascript</span></span>](https://developer.microsoft.com/en-us/graph/get-started/javascript)
- [<span data-ttu-id="2c34a-117">Node.js</span><span class="sxs-lookup"><span data-stu-id="2c34a-117">Node.js</span></span>](https://developer.microsoft.com/en-us/graph/get-started/node.js)
- [<span data-ttu-id="2c34a-118">Java</span><span class="sxs-lookup"><span data-stu-id="2c34a-118">Java</span></span>](https://developer.microsoft.com/en-us/graph/get-started/java)
- [<span data-ttu-id="2c34a-119">PHP</span><span class="sxs-lookup"><span data-stu-id="2c34a-119">PHP</span></span>](https://developer.microsoft.com/en-us/graph/get-started/php)
- [<span data-ttu-id="2c34a-120">Python</span><span class="sxs-lookup"><span data-stu-id="2c34a-120">Python</span></span>](https://developer.microsoft.com/en-us/graph/get-started/python)
- [<span data-ttu-id="2c34a-121">Ruby</span><span class="sxs-lookup"><span data-stu-id="2c34a-121">Ruby</span></span>](https://developer.microsoft.com/en-us/graph/get-started/ruby)

## <a name="microsoft-365-developer-subscription"></a><span data-ttu-id="2c34a-122">Microsoft 365 de desenvolvedor</span><span class="sxs-lookup"><span data-stu-id="2c34a-122">Microsoft 365 developer subscription</span></span>

<span data-ttu-id="2c34a-123">Ao criar aplicativos usando o Microsoft Graph, recomendamos que você receba uma assinatura de desenvolvedor gratuita Microsoft 365 se inscrever no programa Microsoft 365 [Desenvolvedor.](https://developer.microsoft.com/microsoft-365/dev-program)</span><span class="sxs-lookup"><span data-stu-id="2c34a-123">When building applications using Microsoft Graph, we recommend that you get a free Microsoft 365 developer subscription by signing up for the [Microsoft 365 Developer Program](https://developer.microsoft.com/microsoft-365/dev-program).</span></span>

## <a name="see-also"></a><span data-ttu-id="2c34a-124">Confira também</span><span class="sxs-lookup"><span data-stu-id="2c34a-124">See also</span></span>

<span data-ttu-id="2c34a-125">A documentação de [requisitos de design](https://github.com/microsoftgraph/msgraph-sdk-design) do SDK fornece mais detalhes sobre os recursos e os recursos do SDK.</span><span class="sxs-lookup"><span data-stu-id="2c34a-125">The SDK [design requirements documentation](https://github.com/microsoftgraph/msgraph-sdk-design) provides more details about the features and capabilities of the SDK.</span></span> <span data-ttu-id="2c34a-126">Solicite ou vote em recursos adicionais no fórum Microsoft 365 de ideias da Plataforma de [Desenvolvedores.](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph)</span><span class="sxs-lookup"><span data-stu-id="2c34a-126">Request or vote on additional features at the [Microsoft 365 Developer Platform ideas forum](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph).</span></span> <span data-ttu-id="2c34a-127">Para ver uma lista de SDKs e exemplos para o Microsoft Graph, consulte a página recursos do [Microsoft Graph.](https://developer.microsoft.com/en-us/graph/gallery/?filterBy=Samples,SDKs)</span><span class="sxs-lookup"><span data-stu-id="2c34a-127">For a list of SDKs and samples for Microsoft Graph, see the [Microsoft Graph resources page](https://developer.microsoft.com/en-us/graph/gallery/?filterBy=Samples,SDKs).</span></span>
