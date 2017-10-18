# <a name="getting-started-building-microsoft-graph-apps"></a><span data-ttu-id="8698b-101">Introdução à criação de aplicativos do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8698b-101">Getting started building Microsoft Graph apps</span></span>

<span data-ttu-id="8698b-p101">Os artigos desta seção fornecem orientações detalhadas sobre como criar aplicativos que se conectam ao Microsoft Graph em uma variedade de linguagens e plataformas de desenvolvimento. Cada artigo começa com um exemplo de projeto inicial para a plataforma apropriada e orienta para que você consiga adicionar funcionalidades que autenticam o usuário e fazem um exemplo de solicitação para que o Microsoft Graph envie um email da sua conta. O projeto concluído é idêntico ao [Exemplo de conexão no repositório do Microsoft Graph](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=connect) para essa plataforma.</span><span class="sxs-lookup"><span data-stu-id="8698b-p101">The articles in this section provide detailed guidance on how to build apps that connect to Microsoft Graph across a variety of languages and development platforms. Each article starts with a sample starter project for the appropriate platform, and walks you through adding functionality that authenticates the user and makes a sample request to have Microsoft Graph send an email from their account. The completed project is identical to the [Connect sample in the Microsoft Graph repo](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=connect) for that platform.</span></span>

<span data-ttu-id="8698b-105">Escolha o artigo correspondente ao provedor de autenticação e à plataforma de desenvolvimento de sua escolha e comece a conexão com o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8698b-105">Choose the article that covers the authentication provider and development platform of your choice, and get started connecting to Microsoft Graph.</span></span> <span data-ttu-id="8698b-106">Para mais informações, confira [Qual é a diferença do ponto de extremidade v2.0?](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-v2-compare)</span><span class="sxs-lookup"><span data-stu-id="8698b-106">For more information, see [What's different about the v2.0 endpoint?](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-v2-compare)</span></span>

<span data-ttu-id="8698b-107">Você pode seguir as etapas no artigo que aborda a plataforma de desenvolvimento que você escolheu ou, para obter rapidamente uma solução que funcione, tente a experiência de [início rápido](https://developer.microsoft.com/graph/quick-start).</span><span class="sxs-lookup"><span data-stu-id="8698b-107">You can follow the steps in the article that covers the development platform that you choose, or, to quickly get a working solution up and running, try out the [quick start](https://developer.microsoft.com/graph/quick-start) experience.</span></span>

<span data-ttu-id="8698b-p103">Para explorar os exemplos de Conexão concluídos, confira [Microsoft Graph](https://github.com/microsoftgraph) no GitHub. A tabela a seguir mostra os exemplos por provedor e plataforma de autenticação e observa se eles se conectam ao Microsoft Graph usando REST ou uma biblioteca de cliente do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8698b-p103">To explore the finished Connect samples, see [Microsoft Graph](https://github.com/microsoftgraph) in GitHub. The following table lists the samples by authentication provider and platform, and notes whether they connect to Microsoft Graph using REST or a Microsoft Graph client library.</span></span>

<table>
  <tr>
    <th><span data-ttu-id="8698b-110">Plataforma</span><span class="sxs-lookup"><span data-stu-id="8698b-110">Platform</span></span></th>
    <th><span data-ttu-id="8698b-111">Ponto de extremidade do Azure AD</span><span class="sxs-lookup"><span data-stu-id="8698b-111">Azure AD endpoint</span></span></th> 
    <th><span data-ttu-id="8698b-112">Ponto de extremidade do Azure AD v2.0</span><span class="sxs-lookup"><span data-stu-id="8698b-112">Azure AD v2.0 endpoint</span></span></th>
  </tr>
  <tr>
    <td><span data-ttu-id="8698b-113">Android</span><span class="sxs-lookup"><span data-stu-id="8698b-113">Android</span></span></td>
    <td><span data-ttu-id="8698b-114">
        <a href="https://github.com/microsoftgraph/android-java-connect-sample/tree/last_v1_auth">Exemplo de SDK</a>
    </span><span class="sxs-lookup"><span data-stu-id="8698b-114">
        <a href="https://github.com/microsoftgraph/android-java-connect-sample/tree/last_v1_auth">SDK sample</a>
    </span></span></td> 
        <td><span data-ttu-id="8698b-115">
                <a href="https://github.com/microsoftgraph/android-java-connect-sample">Exemplo de SDK</a> ou <a href="https://github.com/microsoftgraph/android-java-connect-rest-sample">Exemplo de REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="8698b-115">
                <a href="https://github.com/microsoftgraph/android-java-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/android-java-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="8698b-116">AngularJS</span><span class="sxs-lookup"><span data-stu-id="8698b-116">AngularJS</span></span></td>
    <td><span data-ttu-id="8698b-117">
        <a href="https://github.com/microsoftgraph/angular-connect-rest-sample/tree/last_v1_auth">Exemplo de REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="8698b-117">
        <a href="https://github.com/microsoftgraph/angular-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td> 
        <td><span data-ttu-id="8698b-118">
        <a href="https://github.com/microsoftgraph/angular-connect-sample">Exemplo de SDK</a> ou <a href="https://github.com/microsoftgraph/angular-connect-rest-sample">Exemplo de REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="8698b-118">
        <a href="https://github.com/microsoftgraph/angular-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/angular-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="8698b-119">ASP.NET</span><span class="sxs-lookup"><span data-stu-id="8698b-119">ASP.NET</span></span></td>
    <td><span data-ttu-id="8698b-120">
        <a href="https://github.com/microsoftgraph/aspnet-connect-rest-sample/tree/last_v1_auth">Exemplo de REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="8698b-120">
        <a href="https://github.com/microsoftgraph/aspnet-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="8698b-121">
        <a href="https://github.com/microsoftgraph/aspnet-connect-sample">Exemplo de SDK</a> ou <a href="https://github.com/microsoftgraph/aspnet-connect-rest-sample">Exemplo de REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="8698b-121">
        <a href="https://github.com/microsoftgraph/aspnet-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/aspnet-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="8698b-122">iOS (Obj-C)</span><span class="sxs-lookup"><span data-stu-id="8698b-122">iOS (Obj-C)</span></span></td>
    <td><span data-ttu-id="8698b-123">
        <a href="https://github.com/microsoftgraph/ios-objectivec-connect-rest-sample">Exemplo de REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="8698b-123">
        <a href="https://github.com/microsoftgraph/ios-objectivec-connect-rest-sample">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="8698b-124">
        <a href="https://github.com/microsoftgraph/ios-objectivec-connect-sample">Exemplo de SDK</a>
    </span><span class="sxs-lookup"><span data-stu-id="8698b-124">
        <a href="https://github.com/microsoftgraph/ios-objectivec-connect-sample">SDK sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="8698b-125">iOS (Swift)</span><span class="sxs-lookup"><span data-stu-id="8698b-125">iOS (Swift)</span></span></td>
    <td><span data-ttu-id="8698b-126">
        <a href="https://github.com/microsoftgraph/ios-swift-connect-rest-sample">Exemplo de REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="8698b-126">
        <a href="https://github.com/microsoftgraph/ios-swift-connect-rest-sample">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="8698b-127">
        <a href="https://github.com/microsoftgraph/ios-swift-connect-sample">Exemplo de SDK</a>
    </span><span class="sxs-lookup"><span data-stu-id="8698b-127">
        <a href="https://github.com/microsoftgraph/ios-swift-connect-sample">SDK sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="8698b-128">NodeJS</span><span class="sxs-lookup"><span data-stu-id="8698b-128">NodeJS</span></span></td>
    <td><span data-ttu-id="8698b-129">
        <a href="https://github.com/microsoftgraph/nodejs-connect-rest-sample/tree/last_v1_auth">Exemplo de REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="8698b-129">
        <a href="https://github.com/microsoftgraph/nodejs-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td>     
    <td>    
        <span data-ttu-id="8698b-130"><a href="https://github.com/microsoftgraph/nodejs-connect-sample">Exemplo de SDK</a> ou <a href="https://github.com/microsoftgraph/nodejs-connect-rest-sample">Exemplo de REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="8698b-130"><a href="https://github.com/microsoftgraph/nodejs-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/nodejs-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="8698b-131">PHP</span><span class="sxs-lookup"><span data-stu-id="8698b-131">PHP</span></span></td>
    <td><span data-ttu-id="8698b-132">
        <a href="https://github.com/microsoftgraph/php-connect-rest-sample/tree/last_v1_auth">Exemplo de REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="8698b-132">
        <a href="https://github.com/microsoftgraph/php-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="8698b-133">
            <a href="https://github.com/microsoftgraph/php-connect-sample">Exemplo de SDK</a> ou <a href="https://github.com/microsoftgraph/php-connect-rest-sample">Exemplo de REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="8698b-133">
            <a href="https://github.com/microsoftgraph/php-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/php-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="8698b-134">Python</span><span class="sxs-lookup"><span data-stu-id="8698b-134">Python</span></span></td>
    <td><span data-ttu-id="8698b-135">
        <a href="https://github.com/microsoftgraph/python3-connect-rest-sample">Exemplo de REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="8698b-135">
        <a href="https://github.com/microsoftgraph/python3-connect-rest-sample">REST sample</a>
    </span></span></td>     
    <td>
    </td> 
  </tr>
  <tr>
    <td><span data-ttu-id="8698b-136">Ruby</span><span class="sxs-lookup"><span data-stu-id="8698b-136">Ruby</span></span></td>
    <td><span data-ttu-id="8698b-137">
        <a href="https://github.com/microsoftgraph/ruby-connect-rest-sample/tree/last_v1_auth">Exemplo de REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="8698b-137">
        <a href="https://github.com/microsoftgraph/ruby-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="8698b-138">
        <a href="https://github.com/microsoftgraph/ruby-connect-rest-sample">Exemplo de REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="8698b-138">
        <a href="https://github.com/microsoftgraph/ruby-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="8698b-139">UWP</span><span class="sxs-lookup"><span data-stu-id="8698b-139">UWP</span></span></td>
    <td><span data-ttu-id="8698b-140">
        <a href="https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample/tree/last_v1_auth">Exemplo de REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="8698b-140">
        <a href="https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="8698b-141">
        <a href="https://github.com/microsoftgraph/uwp-csharp-connect-sample">Exemplo de SDK</a> ou <a href="https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample">Exemplo de REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="8698b-141">
        <a href="https://github.com/microsoftgraph/uwp-csharp-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="8698b-142">Xamarin</span><span class="sxs-lookup"><span data-stu-id="8698b-142">Xamarin</span></span></td>
    <td>
    </td>     
    <td><span data-ttu-id="8698b-143">
        <a href="https://github.com/microsoftgraph/xamarin-csharp-connect-sample">Exemplo de SDK</a>
    </span><span class="sxs-lookup"><span data-stu-id="8698b-143">
        <a href="https://github.com/microsoftgraph/xamarin-csharp-connect-sample">SDK sample</a>
    </span></span></td> 
  </tr>
</table>

## <a name="see-also"></a><span data-ttu-id="8698b-144">Confira também</span><span class="sxs-lookup"><span data-stu-id="8698b-144">See also</span></span>

- <span data-ttu-id="8698b-145">Experimente as chamadas REST de exemplo no [Explorador do Graph](https://developer.microsoft.com/en-us/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="8698b-145">Try out sample REST calls in our [API Explorer](https://developer.microsoft.com/en-us/graph/graph-explorer).</span></span>
- [<span data-ttu-id="8698b-146">Documentação de ponto de extremidade do Microsoft Azure AD</span><span class="sxs-lookup"><span data-stu-id="8698b-146">Azure AD endpoint documentation</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-developers-guide)
- [<span data-ttu-id="8698b-147">Documentação de ponto de extremidade do Azure AD v2.0</span><span class="sxs-lookup"><span data-stu-id="8698b-147">Azure AD v2.0 endpoint documentation</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-appmodel-v2-overview)
